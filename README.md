bootra1n: Linux + checkra1n, on USB
===================================
Just enough Linux to boot checkra1n on any PC.

You will need:
- An USB flash drive (at least 512MB or larger)
- 64-bit or 32-bit AMD or Intel PC

You do not need to install additional software or an OS.

### 1. Download bootra1n
- [bootra1n LiveCD (64-bit - 422 MB)](https://github.com/foxlet/bootra1n/releases/download/0.9.8.1/bootra1n-x86_64-0.9.8.1-20200304.iso)
- [bootra1n LiveCD (32-bit - 365 MB)](https://github.com/foxlet/bootra1n/releases/download/0.9.8b/bootra1n-i686-0.9.8-20200206.zip)
> 64-bit: 2ce01d97bc4e45def8a80ff9a64bc172f9c821bcef7a923fa600f4f2113c4f11   
> 32-bit: 74186eaf60a54d5ec986c5d9529f18b7901c953397e0fd85edb8466b7dc2378e

Unzip bootra1n into any directory, it should contain an ISO file.

### 2. Write bootra1n to USB
- Etcher https://www.balena.io/etcher/

Download Etcher, select the ISO file, flash it to your USB drive.

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
*Error -77:* Remove your passcode before starting the jailbreak, you can set it back once done.  
*Error -78:* Exit checkra1n and double-check you entered `sudo checkra1n`  
*Secure Boot Errors:* You can disable Secure Boot in your BIOS settings.  
*USB Errors:* Try swapping cables and changing from USB 2.0 (black port) to 3.0 (blue port) and vice versa.  
*ACPI Errors:* On the boot menu, select `RAM` mode, then press TAB and add `acpi=off nomodeset` to the prompt.  

## Credits
- Checkra1n for Linux - https://checkra.in/
- Base OS - [Void Linux Team](https://voidlinux.org/)
- Project - Foxlet ([@FoxletFox](https://twitter.com/foxletfox))
- Concept - Evan ([@evanhackerman](https://twitter.com/evanhackerman))
