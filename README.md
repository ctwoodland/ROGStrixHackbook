# ASUS ROG Strix G712L HackbookPro
My files for booting macOS Big Sur on the ASUS ROG Strix G712L laptop.

## DISCLAIMER:
> macOS is a proprietary operating system provided by Apple for use on their devices. macOS must be obtained *legally* from your own Apple device. Any other method of obtaining macOS is considered **piracy** and is *illegal*.

## Using this EFI
Please read through the [OpenCore Install Guide](https://dortania.github.io/OpenCore-Install-Guide/) in its entirety to gain an understanding of the process should something go wrong.
If your system is a G712L, you should be able to replace your own EFI folder with this one. It does not matter which variant of the G712L; since macOS does not currently support the different nVIDIA cards these laptops come with, they are disabled in favor of the integrated Intel UHD Graphics.

I have scrubbed my own SMBIOS information from the `config.plist` - please refer to the OpenCore guide to fill in this information.

If your system is *not* a G712L, I would **highly recommend** following the OpenCore guide step-by-step, only referencing my EFI folder for troubleshooting purposes (eg. if your system is similar in hardware specs and you can't get a certain component to work).

## ROG Aura Lights
This laptop uses LED strips around the base, which also integrate to serve as the keyboard backlight.
I have not had success yet in getting the macOS native keyboard brightness setting to control these lights.
Thankfully, *black.dragon74* has ported Will Roberts' `rogauracore` program for Linux over to macOS as `macRogAuraCore`.
You can find it [on his Github repo](https://github.com/black-dragon74/macRogAuraCore).

## Credits
* [OpenCore bootloader](https://github.com/acidanthera/OpenCorePkg)
* [Sn1mpuls3](https://www.reddit.com/u/Sn1mpuls3) on Reddit for [his EFI folder](https://www.reddit.com/r/hackintosh/comments/ifwchh/asus_rog_strix_g712lu_it_works_flawlessly_just/)
* Lâm Tùng for [his EFI folder](https://github.com/tunglamvghy/AsusROG-G712LW-hackintosh)
* black.dragon74 aka Nick for [macRogAuraCore](https://github.com/black-dragon74/macRogAuraCore)
* Will Roberts for the original [rogauracore](https://github.com/wroberts/rogauracore) for Linux
