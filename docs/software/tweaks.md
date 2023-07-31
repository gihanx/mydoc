---
hide:
 - toc
 - path
 - title
---

## Activate Windows
Microsoft Activation Scripts [**Link**](https://github.com/massgravel/microsoft-activation-scripts)
- Use HWID to get a key tied to motherboad permenently

---

## BIOS/WINDOWS Oprimization Guide
- [Boring Boredom](https://github.com/boringboredom/pc-optimization-hub)
- [Overclock Site Guide](https://www.overclock.net/threads/gaming-and-mouse-response-bios-optimization-guide-for-modern-pc-hardware.1433882/)
- [Melody's Tweak](https://sites.google.com/view/melodystweaks/basictweaks#h.7fhhmr5naoq0)
- [FR33THY](https://www.youtube.com/@fr33thy)
- [Blur Busters](https://forums.blurbusters.com/index.php?sid=739f751405ce888661893b74bedbdbed)
- [Calypto’s Latency Guide](https://docs.google.com/document/d/1c2-lUJq74wuYK1WrA_bIvgb89dUN0sj8-hO3vqmrau4/edit)

---
Better Mic Setup w/ EqAPO + VST Plugins [Link](https://www.youtube.com/watch?v=fnk0au1rt1i)

---
Install Chipset Drivers [Snappy Driver Installer Origin](https://www.snappy-driver-installer.org/)
> Only install if necessary 

Uninstall GPU Drivers [DDU](https://www.guru3d.com/files-details/display-driver-uninstaller-download.html)
> Don't Update, Fresh install gpu drivers

Set Custom Resolution/Hz [CRU](https://www.monitortests.com/forum/thread-custom-resolution-utility-cru)

Force Timer Resolution to 0.5 [ISLC](https://www.wagnardsoft.com/forums/viewtopic.php?t=3775)

Disable Hibernate [Link](https://docs.microsoft.com/en-us/troubleshoot/windows-client/deployment/disable-and-re-enable-hibernation)

Show Seconds in System Clock [RegFile](https://www.howtogeek.com/wp-content/uploads/2017/09/show-seconds-in-system-clock-hacks.zip)

Windows Shortcut Dir [Guide](https://superuser.com/questions/217504/is-there-a-list-of-windows-special-directories-shortcuts-like-temp)

Monitor Hz Changer Task [Guide](https://gaming.stackexchange.com/questions/148651/how-can-i-set-the-resolution-and-refresh-rate-when-the-game-starts)

---

## AMD Sharpen - Registry method

1. In RegEdit Navigate to `\HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\Class\{4d36e968-e325-11ce-bfc1-08002be10318}\0000`

2. Create `KMD_USUEnable` 

3. Set the value to "1"

4. Restart the driver using the CRU or restart the PC.

---
## Benchmark
[HWiNFO](https://www.hwinfo.com/download/)

[GPUZ](https://www.techpowerup.com/gpuz/)

GPU Tuner [MSI AfterBurner](https://www.msi.com/Landing/afterburner/graphics-cards)
> Just use Stable Version

Check System Software Larency [Latency Monitor](https://www.resplendence.com/latencymon)

Check mouse Polling Rate [Mousetester v1.5.3](https://www.overclock.net/threads/mousetester-software-reloaded.1590569/)

---
## Disable/Enable Windows Services

Registry location ``HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Services\``

> 0 = Boot <br>
1 = System <br>
2 = Automatic <br>
3 = Manual <br>
4 = Disable <br>

## Remove Windows CTRL+ALT+DELETE logon restrection

![](./assets/lpg.png)