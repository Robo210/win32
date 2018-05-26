---
Description: Describes a log entry for an IP address audit event in IPAM.
audience: developer
author: REDMOND\\markl
manager: REDMOND\\markl
ms.assetid: 36bff35e-05f7-4926-a2e2-7137017adebe
ms.prod: windows-server-dev
ms.technology:
- internet-protocol-address-management
- windows-management-instrumentation
ms.tgt_platform: multiple
title: MSFT\_IPAM\_IpAuditLogEntry class
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
---

# MSFT\_IPAM\_IpAuditLogEntry class

Describes a log entry for an IP address audit event in IPAM.

The following syntax is simplified from Managed Object Format (MOF) code and includes all of the inherited properties.

## Syntax

``` syntax
[UMLPackagePath("CIM::System::Logs"), ClassVersion("1.0.0"), dynamic, provider("IPAMServerPSProvider"), AMENDMENT]
class MSFT_IPAM_IpAuditLogEntry : CIM_LogEntry
{
  string   Caption;
  string   Description;
  string   ElementName;
  string   RecordFormat;
  string   RecordData;
  string   Locale;
  uint16   PerceivedSeverity;
  string   InstanceID;
  string   LogInstanceID;
  string   LogName;
  string   RecordID;
  datetime CreationTimeStamp;
  string   MessageID;
  string   Message;
  string   MessageArguments[];
  datetime TimeOfEvent;
  string   IPAddress;
  uint16   EventType;
  string   HostName;
  string   UserName;
  string   ClientId;
  string   UserDomainName;
  string   UserForestName;
  string   SourceServer;
  uint16   ServerType;
};
```

## Members

The **MSFT\_IPAM\_IpAuditLogEntry** class has these types of members:

