# Install-ROS2-on-Jatson-Nano:

## Step1: Download Xubuntu 20.04 Focal Fossa L4T R32.3.1 - Custom Image for the Jetson Nano
After downloading the file, unzip it

https://forums.developer.nvidia.com/t/xubuntu-20-04-focal-fossa-l4t-r32-3-1-custom-image-for-the-jetson-nano/121768

## Step2: Download Program to flash your SD card
https://www.balena.io/etcher/

## Step3: Extract
Command to extract the Ubuntu image in terminal

```
tar -xvjf Xubuntu-20.04-l4t-r32.3.1.tar.tbz2
```

open file balena-etcher-electron-1.7.9-linux-x64 and click the file inside

## Step4: Flash from file
choics xubuntu-20.04-l4t-r32.3.1img then click open

<img width="400" alt="Screenshot 2022-07-17 174235balenaetcher" src="https://user-images.githubusercontent.com/107959289/179404786-c676ca87-2134-403a-b33c-3c728640dcad.png">

## Step5: Select target
put the USB on the laptop and check its name on screen and select

## Step6: Flash!
put in password

## Step7: Run piece Jetson Nano B01
If you have the Jetson Nano B01, you have to add the following line in the extlinux.conf: 
``
FDT /boot/tegra210-p3448-0000-p3449-0000-b00.dtb
``
click continue on screen APP partition size

## Step8: Installing ROS 2 via debian packges
https://docs.ros.org/en/dashing/Installation/Ubuntu-Install-Debians.html
