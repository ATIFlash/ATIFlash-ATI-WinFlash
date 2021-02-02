# ATIFlash/ATI WinFlash v2.93


### Important: You need to disable SecureBoot / Activate CSM in your
### Motherboard UEFI because the modification will make
### the cryptographic signature invalid.

0/58. If your AV warns you about a virus/trojan, consider it as false positive.

Fork from lojkinKot

works on linux with mono, executable is build against .net 3.5

one click timing feature should be used with care, it maybe not stable for you

please build the executable yourself or decompile the existing one if you don't trust
### v2.93
- Added support for BIOS Navi Radeon RX 5700 Series firmware.
### v2.84
- Fixed issue with launching Build 1803 on Windows 10.
### v2.77
- Added support for Radeon RX Vega series cards.
### v2.71
- Added support for AMD Fiji.
### v2.0.1.18
- Fixed a bug that made it impossible to read a BIOS file with a two-character extension in the name.
Added support for a number of ROM chips.
- Fixed checksum error when flashing boards with ISR already enabled.
- Fixed issues when flashing cards based on GPU Pitcarin.

### v2.0.1.14
- Added function to save ISR data after flashing.
- Added command line parameter caymandualrom = true / false.
- Improved support for new video cards based on the Cayman chip (including the Radeon HD 6990).

### v2.0.1.13
- Added support for Radeon HD 6850 / HD 6870 (Barts) and Radeon HD 6950 / HD 6970 (Cayman).
- Bug fixed — the last 2 digits of the new P / N format of HD 6850 and HD 6870 video cards (Barts) were not displayed.

Contribution from Sebohe:

### Build Dependencies

Ubuntu 16.04.2:

```
sudo apt-get install mono-complete
```

### Building

```
sh build.sh
```

### Executing

Just change your working directory to the ATIFlash/ATI WinFlash and execute:

```
./run.sh
```
