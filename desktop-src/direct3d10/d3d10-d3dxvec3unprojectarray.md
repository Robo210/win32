---
Description: Projects an array (x, y, z, 0) from screen space into object space.
ms.assetid: 02db5b32-7fa3-4cde-bd63-0d8b3dfc31e7
title: D3DXVec3UnprojectArray function
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# D3DXVec3UnprojectArray function

Projects an array (x, y, z, 0) from screen space into object space.

## Syntax


```C++
D3DXVECTOR3* D3DXVec3UnprojectArray(
  _Inout_       D3DXVECTOR3    *pOut,
  _In_          UINT           OutStride,
  _In_    const D3DXVECTOR3    *pV,
  _In_          UINT           VStride,
  _In_    const D3D10_VIEWPORT *pViewport,
  _In_    const D3DXMATRIX     *pProjection,
  _In_    const D3DXMATRIX     *pView,
  _In_    const D3DXMATRIX     *pWorld,
  _In_          UINT           n
);
```



## Parameters

<dl> <dt>

*pOut* \[in, out\]
</dt> <dd>

Type: **[**D3DXVECTOR3**](direct3d9.d3dxvector3)\***

Pointer to the [**D3DXVECTOR3**](d3d10-d3dxvector3.md) that is the result of the operation.

</dd> <dt>

*OutStride* \[in\]
</dt> <dd>

Type: **[**UINT**](winprog.windows_data_types)**

Stride between vectors in the output data stream.

</dd> <dt>

*pV* \[in\]
</dt> <dd>

Type: **const [**D3DXVECTOR3**](direct3d9.d3dxvector3)\***

Pointer to the source D3DXVECTOR3 structure.

</dd> <dt>

*VStride* \[in\]
</dt> <dd>

Type: **[**UINT**](winprog.windows_data_types)**

Stride between vectors in the input data stream.

</dd> <dt>

*pViewport* \[in\]
</dt> <dd>

Type: **const [**D3D10\_VIEWPORT**](/windows/win32/D3D10/ns-d3d10-d3d10_viewport?branch=master)\***

Pointer to a [**D3D10\_VIEWPORT**](/windows/win32/D3D10/ns-d3d10-d3d10_viewport?branch=master), representing the viewport.

</dd> <dt>

*pProjection* \[in\]
</dt> <dd>

Type: **const [**D3DXMATRIX**](direct3d9.d3dxmatrix)\***

Pointer to a [**D3DXMATRIX**](d3d10-d3dxmatrix.md) structure, representing the projection matrix.

</dd> <dt>

*pView* \[in\]
</dt> <dd>

Type: **const [**D3DXMATRIX**](direct3d9.d3dxmatrix)\***

Pointer to a D3DXMATRIX structure, representing the view matrix.

</dd> <dt>

*pWorld* \[in\]
</dt> <dd>

Type: **const [**D3DXMATRIX**](direct3d9.d3dxmatrix)\***

Pointer to a D3DXMATRIX structure, representing the world matrix.

</dd> <dt>

*n* \[in\]
</dt> <dd>

Type: **[**UINT**](winprog.windows_data_types)**

Number of elements in the array.

</dd> </dl>

## Return value

Type: **[**D3DXVECTOR3**](direct3d9.d3dxvector3)\***

Pointer to a D3DXVECTOR3 structure that is the array projected from screen space to object space.

## Remarks

The return value for this function is the same value returned in the pOut parameter. In this way, the [**D3DXVec3Unproject**](d3d10-d3dxvec3unproject.md) function can be used as a parameter for another function.

## Requirements



|                   |                                                                                         |
|-------------------|-----------------------------------------------------------------------------------------|
| Header<br/> | <dl> <dt>D3DX10Math.h</dt> </dl> |



## See also

<dl> <dt>

[Math Functions](d3d10-graphics-reference-d3dx10-functions-math.md)
</dt> </dl>

 

 



