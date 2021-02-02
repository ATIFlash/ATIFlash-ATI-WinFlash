# ATIFlash/ATI WinFlash v2.93


If you don't trust the EXE just build on Linux with ```sh build.sh```. Quick and easy.

### Important: You need to disable SecureBoot / Activate CSM in your
### Motherboard UEFI because the modification will make
### the cryptographic signature invalid.

VirusTotal Report: https://www.virustotal.com/gui/file/baeba7089443f2341b83fe00302bfd6dcdf3a83b452fa3f085bc76c84162fea1/detection

0/58. If your AV warns you about a virus/trojan, consider it as false positive.

Fork from lojkinKot

works on linux with mono, executable is build against .net 3.5

one click timing feature should be used with care, it maybe not stable for you

please build the executable yourself or decompile the existing one if you don't trust
### v2.93
- Added UberMix 3.3
- Few small changes in code
### v2.84
- Fixed bug no supported memory found (K4G80325FC)
- Old version bump in properties
### v2.77
- Added support for memory Samsung K4G80325FC
- Added new device AMD Radeon RX 580 2048SP - 6FDF
### v2.71
- Fixed apply timings for Hynix memory
- Added support for RX590
- Added support for New Hynix memory H5GC8H24AJ
- Added timing for New Hynix H5GC8H24AJ

### v2.0.1.18
- Updated Elpida Timing

### v2.0.1.14
- Added New timing for Hynix.
- Added option for choosing timings on hynix Between Universal Hynix timing and Good hynix timing.
- Universal Hynix timing work on: H5GC8H24MJ, H5GQ8H24MJ, H5GQ4H24AJ.

### v2.0.1.13
- Fixed UI (updated design)
- Fixed and Updated all Timing's
- Added New strap for Micron and Hynix
- Added option for choosing timings on samsung between uber-mix 3.1 and 3.2, and on Micron between Good Micron timing and S Micron timing.
- Added Icon
- Added option for max. Mem. freq. (after one click timing patch button click automatically change max. mem. to 2300 MHz)

Contribution from Sebohe:

### Build Dependencies

Ubuntu 16.04.2:

```
sudo apt-get install mono-complete
```

Arch Linux:

```
yaourt -Sy mono48
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
