# ATIFlash/ATI WinFlash v2.93

## ATIFLASH is used to flash the BIOS of the video card.

It supports all **AMD Radeon** graphics cards like **RX 5700, RX 5600, RX 5500.** You can also flash **BIOS** for all **AMD Radeon RX Vega, RX 580, RX 480** and all old **ATI** cards.

**ATIFlash 2.93** is not intended for **DOS** use. The latest **DOS** version can be found on the **ATIFlash** for **DOS** page

Atiwinflash has a very simple and user-friendly interface.

![ati](https://atiflash.eu/wp-content/uploads/2020/12/screenshot_3.png)

## Using the GUI in Atiwinflash

### The program must be run as administrator!

After starting the program, the panel opens

![ati](https://atiflash.eu/wp-content/uploads/2020/12/screenshot_4.png)

- The area in which you can select the video card with which you will work, as well as information about the available video cards, is highlighted in red.
- The blue arrow points to the button through which you select the BIOS you need
- The yellow arrow points to the button that is responsible for starting the firmware (after pressing the program, we will start flashing the BIOS)
- The red arrow shows the button with which you save the factory BIOS, or the one you have already installed.

## ATIFlash firmware via command line

![ati](https://atiflash.eu/wp-content/uploads/2020/12/jctyybtvmnk.jpg)

### The most useful ATIFlash commands are:

- atiflash.exe -i — will show the list of video cards installed in the AMD system. Useful for flashing the BIOS on a specific video card.
- atiflash.exe -p <video card number> <file name> — flash the video card with the specified BIOS number from the specified file.
- atiflash.exe -pa <file name> — flash to ALL video cards with the specified BIOS file.
  
### Examples of using:

- The system has a single AMD graphics card. In this case, everything is simple — we indicate the flashing of all card cards in the system using a file with a modified BIOS (let’s say it is called BIOS_mod_470.rom):
- AtiFlash.exe -pa BIOS_mod_470.rom
- The system has two different video cards — AMD Radeon R9 390 and AMD Radeon RX 470, you need to flash the BIOS only on RX 470:
- We launch the program with the -i parameter and look at the list of video cards in the system. We remember the number of the RX 470 video card.
- AtiFlash.exe -i

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
