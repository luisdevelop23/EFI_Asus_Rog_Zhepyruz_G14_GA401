
# Hackintosh - Asus Rog Zhepiruz G14 (GA401)

This Efi is compatible with macos sonoma, (maybe there are internet connection problems), it already has the product name, kexts necessary for the specified model






# Indications
Step 1:
## Configuration

|Component      | Model GA401 2020  |
|:--------------|:------------------|
|CPU            | AMD Ryzen 7 4800hs|
|GPU - D/I      | AMD Vega 8 / Gtx 1650|
|Network/Bluetooth| Intel AX200 (I had an MT7921 which I changed for Intel)|
|SDD | INTEL SDDPEKNU512GZ|
|Keyboard/Trackpad	| ISO HID|


## Indications

- use the OCAuxiliaryTools tool,change the information on your system, in the sections SystemUUID, SystemSerialNumber, ROM

- Create two partitions, one with a volume greater than 80gb recommended and name it macos, and another with 230mb, the latter we will use as boot so name it boot in FAT32

- install the EFI, separate the after-config folder, with a USB or external drive format it to FAT32, place the EFI file there.

- Turn off the computer, when you turn it on press F2, go to advanced options, and disable boot-security, and fast-boot, then press F8 and select your EFI drive

- When starting the USB, select the option name_of_your_USB.dmg, then the macOS recovery mode will open.

- When in recovery mode, connect your laptop to the internet, select disk utilities, in the left section your disk or partition where you want to install macOS will appear

- When you select your disk/partition, go to the top and select Erase, then format the drive to APFS, after formatting is complete close disk utilities

- Then select install macos sonoma, give everything okay and wait for it to finish

- When it finishes, the laptop will most likely restart, and you will return to the boot where a new option called macOS Install will appear, select Windows.

- Once we are in Windows we will go to our EFI, we will update the config and oldconfig, with the files in after-config, this will be our new EFI, and also our new boot, after doing this we will turn off the laptop.

- When you turn it on, you will return to the BIOS and this time place the boot partition as the first boot. We do this so that after installing macOS you will not have to use the USB again to enter the macOS system.

- After doing that we will start the boot process, install macOS in the new option, and configure our new Mac. You can see the latter in any YouTube tutorial.


## Thans to

the people who helped me complete my efi

- Pluto (https://github.com/PIut02) , for the kexts and other files
- oceanthedev (https://github.com/oceanthedev) for the advice and help to get here
- Apple for the very beautiful system

