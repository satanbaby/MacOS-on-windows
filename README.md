# How to Install MACOS on VirstualBox on Windows

1.https://i1.wp.com/techsviewer.com/wp-content/uploads/2017/06/Extract-Virtual-Machine-Image-for-VirtualBox.jpg?resize=810%2C621&ssl=1
2.https://i2.wp.com/techsviewer.com/wp-content/uploads/2017/06/Create-new-virtual-machine.jpg?resize=810%2C429&ssl=1
3.https://i1.wp.com/techsviewer.com/wp-content/uploads/2017/06/Add-macOS-High-Sierra-Disk-to-VirtualBox.jpg?resize=810%2C429&ssl=1
4.https://i1.wp.com/techsviewer.com/wp-content/uploads/2017/06/System-in-VirtualBox.jpg?w=698&ssl=1
5.https://i0.wp.com/techsviewer.com/wp-content/uploads/2017/06/Run-Command-Prompt.jpg?w=699&ssl=1
6.https://i1.wp.com/techsviewer.com/wp-content/uploads/2017/06/Add-Code-to-CMD.jpg?resize=810%2C471&ssl=1

## Code for Virtualbox 5.x:
cd "C:\Program Files\Oracle\VirtualBox\"
VBoxManage.exe modifyvm "Your VM Name" --cpuidset 00000001 000106e5 00100800 0098e3fd bfebfbff
VBoxManage setextradata "Your VM Name" "VBoxInternal/Devices/efi/0/Config/DmiSystemProduct" "iMac11,3"
VBoxManage setextradata "Your VM Name" "VBoxInternal/Devices/efi/0/Config/DmiSystemVersion" "1.0"
VBoxManage setextradata "Your VM Name" "VBoxInternal/Devices/efi/0/Config/DmiBoardProduct" "Iloveapple"
VBoxManage setextradata "Your VM Name" "VBoxInternal/Devices/smc/0/Config/DeviceKey" "ourhardworkbythesewordsguardedpleasedontsteal(c)AppleComputerInc"
VBoxManage setextradata "Your VM Name" "VBoxInternal/Devices/smc/0/Config/GetKeyFromRealSMC" 1

## Code for Virtualbox 4.x:
cd "C:\Program Files\Oracle\VirtualBox\"
VBoxManage.exe modifyvm "Your VM Name" --cpuidset 00000001 000306a9 04100800 7fbae3ff bfebfbff
VBoxManage setextradata "Your VM Name" "VBoxInternal/Devices/efi/0/Config/DmiSystemProduct" "MacBookPro11,3"
VBoxManage setextradata "Your VM Name" "VBoxInternal/Devices/efi/0/Config/DmiSystemVersion" "1.0"
VBoxManage setextradata "Your VM Name" "VBoxInternal/Devices/efi/0/Config/DmiBoardProduct" "Iloveapple"
VBoxManage setextradata "Your VM Name" "VBoxInternal/Devices/smc/0/Config/DeviceKey" "ourhardworkbythesewordsguardedpleasedontsteal(c)AppleComputerInc"
VBoxManage setextradata "Your VM Name" "VBoxInternal/Devices/smc/0/Config/GetKeyFromRealSMC" 1
