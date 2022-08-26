# THIS README IS UNDER HEAVY DEVELOPMENT. Do not use it until its done!

# CH341A-drivers-software-and-documentation

Mirror to the official CH341A drivers and used software, along with the documentation.

## I. Requirements

1. The PC you want to modify. 
    (Make Sure To check if the bios chip is 8-pin 24XXX or 25XXX series before doing anything!!!!)
    
2. A second PC, to be able to flash the firmware from it to the the pc's bios chip you want to modify.
       
    Supported OS 
    
- Windows 7 SP1   and up (need to run as Admin)
- Android 3.x     and up (no root access needed)
- Linux   2.6.25  and up (root access required)
- MacOSX  10.12.x and up (root access required)

----------------------------------------------------------------------

NOTE: Linux and BSD systems (Android, MacOS, iOS, Ubuntu, ChromeOS etc) are sometimes called "UNIX-like" operating systems.


3. The CH341A programmer

4. A SOIC8 SOP-8 Test Clip for 24XXX / 25XXX series
    
    (No soldering/desoldering support for this article)    
    (That clip is recommanded because it replaces this process, therefore, it is safe)

5. Be careful and patient when you work with the CH341A !


## II. CH341A 101 briefly - The Basics

Complete ALL the steps below to make sure you understand how to use CH341A

[1. Read The Basic Information and Schema of CH341A (~5 minutes read)][basic_info]

[2. Learn the Basics of CH341A (10 minutes video)][basic_tutorial]

[3. How to flash BIOS with CH341A on Windows/Linux/MacOS with ASProgrammer or flashrom (9 minutes video)][flashing_tutorial]

## III. Setting up the environment

### A. Downloading the tools

|                     |                                                                     Windows                                                                    |         Android         |                                  Linux (kernel version)                                  |                                        MacOS X                                       |        FreeBSD        |       OpenBSD      |    DragonFlyBSD    |       NetBSD       |
|:-------------------:|:----------------------------------------------------------------------------------------------------------------------------------------------:|:-----------------------:|:----------------------------------------------------------------------------------------:|:------------------------------------------------------------------------------------:|:---------------------:|:------------------:|:------------------:|:------------------:|
|      CH341ASER      |                                                            [Download][drv_windows1]                                                            | [Download][drv_android] | [Download (2.6.25 - 3.13.x)][drv_linux_old]<br>[Download (3.14.x and up)][drv_linux_new] | [Download (10.9-10.15)][drv_macosx_old]<br>[Download (10.16 and up)][drv_macosx_new] |     Pre-Installed     |    Pre-Installed   |    Pre-Installed   |    Pre-Installed   |
|      CH341APAR      |                                                            [Download][drv_windows2]                                                            |   Included in package   |                                        Not Needed                                        |                                      Not needed                                      |       Not needed      |     Not needed     |     Not needed     |     Not needed     |
| Programmer Software | [AS Programmer][ASProgrammer]<br>[Neo Programmer][NeoProgrammer]<br>[Siberia Programmer][SiberiaProg]<br>[CH341A Programmer][CH341AProgrammer] |   Included in package   |                        [Download FlashROM Script][FlashRomScript]                        |                      [Download FlashROM Script][FlashRomScript]                      | `pkg_add -r flashrom` | `pkg_add flashrom` | `pkg_add flashrom` | `pkg_add flashrom` |

### B. Installing the tools

Disconnect the CH341A programmer if you plugged it into your PC before installing the software.

#### Windows

GIF here

```
commands here
```

#### Linux, MacOS X, FreeBSD, OpenBSD and DragonflyBSD

GIF here

```
commands here
```

#### Android

GIF here

```
commands here
```


## IV. Gathering information about that BIOS/UEFI firmware

### A. Backing up BIOS information



### B. Dumping the FULL BIOS Image 


## V. Danger zone (well, not actually, but still :) )

### A. Editing the BIOS/UEFI

There are various ways to edit one's BIOS/UEFI firmware.
I will put a list of tools here to help you get started, but you will have to play with them, for now.

[UEFI-BIOS-MODDING-TOOLS][]

### B. Flashing the BIOS/UEFI

#### With ASProgrammer

GIF here

#### With NeoProgrammer

GIF here

#### With SiberiaProg

GIF here

#### With CH341A Programmer

#### With FlashROM

## Final thoughts

I have eye fatigue.

[basic_info]: https://www.onetransistor.eu/2017/08/ch341a-mini-programmer-schematic.html "Click me!"
[basic_tutorial]: https://www.youtube.com/watch?v=4qX2zihB6UE "Click meeee!"
[flashing_tutorial]: https://www.youtube.com/watch?v=r8f-3syiFSc "Click Me please :D"

[drv_windows1]: http://wch-ic.com/downloads/CH341SER_EXE.html
[drv_windows2]: http://wch-ic.com/downloads/CH341PAR_EXE.html
[drv_linux_old]: http://wch-ic.com/downloads/CH341SER_LINUX_ZIP.html
[drv_linux_new]: https://github.com/frank-zago/ch341-i2c-spi-gpio/archive/refs/heads/master.zip
[drv_macosx_old]: http://wch-ic.com/downloads/CH34XSER_MAC_ZIP.html
[drv_macosx_new]: http://wch-ic.com/downloads/CH341SER_MAC_ZIP.html
[drv_android]: http://wch-ic.com/downloads/CH341SER_ANDROID_ZIP.html
[ASProgrammer]: https://github.com/nofeletru/UsbAsp-flash/releases
[CH341AProgrammer]: https://receiverpro.net/dl/ch341a-programmer-v1-44-31-01-2022/
[NeoProgrammer]: https://receiverpro.net/dl/neoprogrammer-v2-2-0-10_15102021/
[SiberiaProg]: https://receiverpro.net/dl/siberiaprog-ch341a-new-update-v1-45-04-02-2022/
[FlashRomScript]: ./flashrom_installer.sh

[uefi_bios_modding_tools]: ./tools/

[gif_windows_install_ch341a]: 
[gif_unix_install_ch341a]: 
[gif_android_install_ch341a]: 

[gif_clamp_on_ch341a]: 
[gif_clamp_to_1st_pc]: 
[gif_ch341a_usb_to_2nd_pc]: 

[gif_asprogrammer_biosdump]: 
[gif_neoprogrammer_biosdump]: 
[gif_siberiaprog_biosdump]: 
[gif_ch341aprogrammer_biosdump]: 
[gif_flashrom_biosdump]: 

[gif_asprogrammer_biosflash]: 
[gif_neoprogrammer_biosflash]: 
[gif_siberiaprog_biosflash]: 
[gif_ch341aprogrammer_biosflash]: 
[gif_flashrom_biosflash]: 


