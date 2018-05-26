---
Description: Returns the shader version of the compiled shader.
ms.assetid: 6cc6c654-e8d1-4225-b5d0-6bc2434a16bd
title: D3DXGetShaderVersion function
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# D3DXGetShaderVersion function

Returns the shader version of the compiled shader.

## Syntax


```C++
DWORD D3DXGetShaderVersion(
  _In_ const DWORD *pFunction
);
```



## Parameters

<dl> <dt>

*pFunction* \[in\]
</dt> <dd>

Type: **const [**DWORD**](winprog.windows_data_types)\***

Pointer to the function DWORD stream.

</dd> </dl>

## Return value

Type: **[**DWORD**](winprog.windows_data_types)**

Returns the shader version of the given shader, or zero if the shader function is **NULL**.

## Requirements



|                    |                                                                                          |
|--------------------|------------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>D3DX9Shader.h</dt> </dl> |
| Library<br/> | <dl> <dt>D3dx9.lib</dt> </dl>     |



## See also

<dl> <dt>

[Shader Functions](dx9-graphics-reference-d3dx-functions-shader.md)
</dt> </dl>

 

 



