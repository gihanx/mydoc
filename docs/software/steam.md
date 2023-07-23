---
hide:
 - toc
 - path
 - title
---
## Steam Client

Bloatless Client [Steam CMD](https://developer.valvesoftware.com/wiki/SteamCMD)

No Mobile Phone needed to use Marketplace [Steam Desktop Authenticator](https://github.com/jessecar96/steamdesktopauthenticator)

---
## Steam Launch Arguments 
- Run it as a bat from steam dir<br>
- Disable Steam Chromium Backend and some stuff 
  > as of 2023 this will not work, but there is a way, i will update soon

```
start steam.exe -dev -console -nofriendsui -no-dwrite -nointro -nobigpicture -nofasthtml -nocrashmonitor -noshaders -no-shared-textures -disablehighdpi -cef-single-process -cef-in-process-gpu -single_core -cef-disable-d3d11 -cef-disable-sandbox -disable-winh264 -cef-force-32bit -no-cef-sandbox -vrdisable -cef-disable-breakpad +open steam://open/minigameslist 
```

---

## Launch Options for Steam Games

Disable Vsync
```
-NoVSync
```
Disable Splash Screen
```
 -NOSPLASH 
```
Force to use all cores
```
-USEALLAVAILABLECORES
```
Memory Allocation Tweak
```
-malloc=system 
```
Disables Antialias
```
+mat_antialias 0
```
Disables Eye Candy
```
-NOMANSKY
```
Disable PUBG Ragdoll
```
-KoreanRating
```
---

## Steam Unlocker
[Koalageddon2](https://github.com/acidicoala/Koalageddon2)