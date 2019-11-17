#### This is a fork of LuletterSoul's XPS 9570 configuration with a few changes and updates:
* I replaced **FakeSMC** with **VirtualSMC** (solves the jumpy trackpad problem)
* Updated VoodooI2C, WhateverGreen, AppleALC and Lilu to the latest versions
* Decreased the **QuietAfterTyping** parameter of the **VoodooI2CHID** kext (the time it takes trackpad to become responsive again after typing) to 150ms
* Disabled Turbo Boost while on battery (remove **DisableTurboOnBattery.kext** if you don't want that)
* Added **VerbStub by KNNSpeed** for better working audio (no more noise in the headphones)
  * Requires additional setup – please refer to the _Post-Installation_ folder for instructions!
* Added **VoltageShift.kext** and voltageshift binary by @sicreative – please refer to the _Post-Installation_ folder for instructions on how to set it up.
* Changed the theme to clover-minimal-inverted by u/jo_ko_0 – https://i.redd.it/np7ai9qbdld21.png

#### My configuration:
* CPU: Intel i7-8750H
* GPU: UHD630 + Nvidia Gefore 1050Ti
* RAM: 16GB RAM
* Display: 4K Sharp Display
* SSD: Sabrent Rocket 1TB NVMe
* Audio: Realtek ALC298
* Touchscreen
* BIOS version: 1.11.2

#### Caveats
* NVIDIA 1050ti Graphics **doesn't work** and will probably not work in the foreseeable future. I recommend dualbooting if you plan on gaming from time to time (you won't be gaming much on macOS anyway, regardless of the video card)
* Thunderbolt 3 hotplug **works** (tested with TB16) dock with one condition: the peripheral has to be connected during the bootup. Afterwards, you can unplug and replug it all you want, but if you boot without the Thunderbolt device plugged-in and try to hotplug it afterwards, it will not work.
* Make sure to **downgrade** your bios to 1.11.2 if you have a newer version: otherwise the internal laptop display will stop working when an external display is plugged in (it will stay black even after you unplug the external display).
