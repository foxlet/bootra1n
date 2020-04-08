bootra1n: Linux + checkra1n, on USB
===================================
Just enough Linux to boot checkra1n on any PC.

You will need:
- An USB flash drive (at least 512MB or larger)
- 64-bit or 32-bit AMD or Intel PC

You do not need to install additional software or an OS.

### 1. Download bootra1n 0.10.1
- [bootra1n LiveCD (64-bit - 411 MB)](https://github.com/foxlet/bootra1n/releases/download/0.10.1/bootra1n-x86_64-0.10.1-20200408.iso)
- [bootra1n LiveCD (32-bit - 387 MB)](https://github.com/foxlet/bootra1n/releases/download/0.10.1/bootra1n-i686-0.10.1-20200408.iso)
> 64-bit: 846f3c9951a7fd27d164ca80b6d633944ce2c8d1ea3269f0f252e439191348ef   
> 32-bit: cbcb71f85843fcb8d9c21b2635b2c4d4ad56912e908f72b73bd029f021dde4fe

### 2. Write bootra1n to USB
- Rufus https://rufus.ie/

Download Rufus, press SELECT, open the ISO file, and press START to flash it to your USB drive.

### 3. Reboot and run checkra1n
Reboot your computer and enter your BIOS's boot menu.

- Select the flash drive, and it should boot into the login prompt
- Log in as `anon`, with password `voidlinux`
- At the `$` prompt, enter `sudo checkra1n`

![Prompt](https://i.imgur.com/MmqUBUJ.png)

Happy jailbreaking!

## Shutdown/Restart
Quit checkra1n and at prompt type:
- `sudo shutdown -h now` to shut down, or
- `sudo shutdown -r now` to restart.

## Troubleshooting
*Error -71:* Use the (USB Safe) option in the boot menu.  
*Error -77:* Remove your passcode before starting the jailbreak, you can set it back once done.  
*Error -78:* Exit checkra1n and double-check you entered `sudo checkra1n`  
*Secure Boot Errors:* You can disable Secure Boot in your BIOS settings.  
*USB Errors:* Try swapping cables and changing from USB 2.0 (black port) to 3.0 (blue port) and vice versa.  
*Graphics Errors:* Use the (Graphics Safe) option in the boot menu.  
*ACPI Errors:* On the boot menu, select `RAM` mode, then press TAB and add `acpi=off nomodeset` to the prompt.  

## Credits
- Checkra1n for Linux - https://checkra.in/
- Base OS - [Void Linux Team](https://voidlinux.org/)
- Project - Foxlet ([@FoxletFox](https://twitter.com/foxletfox))
- Concept - Evan ([@evanhackerman](https://twitter.com/evanhackerman))
