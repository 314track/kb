---
title: "windows"
draft: false
---
# windows

some windows stuff


## win11-context-menu

Change Windows11 context menu to default Windows10 context menu

```bash
reg.exe add "HKCU\Software\Classes\CLSID\{86ca1aa0-34aa-4e8b-a509-50c905bae2a2}\InprocServer32" /f /ve
```