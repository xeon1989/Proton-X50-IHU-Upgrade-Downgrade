# Flash your Proton X50 IHU to ATLAS version 617v1 / 618v1 #

## Before You Start ##
- Flashing firmware comes with risk. Proceed with caution and exercise due diligence.
- No warranty from me. If you broke your IHU, you will need to find your way out.
- One of the fellow bro feedback that this works for Firmware version ends with 0644. 

## Should You Flash 617v1 / 618v1 Firmware? ##
- If your IHU is running on GKUI19, its performance and functionality are good enough. There is no need to upgrade to ATLAS unless you prefer the modern UI.
- If your IHU running on ATLAS stucked on version 581/582 and you wanted to install your own apps, Yes.
- If your IHU updated to version 617 / 618 after 2-Mar-2023 and you wanted to install your own apps, Yes.

## Prerequisites ##
- (!IMPORTANT!) IHU with *Hardware version 0090 or 0200*, Firmware version GKUI H379 / L380, ATLAS H581 / L582/H617(ver2) / L618(Ver2).
- **USB 2.0 drive** formatted with FAT32 file system. (credit to @nnyj for reminding me)
- A device to download and copy files to USB drive.
- (optional) A cup of coffee to stay alert. 

## Steps to flash firmware ##
1. Download firmware file based on your X50 model. Make sure you download the correct firmware. DO NOT flash Flagship firmware in Executive variant or vice versa. 

| Model              | Current Firmware           | Download |
|--------------------|----------------------------|----------|
| Standard<br />Executive | GKUI: SW0SXRA1201L5064.00380 <br />ATLAS: SW0SXRA0616L5170.00582 <br />ATLAS: SW0SXRA1124L5170.00618(v2) <br />ATLAS: SW0SXRA0413L5170.00645 | [Proton X50 Standard Executive.7z](https://drive.google.com/file/d/1hvU93XhB6K1q-e_x1XrCwucJmJDQLqzF/view?usp=share_link)   |
| Premium<br />Flagship   | GKUI: SW0SXRA1201H5064.00379 <br />ATLAS: SW0SXRA0616H5170.00581 <br />ATLAS: SW0SXRA1124H5170.00617(v2) <br />ATLAS: SW0SXRA0413H5170.00644 | [Proton X50 Premium Flagship.7z](https://drive.google.com/file/d/11VgpWI4qZRpvMWI9ogBGUnhvKK3S88go/view?usp=share_link)   |


2. Once downloaded, unzip the file. Make sure SW0SXRA1124xxxx.zip file not corrupted by comparing checksum of your file with following hash. ([follow this guide](https://howardsimpson.blogspot.com/2022/01/quickly-create-checksum-in-windows.html) if you don't know how) 

![image](https://user-images.githubusercontent.com/17538895/232070563-37d87a31-5f3b-4c87-8498-8539b0123707.png)

![image](https://user-images.githubusercontent.com/17538895/232070741-8e56855e-36a0-4009-abb3-9507e45c89fc.png)

3. Place unzipped files in your USB drive. Tip: You may place [Apps installation Script](https://github.com/xeon1989/Proton-X50-APK-Installer-ATLAS) on the same USB so that the installation takes place right after Firmware is flashed. 
4. Start the car engine and plug in the USB drive.
5. Go to Settings > Vehicle > System > About. For Flagship/Premium, long tap on the "System Settings" icon. For Standard/Exec, long tap on "Mac address". (I'm not certain about Std/Exec variant, let me know if long tap "MAC address" not working)
6. Keyboard now pops up. Enter engineering mode code. ([Code mentioned in this LYN post](https://forum.lowyat.net/index.php?showtopic=4997599&view=findpost&p=106358874); I can't post the code here 😥 )
7. Tap "SOC升级". If everything works, you should see a similar screen as below.
  
  ![image](https://user-images.githubusercontent.com/17538895/231667654-104b03aa-1b35-4aaa-8307-b939205f6a76.png)
  
  ![image](https://user-images.githubusercontent.com/17538895/231677754-d8075407-4130-4236-b1c3-21ac3dd3aed6.png)
  
8. Tap "确定" to start te verification. 
  
  ![image](https://user-images.githubusercontent.com/17538895/231677926-2c75366f-52f9-4938-a58a-79d4ac74ce95.png)

  ![image](https://user-images.githubusercontent.com/17538895/231667748-b3181a3c-7442-4e15-95ce-db3b259c11b0.png)
  
9. Once verification done, tap 升级 to proceed with upgrade and reboot.
  
  ![image](https://user-images.githubusercontent.com/17538895/231679709-4212f199-98b8-4ee9-9378-c4a64acedd10.png)
  
10. Once rebooted, it should be upgraded to 617v1 / 618v1. If you have an installation script on your USB drive, your apps will be installed automatically. 
