---
Description: HKLM\\Software\\Microsoft\\Internet Explorer\\Extensions\\{e2e2dd38-d088-4134-82b7-f2ba38496583}.
ms.assetid: a0d9e959-d8fd-4546-9529-1dc42fa0bdd6
title: Exec
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# Exec

**HKLM\\Software\\Microsoft\\Internet Explorer\\Extensions\\{e2e2dd38-d088-4134-82b7-f2ba38496583}**



| Data type | Range                    | Default value |
|-----------|--------------------------|---------------|
| REG\_SZ   | *Path to the executable* |               |



 

## Browser Integration Steps

1.  Use the [**RegOpenKeyEx**](https://msdn.microsoft.com/windows/desktop/c8a590f2-3249-437f-a320-c7443d42b792) function to determine whether the Network Diagnostic is installed. If it is installed, the **{e2e2dd38-d088-4134-82b7-f2ba38496583}** key is present.
2.  Use the [**RegQueryValueEx**](https://msdn.microsoft.com/windows/desktop/202d253a-10ff-40e7-8eec-a49717443b81) function to retrieve the path of the Network Diagnostic executable file from the **Exec** entry.
3.  Display the new error page if the diagnostic is installed on the system.
4.  Create a browser extension that creates a standard toolbar item if the diagnostic is installed on the system.
5.  Execute the Network Diagnostic executable using the path retrieved in step 2.

## Related topics

<dl> <dt>

[Network Diagnostics Tools Feature Overview](Http://go.microsoft.com/fwlink/p/?linkid=85313)
</dt> </dl>

 

 


