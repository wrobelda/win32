---
title: JET_DBINFOMISC.ulBadChecksumOld property  (Microsoft.Isam.Esent.Interop)
TOCTitle: 'ulBadChecksumOld property '
ms:assetid: P:Microsoft.Isam.Esent.Interop.JET_DBINFOMISC.ulBadChecksumOld
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/microsoft.isam.esent.interop.jet_dbinfomisc.ulbadchecksumold(v=EXCHG.10)
ms:contentKeyID: 39513159
ms.date: 07/30/2014
ms.topic: article
f1_keywords:
- Microsoft.Isam.Esent.Interop.JET_DBINFOMISC.ulBadChecksumOld
dev_langs:
- CSharp
- JScript
- VB
- other
api_name: 
- Microsoft.Isam.Esent.Interop.JET_DBINFOMISC.get_ulBadChecksumOld
- Microsoft.Isam.Esent.Interop.JET_DBINFOMISC.set_ulBadChecksumOld
- Microsoft.Isam.Esent.Interop.JET_DBINFOMISC.ulBadChecksumOld
topic_type: 
- kbSyntax
- apiref
api_type: 
- Managed
api_location: 
- Microsoft.Isam.Esent.Interop.dll
ROBOTS: INDEX,FOLLOW

---

# JET\_DBINFOMISC.ulBadChecksumOld property

Gets the number of times a non-correctable checksum error was found before the last repair.

**Namespace:**  [Microsoft.Isam.Esent.Interop](hh596136\(v=exchg.10\).md)  
**Assembly:**  Microsoft.Isam.Esent.Interop (in Microsoft.Isam.Esent.Interop.dll)

## Syntax

``` vb
'Declaration
Public Property ulBadChecksumOld As Integer
    Get
    Friend Set
'Usage
Dim instance As JET_DBINFOMISC
Dim value As Integer

value = instance.ulBadChecksumOld
```

``` csharp
public int ulBadChecksumOld { get; internal set; }
```

#### Property value

Type: [System.Int32](http://msdn2.microsoft.com/en-us/library/td2s409d)  

## See also

#### Reference

[JET\_DBINFOMISC class](hh538867\(v=exchg.10\).md)

[JET\_DBINFOMISC members](hh566148\(v=exchg.10\).md)

[Microsoft.Isam.Esent.Interop namespace](hh596136\(v=exchg.10\).md)
