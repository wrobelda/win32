---
title: IEnumFsiItems RemoteNext method
description: Supports a remote client that wants to retrieve a specified number of items in the enumeration sequence.
ms.assetid: a5ae59ed-08d7-4225-9aec-91049789e8fe
keywords:
- RemoteNext method IMAPI
- RemoteNext method IMAPI , IEnumFsiItems interface
- IEnumFsiItems interface IMAPI , RemoteNext method
topic_type:
- apiref
api_name:
- IEnumFsiItems.RemoteNext
api_location:
- Imapi2fs.idl
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
---

# IEnumFsiItems::RemoteNext method

Supports a remote client that wants to retrieve a specified number of items in the enumeration sequence.

## Syntax


```C++
HRESULT RemoteNext(
  [in]  ULONG    celt,
  [out] IFsiItem **rgelt,
  [out] ULONG    *pceltFetched
);
```



## Parameters

<dl> <dt>

*celt* \[in\]
</dt> <dd>

Number of items to retrieve.

</dd> <dt>

*rgelt* \[out\]
</dt> <dd>

Array of [**IFsiItem**](/windows/desktop/api/imapi2fs/nn-imapi2fs-ifsiitem) interfaces. You must release each interface in rgelt when done.

</dd> <dt>

*pceltFetched* \[out\]
</dt> <dd>

Number of elements returned in rgelt. You can set *pceltFetched* to **NULL** if *celt* is one. Otherwise, initialize the value of *pceltFetched* to 0 before calling this method.

</dd> </dl>

## Return value

S\_OK is returned when the number of requested elements (*celt*) are returned successfully or the number of returned items (*pceltFetched*) is less than the number of requested elements.

Other success codes may be returned as a result of implementation. The following error codes are commonly returned on operation failure, but do not represent the only possible error values:



| Return code                                                                                   | Description                                                                     |
|-----------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------|
| <dl> <dt>**E\_POINTER**</dt> </dl>     | Pointer is not valid.<br/> Value: 0x80004003<br/>                   |
| <dl> <dt>**E\_OUTOFMEMORY**</dt> </dl> | Failed to allocate the required memory.<br/> Value: 0x8007000E<br/> |
| <dl> <dt>**E\_INVALIDARG**</dt> </dl>  | One or more arguments are not valid.<br/> Value: 0x80070057<br/>    |



 

## Requirements



|                                     |                                                                                         |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows Vista, Windows XP with SP2 \[desktop apps only\]<br/>                     |
| Minimum supported server<br/> | Windows Server 2003 \[desktop apps only\]<br/>                                    |
| IDL<br/>                      | <dl> <dt>Imapi2fs.idl</dt> </dl> |



## See also

<dl> <dt>

[**IEnumFsiItems**](/windows/desktop/api/imapi2fs/nn-imapi2fs-ienumfsiitems)
</dt> <dt>

[IEnumFsiItems::Next](/windows/desktop/api/imapi2fs/nf-imapi2fs-ienumfsiitems-next)
</dt> </dl>

 

 





