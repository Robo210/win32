---
Description: The MsiAssembly Table specifies Windows Installer settings for Microsoft .NET Framework assemblies and Win32 assemblies. For more information, see Installation of Assemblies to the Global Assembly Cache and Installation of Win32 Assemblies.
ms.assetid: 3a8cd206-0112-4840-8c9d-773483f5c771
title: MsiAssembly Table
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# MsiAssembly Table

The MsiAssembly Table specifies Windows Installer settings for Microsoft .NET Framework assemblies and Win32 assemblies. For more information, see [Installation of Assemblies to the Global Assembly Cache](installation-of-assemblies-to-the-global-assembly-cache.md) and [Installation of Win32 Assemblies](installation-of-win32-assemblies.md).

On Windows XP, Windows Installer can install Win32 assemblies as [side-by-side assemblies](side-by-side-assemblies.md). For more information, see the [Side-by-Side Assembly API](setup.side-by-side_assembly_api).

**Windows 2000:** This feature is not supported.

The MsiAssembly Table has the following columns.



| Column            | Type                         | Key | Nullable |
|-------------------|------------------------------|-----|----------|
| Component\_       | [Identifier](identifier.md) | Y   | N        |
| Feature\_         | [Identifier](identifier.md) | N   | N        |
| File\_Manifest    | [Identifier](identifier.md) | N   | Y        |
| File\_Application | [Identifier](identifier.md) | N   | Y        |
| Attributes        | [Integer](integer.md)       | N   | Y        |



 

## Columns

<dl> <dt>

<span id="Component_"></span><span id="component_"></span><span id="COMPONENT_"></span>Component\_
</dt> <dd>

The key into the [Component Table](component-table.md) that specifies the Windows Installer component that contains this assembly.

The value in this field must not be set to null. The component KeyPath field in the [Component Table](component-table.md) must not be null.

For Win32 assemblies, the component KeyPath cannot be the manifest file that is specified in File\_Manifest. The manifest can be the keypath for a .NET Framework or policy assembly.

</dd> <dt>

<span id="Feature_"></span><span id="feature_"></span><span id="FEATURE_"></span>Feature\_
</dt> <dd>

Key into the [Feature Table](feature-table.md).

When the assembly must be installed by a feature installation, Windows Installer installs the feature pointed to by this field.

</dd> <dt>

<span id="File_Manifest"></span><span id="file_manifest"></span><span id="FILE_MANIFEST"></span>File\_Manifest
</dt> <dd>

An external key into the [File Table](file-table.md) that specifies the file that contains the manifest for a .NET Framework assembly or Win32 assembly.

For a Win32 assembly, do not specify this file as the component key path file in the KeyPath field of the [Component Table](component-table.md).

</dd> <dt>

<span id="File_Application"></span><span id="file_application"></span><span id="FILE_APPLICATION"></span>File\_Application
</dt> <dd>

To install the assembly at a private location, enter the key path file for the assembly component in this field.

This is the value that appears in the KeyPath field of the [Component Table](component-table.md). The Installer can then install the assembly to the directory structure of the component that is specified in the [Directory Table](directory-table.md). This field must be null if the assembly is to be installed into the global assembly cache.

</dd> <dt>

<span id="Attributes"></span><span id="attributes"></span><span id="ATTRIBUTES"></span>Attributes
</dt> <dd>

Enter a value of 1 (one) for a Win32 assembly. Enter a value of 0 (zero) for a .NET Framework assembly.

If the Attributes column is NULL, the Installer treats the assembly as a .NET Framework assembly.

</dd> </dl>

## Remarks

If there is at least one entry in the MsiAssembly Table, the [InstallExecuteSequence Table](installexecutesequence-table.md) must contain the [MsiPublishAssemblies Action](msipublishassemblies-action.md), and [MsiUnpublishAssemblies Action](msiunpublishassemblies-action.md).

Because assemblies cannot be rolled back after they are committed, Windows Installer uses a two-step installation process. The interfaces to the assemblies are created during the installation operations that are generated by the [MsiPublishAssemblies Action](msipublishassemblies-action.md).

The assemblies are not committed until successful execution of the [InstallFinalize Action](installfinalize-action.md). This means that if you author a custom action or resource that relies on the assembly, it must be sequenced after the [InstallFinalize Action](installfinalize-action.md). For example, if you need to start a service that depends on an assembly in the Global Assembly Cache (GAC), you must schedule the starting of that service after the [InstallFinalize Action](installfinalize-action.md). This means you cannot use the [ServiceControl Table](servicecontrol-table.md) to start the service, instead you must use a custom action that is sequenced after InstallFinalize.

## Validation

<dl>

[ICE03](ice03.md)  
[ICE06](ice06.md)  
[ICE32](ice32.md)  
[ICE66](ice66.md)  
[ICE83](ice83.md)  
[ICE94](ice94.md)  
</dl>

 

 


