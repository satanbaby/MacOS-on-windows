# How to Install MACOS on VirstualBox on Windows

[原文連結](https://techsviewer.com/install-macos-high-sierra-virtualbox-windows/) <br>

<a href="https://www.youtube.com/watch?v=jojB18n50dU" target="_blank">Youtube</a><br>
![](https://i1.wp.com/techsviewer.com/wp-content/uploads/2017/06/System-in-VirtualBox.jpg?w=698&ssl=1)


## Code for Virtualbox 5.x:
cd "C:\Program Files\Oracle\VirtualBox\"<br>
VBoxManage.exe modifyvm "Your VM Name" --cpuidset 00000001 000106e5 00100800 0098e3fd bfebfbff<br>
VBoxManage setextradata "Your VM Name" "VBoxInternal/Devices/efi/0/Config/DmiSystemProduct" "iMac11,3"<br>
VBoxManage setextradata "Your VM Name" "VBoxInternal/Devices/efi/0/Config/DmiSystemVersion" "1.0"<br>
VBoxManage setextradata "Your VM Name" "VBoxInternal/Devices/efi/0/Config/DmiBoardProduct" "Iloveapple"<br>
VBoxManage setextradata "Your VM Name" "VBoxInternal/Devices/smc/0/Config/DeviceKey" "ourhardworkbythesewordsguardedpleasedontsteal(c)AppleComputerInc"<br>
VBoxManage setextradata "Your VM Name" "VBoxInternal/Devices/smc/0/Config/GetKeyFromRealSMC" 1<br>

## Code for Virtualbox 4.x:
cd "C:\Program Files\Oracle\VirtualBox\"<br>
VBoxManage.exe modifyvm "Your VM Name" --cpuidset 00000001 000306a9 04100800 7fbae3ff bfebfbff<br>
VBoxManage setextradata "Your VM Name" "VBoxInternal/Devices/efi/0/Config/DmiSystemProduct" "MacBookPro11,3"<br>
VBoxManage setextradata "Your VM Name" "VBoxInternal/Devices/efi/0/Config/DmiSystemVersion" "1.0"<br>
VBoxManage setextradata "Your VM Name" "VBoxInternal/Devices/efi/0/Config/DmiBoardProduct" "Iloveapple"<br>
VBoxManage setextradata "Your VM Name" "VBoxInternal/Devices/smc/0/Config/DeviceKey" "ourhardworkbythesewordsguardedpleasedontsteal(c)AppleComputerInc"<br>
VBoxManage setextradata "Your VM Name" "VBoxInternal/Devices/smc/0/Config/GetKeyFromRealSMC" 1<br>
***
