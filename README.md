# cp65s_hackintosh_efi_driver
## Description:
It is a hackintosh efi driver for cp65s, the model is CLEVO P655SA.
It fits for macOS Mojave 10.14.x .
## So which laptop can eat this apple? (Fits my driver)
The cp65s LapTop computer is made in China on September , 2015.

In China, its name is Shenzhou z7m i78172d1.

For i78172d1, 'i7' means that its CPU is Intel Core i7-4720HQ @2.7GHz four cores, 
'8' means it uses 8GB 1600MHz DDR3L RAM, '172' means it uses a 7200 Speeds ROM.
'd1' is the second generation, because it may have a test model which is named by d0.

The LapTop is used by Nvidia GTX965m, but hackintosh can not drive it.

And its core GPU is Intel Graphics HD 4600. The two GPU use a 2048MB GRAM together.
### So if your Computer is the same as my core GPU, it may help you eat it.
### The other thing you should know is that its model is used by a 15.3 screen (SAMSUNG SDC4852). This tip is also necessary.
Sound Card is Realtek ALC892, the LAN is RL81xx, and the WAN is RL8723RE(it can not be used, you can buy a USB WAN or equip a new WAN to hack it)
## how to drive it?
First, using a driver named as 'CLOVER' to hack the apple.

Second, these kext driver are equipped.  
* [Lilu](https://github.com/acidanthera/Lilu)
* [WhateverGreen](https://github.com/acidanthera/WhateverGreen)
* [VirtualSMC](https://github.com/acidanthera/VirtualSMC)
* [USBInjectAll]()
* [AppleALC](https://github.com/acidanthera/AppleALC)
* [ACPIBatteryManager]()
* [VoodooPS2Controller]()

Third, directly inject intel for 0x04160000 to drive it, but it only has 1024MB GRAM.

If try other platfrom id, all have problems for its SUMSANG screen.(May not to control screen light because it drives the out screen, may start computer having 8 apples)

For this [forum](http://bbs.pcbeta.com/viewthread-1803809-1-1.html), i find a way to solve it, just directly inject id, put 2048MB patch, and change the CLOVER resolution.

But for this way, also have some glistening. Maybe i will try to update it.
