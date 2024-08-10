# Ryzentosh Lenovo Ideapad gaming 3 (15ach6) EFI

## What works and what doesn't

Working: Camera, brightness, speakers, mic, ethernet, power managment

Broken: WLAN, Bluetooth, dGPU




## What's required?
- Lenovo ideapad gaming 3 - With AMD Ryzen 5600H (others may work)
- Mac / Hackintosh // You can use Windows / Linux PC to create a web installer
- Atleast 16 GB USB stick
- A lot of time and patience
- Ethernet cable or Android phone with internet over USB.
- macOS BigSur, Monterey, Ventura, Sonoma or 15 BETA installer
- A brain
## Help

 - [OpenCore guide](https://dortania.github.io/OpenCore-Install-Guide/)
 - [How to create macOS installer - Apple](https://support.apple.com/en-us/101578)
 - [macOS installers download](https://support.apple.com/en-us/102662)


## Installation
1. Create macOS installer using 'createinstallmedia'
2. Open terminal and type "diskutil list" find your USB that installer has been copied to.
3. Type "sudo disktutil mount diskXsX" replace diskXsX with your USB ID for ex. disk2s1
4. Copy whole EFI folder you can download it [here](https://github.com/Mihot7/lenovo-ideapad-gaming-3-15ach6-open-core/releases/download/1.0/EFI.zip) onto EFI partiton of the USB DRIVE NOT YOUR PC's
5. Eject usb plug it into your laptop
6. Enter BIOS and:
- disable: secure boot, dedicated GPU
- Change integrated graphics memory to 2GB
- Set USB drive as first boot device
7. Reboot your pc with usb inserted
8. Boot macOS installer
9. Wipe your hardrive with drive utility
10. Install macOS
Note: after 2nd part of the installer 1st boot may take 30 minutes+ so be patient!

11. Configure macOS
12. Download the EFI again
13. Open termial and type: "sudo diskutil mount disk0s1"
14. Copy EFI folder onto EFI partiton OF YOUR COMPUTER NOT YOUR USB DRIVE
15. Download VooDooHDA  [here](https://github.com/CloverHackyColor/VoodooHDA) and follow the instructions there.
16. Use Open Core tutorial above to generate a SMBIOS
17. DONE
