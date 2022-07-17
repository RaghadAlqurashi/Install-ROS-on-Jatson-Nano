# Install-ROS2-on-Jatson-Nano
## step1: Download Xubuntu 20.04 Focal Fossa L4T R32.3.1 - Custom Image for the Jetson Nano
After downloading the file, unzip it
https://forums.developer.nvidia.com/t/xubuntu-20-04-focal-fossa-l4t-r32-3-1-custom-image-for-the-jetson-nano/121768

## step2: Download Program to flash your SD card
https://www.balena.io/etcher/

## step3: 
Command to extract the Ubuntu image in terminal
``
tar -xvjf Xubuntu-20.04-l4t-r32.3.1.tar.tbz2
``
open file balena-etcher-electron-1.7.9-linux-x64
## step4: flash from file
choics xubuntu-20.04-l4t-r32.3.1img then click open
<img width="400" alt="Screenshot 2022-07-17 174235balenaetcher" src="https://user-images.githubusercontent.com/107959289/179404786-c676ca87-2134-403a-b33c-3c728640dcad.png">

## step4: select target
If you have the Jetson Nano B01, you have to add the following line in the extlinux.conf: FDT /boot/tegra210-p3448-0000-p3449-0000-b00.dtb

## step4: flash!