-   [Methods](#methods)
-   [Properties](#properties)

### Methods

The **MSFT\_IPAM\_IpAuditLogEntry** class has these methods.



| Method                                                                 | Description                                                                         |
|:-----------------------------------------------------------------------|:------------------------------------------------------------------------------------|
| [**RemoveIpAuditLog**](removeipauditlog-msft-ipam-ipauditlogentry.md) | Deletes IP address audit events that occurred before the specified date.<br/> |



 

### Properties

The **MSFT\_IPAM\_IpAuditLogEntry** class has these properties.

<dl> <dt>

**Caption**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: [**MaxLen**](https://msdn.microsoft.com/library/aa393650) (64)
</dt> </dl>

The Caption property is a short textual description (one- line string) of the object.

This property is inherited from [**CIM\_ManagedElement**](cim-managedelement.md).

</dd> <dt>

**ClientId**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> </dl>

The client Id from DHCP lease events.

</dd> <dt>

**CreationTimeStamp**
</dt> <dd> <dl> <dt>

Data type: **datetime**
</dt> <dt>

Access type: Read-only
</dt> </dl>

A LogEntry may include a timestamp for the entry.

This property is inherited from [**CIM\_LogEntry**](cim-logentry.md).

</dd> <dt>

**Description**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> </dl>

The Description property provides a textual description of the object.

This property is inherited from [**CIM\_ManagedElement**](cim-managedelement.md).

</dd> <dt>

**ElementName**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> </dl>

A user-friendly name for the object. This property allows each instance to define a user-friendly name in addition to its key properties, identity data, and description information.

This property is inherited from [**CIM\_ManagedElement**](cim-managedelement.md).

</dd> <dt>

**EventType**
</dt> <dd> <dl> <dt>

Data type: **uint16**
</dt> <dt>

Access type: Read-only
</dt> </dl>

The type of IP tracking for the event. This specifies the source of this particular audit data.

The possible values are.

<dt>

<span id="None"></span><span id="none"></span><span id="NONE"></span>

**None** (0)


</dt> <dd></dd> <dt>

<span id="DHCPNewLease"></span><span id="dhcpnewlease"></span><span id="DHCPNEWLEASE"></span>

**DHCPNewLease** (1)


</dt> <dd></dd> <dt>

<span id="DHCPRenewLease"></span><span id="dhcprenewlease"></span><span id="DHCPRENEWLEASE"></span>

**DHCPRenewLease** (2)


</dt> <dd></dd> <dt>

<span id="DHCPReleaseLease"></span><span id="dhcpreleaselease"></span><span id="DHCPRELEASELEASE"></span>

**DHCPReleaseLease** (3)


</dt> <dd></dd> <dt>

<span id="DHCPLeaseExpired"></span><span id="dhcpleaseexpired"></span><span id="DHCPLEASEEXPIRED"></span>

**DHCPLeaseExpired** (4)


</dt> <dd></dd> <dt>

<span id="DHCPDeleteLease"></span><span id="dhcpdeletelease"></span><span id="DHCPDELETELEASE"></span>

**DHCPDeleteLease** (5)


</dt> <dd></dd> <dt>

<span id="DHCPBootpLease"></span><span id="dhcpbootplease"></span><span id="DHCPBOOTPLEASE"></span>

**DHCPBootpLease** (6)


</dt> <dd></dd> <dt>

<span id="DHCPBootpDynamicLease"></span><span id="dhcpbootpdynamiclease"></span><span id="DHCPBOOTPDYNAMICLEASE"></span>

**DHCPBootpDynamicLease** (7)


</dt> <dd></dd> <dt>

<span id="DHCPStatelessInfoReq"></span><span id="dhcpstatelessinforeq"></span><span id="DHCPSTATELESSINFOREQ"></span>

**DHCPStatelessInfoReq** (8)


</dt> <dd></dd> <dt>

<span id="DHCPStatelessClientPurged"></span><span id="dhcpstatelessclientpurged"></span><span id="DHCPSTATELESSCLIENTPURGED"></span>

**DHCPStatelessClientPurged** (9)


</dt> <dd></dd> <dt>

<span id="DCAuthentication"></span><span id="dcauthentication"></span><span id="DCAUTHENTICATION"></span>

**DCAuthentication** (10)


</dt> <dd></dd> <dt>

<span id="NPSAuthentication"></span><span id="npsauthentication"></span><span id="NPSAUTHENTICATION"></span>

**NPSAuthentication** (11)


</dt> <dd></dd> </dl>

</dd> <dt>

**HostName**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> </dl>

The hostname from DHCP lease events.

</dd> <dt>

**InstanceID**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: [**key**](https://msdn.microsoft.com/library/aa392157)
</dt> </dl>

Within the scope of the instantiating Namespace, InstanceID opaquely and uniquely identifies an instance of this class. In order to ensure uniqueness within the NameSpace, the value of InstanceID SHOULD be constructed using the following 'preferred' algorithm:

&lt;OrgID&gt;:&lt;LocalID&gt;

Where &lt;OrgID&gt; and &lt;LocalID&gt; are separated by a colon ':', and where &lt;OrgID&gt; MUST include a copyrighted, trademarked or otherwise unique name that is owned by the business entity creating/defining the InstanceID, or is a registered ID that is assigned to the business entity by a recognized global authority (This is similar to the &lt;Schema Name&gt;\_&lt;Class Name&gt; structure of Schema class names.) In addition, to ensure uniqueness &lt;OrgID&gt; MUST NOT contain a colon (':'). When using this algorithm, the first colon to appear in InstanceID MUST appear between &lt;OrgID&gt; and &lt;LocalID&gt;.

&lt;LocalID&gt; is chosen by the business entity and SHOULD not be re-used to identify different underlying (real-world) elements. If the above 'preferred' algorithm is not used, the defining entity MUST assure that the resultant InstanceID is not re-used across any InstanceIDs produced by this or other providers for this instance's NameSpace.

For DMTF defined instances, the 'preferred' algorithm MUST be used with the &lt;OrgID&gt; set to 'CIM'.

This property is inherited from [**CIM\_LogEntry**](cim-logentry.md).

</dd> <dt>

**IPAddress**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> </dl>

The IP Address from DHCP lease events.

</dd> <dt>

**Locale**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> </dl>

A locale indicates a particular geographical, political, or cultural region. The Locale specifies the language used in creating the RecordForLog data. If the Locale property is empty, it is assumed that the default locale is en\_US (English).

The locale string consists of three sub-strings, separated by underscores:

\- The first sub-string is the language code, as specified in ISO639.

\- The second sub-string is the country code, as specified in ISO3166.

\- The third sub-string is a variant, which is vendor specific.

For example, US English appears as: "en\_US\_WIN", where the "WIN" variant would specify a Windows browser-specific collation (if one exists). Since the variant is not standardized, it is not commonly used and generally is limited to easily recognizable values ("WIN", "UNIX", "EURO", etc.) used in standard environments. The language and country codes are required; the variant may be empty.

This property is inherited from [**CIM\_RecordForLog**](cim-recordforlog.md).

</dd> <dt>

**LogInstanceID**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: [**MaxLen**](https://msdn.microsoft.com/library/aa393650) (256)
</dt> </dl>

The containing Log's InstanceID.

This property is inherited from [**CIM\_LogEntry**](cim-logentry.md).

</dd> <dt>

**LogName**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: [**MaxLen**](https://msdn.microsoft.com/library/aa393650) (256)
</dt> </dl>

The containing Log's Name. This property is available for backwards continuity with CIM\_LogRecord.

This property is inherited from [**CIM\_LogEntry**](cim-logentry.md).

</dd> <dt>

**Message**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: [**ModelCorrespondence**](https://msdn.microsoft.com/library/aa393650) ("CIM\_LogEntry.MessageID", "CIM\_LogEntry.MessageArguments")
</dt> </dl>

The formatted message. This message is constructed by combining some or all of the dynamic elements specified in the MessageArguments property with the static elements uniquely identified by the MessageID in a message registry or other catalog associated with the OwningEntity.

This property is inherited from [**CIM\_LogEntry**](cim-logentry.md).

</dd> <dt>

**MessageArguments**
</dt> <dd> <dl> <dt>

Data type: **string** array
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: [**ModelCorrespondence**](https://msdn.microsoft.com/library/aa393650) ("CIM\_LogEntry.Message", "CIM\_LogEntry.MessageID")
</dt> </dl>

An array containing the dynamic content of the message.

Each DYNAMIC\_ELEMENT for the message referred to by the MessageID property shall be contained in MessageArguments whether the DYNAMIC\_ELEMENT is included in the Message or not.

In addition, the entries in MessageArguments need to be in the same order as the DYNAMIC\_ELEMENTs.

This property is inherited from [**CIM\_LogEntry**](cim-logentry.md).

</dd> <dt>

**MessageID**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: [**ModelCorrespondence**](https://msdn.microsoft.com/library/aa393650) ("CIM\_LogEntry.Message", "CIM\_LogEntry.MessageArguments")
</dt> </dl>

A string that uniquely identifies, within the scope of the OwningEntity, the format of the Message.

This property is inherited from [**CIM\_LogEntry**](cim-logentry.md).

</dd> <dt>

**PerceivedSeverity**
</dt> <dd> <dl> <dt>

Data type: **uint16**
</dt> <dt>

Access type: Read-only
</dt> </dl>

Describes the severity of the Indication from the originator's point of view.

This property is inherited from [**CIM\_RecordForLog**](cim-recordforlog.md).

The possible values are.

<dt>

<span id="Unknown"></span><span id="unknown"></span><span id="UNKNOWN"></span>

<span id="Unknown"></span><span id="unknown"></span><span id="UNKNOWN"></span>**Unknown** (0)


</dt> <dd></dd> <dt>

<span id="Other"></span><span id="other"></span><span id="OTHER"></span>

<span id="Other"></span><span id="other"></span><span id="OTHER"></span>**Other** (1)


</dt> <dd></dd> <dt>

<span id="Information"></span><span id="information"></span><span id="INFORMATION"></span>

<span id="Information"></span><span id="information"></span><span id="INFORMATION"></span>**Information** (2)


</dt> <dd>

Informational only.

</dd> <dt>

<span id="Degraded_Warning"></span><span id="degraded_warning"></span><span id="DEGRADED_WARNING"></span>

<span id="Degraded_Warning"></span><span id="degraded_warning"></span><span id="DEGRADED_WARNING"></span>**Degraded/Warning** (3)


</dt> <dd>

The user decides if action is needed.

</dd> <dt>

<span id="Minor"></span><span id="minor"></span><span id="MINOR"></span>

<span id="Minor"></span><span id="minor"></span><span id="MINOR"></span>**Minor** (4)


</dt> <dd>

Not serious, but action is needed.

</dd> <dt>

<span id="Major"></span><span id="major"></span><span id="MAJOR"></span>

<span id="Major"></span><span id="major"></span><span id="MAJOR"></span>**Major** (5)


</dt> <dd>

Immediate action is needed.

</dd> <dt>

<span id="Critical"></span><span id="critical"></span><span id="CRITICAL"></span>

<span id="Critical"></span><span id="critical"></span><span id="CRITICAL"></span>**Critical** (6)


</dt> <dd>

Immediate action is needed for an issue with a broad scope or critical consequences.

</dd> <dt>

<span id="Fatal_NonRecoverable"></span><span id="fatal_nonrecoverable"></span><span id="FATAL_NONRECOVERABLE"></span>

<span id="Fatal_NonRecoverable"></span><span id="fatal_nonrecoverable"></span><span id="FATAL_NONRECOVERABLE"></span>**Fatal/NonRecoverable** (7)


</dt> <dd>

It is too late to take action on the indicated error.

</dd> </dl>

</dd> <dt>

**RecordData**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: [**ModelCorrespondence**](https://msdn.microsoft.com/library/aa393650) ("CIM\_RecordForLog.RecordFormat")
</dt> </dl>

A string containing LogRecord data.

If the corresponding RecordFormat property is &lt;empty&gt;, or cannot be parsed according to the recommended format, RecordData should be interpreted as a free-form string. If the RecordFormat property contains parseable format information (as recommended in the RecordFormat Description qualifier), the RecordData string SHOULD be parsed in accordance with this format. In this case, RecordData SHOULD begin with the delimiter character and this character SHOULD be used to separate substrings in the manner described. The RecordData string can then be parsed by the data consumer and appropriately typed.

This property is inherited from [**CIM\_RecordForLog**](cim-recordforlog.md).

</dd> <dt>

**RecordFormat**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: [**ModelCorrespondence**](https://msdn.microsoft.com/library/aa393650) ("CIM\_RecordForLog.RecordData")
</dt> </dl>

A string describing the data structure of the information in the property, RecordData. If the RecordFormat string is &lt;empty&gt;, RecordData should be interpreted as a free-form string.

To describe the data structure of RecordData, the RecordFormat string should be constructed as follows:

\- The first character is a delimiter character and is used to parse the remainder of the string into sub-strings.

\- Each sub-string is separated by the delimiter character and should be in the form of a CIM property declaration (i.e., datatype and property name). This set of declarations may be used to interpret the similarly delimited RecordData property.

For example, using a '\*' delimiter, RecordFormat = "\*string ThisDay\*uint32 ThisYear\*datetime SomeTime"

may be used to interpret: RecordData = "\*This is Friday\*2002\*20020807141000.000000-300".

This property is inherited from [**CIM\_RecordForLog**](cim-recordforlog.md).

</dd> <dt>

**RecordID**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: [**MaxLen**](https://msdn.microsoft.com/library/aa393650) (256)
</dt> </dl>

RecordID may be used to provide a representation of log entry ordering or pointers/handles for log entries.

This property is inherited from [**CIM\_LogEntry**](cim-logentry.md).

</dd> <dt>

**ServerType**
</dt> <dd> <dl> <dt>

Data type: **uint16**
</dt> <dt>

Access type: Read-only
</dt> </dl>

The type of server that contained the event.

The possible values are.

<dt>

<span id="None"></span><span id="none"></span><span id="NONE"></span>

**None** (0)


</dt> <dd></dd> <dt>

<span id="Ipam"></span><span id="ipam"></span><span id="IPAM"></span>

**Ipam** (1)


</dt> <dd></dd> <dt>

<span id="Dhcp"></span><span id="dhcp"></span><span id="DHCP"></span>

**Dhcp** (2)


</dt> <dd></dd> <dt>

<span id="Nps"></span><span id="nps"></span><span id="NPS"></span>

**Nps** (3)


</dt> <dd></dd> <dt>

<span id="Dc"></span><span id="dc"></span><span id="DC"></span>

**Dc** (4)


</dt> <dd></dd> </dl>

</dd> <dt>

**SourceServer**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> </dl>

The name of the server that contained the event.

</dd> <dt>

**TimeOfEvent**
</dt> <dd> <dl> <dt>

Data type: **datetime**
</dt> <dt>

Access type: Read-only
</dt> </dl>

The date and time when the event occurred.

</dd> <dt>

**UserDomainName**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> </dl>

The domain name from domain controller login events.

</dd> <dt>

**UserForestName**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> </dl>

Forest name collected from DC logon events.

**Windows Server 2012 R2:** This property is unavailable prior to Windows Server 2016.

</dd> <dt>

**UserName**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> </dl>

The username from DC logon events and NPS events.

</dd> </dl>

## Requirements



|                                     |                                                                                                     |
|-------------------------------------|-----------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | None supported<br/>                                                                           |
| Minimum supported server<br/> | Windows Server 2012 R2<br/>                                                                   |
| Namespace<br/>                | RootMicrosoftIPAM<br/>                                                                        |
| MOF<br/>                      | <dl> <dt>IPAMServerPSProvider.mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>IPAMServerPSProvider.dll</dt> </dl> |



## See also

<dl> <dt>

[**CIM\_LogEntry**](cim-logentry.md)
</dt> <dt>

[IPAM Server WMI Provider Reference](ipam-server-wmi-provider-reference.md)
</dt> </dl>

 

 



