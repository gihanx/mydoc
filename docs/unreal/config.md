---
hide:
 - toc
 - path
 - title
---
## Set Default Project to DX11 instead of DX12

- Navigate to ```..\UE_5.2\Engine\Config```

- Past the Following text in the ``BaseEngine.ini``
```
[/Script/WindowsTargetPlatform.WindowsTargetSettings]
DefaultGraphicsRHI=DefaultGraphicsRHI_DX11
```

> - This file defines the default settings for core and engine-level features
> - These settings are overridden by a project's DefaultEngine.ini file and per-platform overrides
> - Some of these settings can be modified from the project settings in the editor

## Migrate Files the Easy way

- Create a Empty Folder
- Inside Create a Content Folder
- Create Text file and Rename .txt extension to .uproject
- When Migrating select Content Folder

Yay now you just need a folder.

> When migrating Unreal checks for **Content** folder and **.uproject** file

## Quick Commands to Disable On-Screen Warning

``DisableAllScreenMessages`` <br>
``EnableAllScreenMessages``

