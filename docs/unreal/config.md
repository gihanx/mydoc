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

> When migrating Unreal checks for **Content** folder and **.uproject** file

## Allocate More threads to compile shaders

in BaseEngine.ini  set NumUnusedShaderCompilingThreads to 0

also WorkerProcessPriority is something to look at, set it to 1

https://store.algosyntax.com/tutorials/unreal-engine/ue5-how-to-speed-up-compiling-shaders/

## Movie Render Queue FFMPEG Setup

[/Script/MovieRenderPipelineCore.MoviePipelineCommandLineEncoderSettings]
ExecutablePath=C:\Program Files\ffmpeg-master-latest-win64-gpl\bin\ffmpeg.exe
VideoCodec=libx264
AudioCodec=aac
OutputFileExtension=mp4


## Stats Details
![x](../assets/UE_Stats.png)

## Change DDC Cache Location

Edit BaseEngine.ini *C:\Program Files\Epic Games\UE_5.2\Engine\Config\BaseEngine.ini*

[InstalledDerivedDataBackendGraph]

Change Default Path *Path="%ENGINEVERSIONAGNOSTICUSERDIR%DerivedDataCache"

To save within project *Path=“%GAMEDIR%LocalDerivedDataCache”

or your own location *Path=D:\UE_DDC*

