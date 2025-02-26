# Follow instructions below to get HHD working on Cachyos Handheld
+ Open Kernel Manager and select configure kernel
+ Select RC kernel from top drop down and check the options you see here

![Screenshot_20250226_112611](https://github.com/user-attachments/assets/ef50d1f4-6259-4faa-b310-aa5d57de4580)

+ Click compile kernel
+ Once option menu open up go here press Enter
  
![Screenshot_20250226_112713](https://github.com/user-attachments/assets/d52489a5-8675-4227-8f0a-adadf5877ea1)

+ Scroll down till you see this then press enter again.
  
![Screenshot_20250226_112740](https://github.com/user-attachments/assets/026b3ef4-b797-442d-82e4-d19dff7153f4)

+ Scroll down to This option and enter again.

![Screenshot_20250226_112755](https://github.com/user-attachments/assets/da23ab93-bb55-458d-9b86-4615d2a73de6)

+ Scroll down to the two asus options and deselect them by pressing n key.

![Screenshot_20250226_112829](https://github.com/user-attachments/assets/c1c6829b-db24-4f2c-8fc9-bd14f6156840)

+ Press F6 to save .conf then esc to exit and Kernel will start to build this will take up to 30 mins.
+ Follow instructions on screen and select yes to install modules
+ After this is complete run the commands below in your terminal

 ```
sudo pacman -S discover flatpak 
sudo pacman -R inputplumber
yay -S mkinitcpio-firmware
curl -L https://github.com/hhd-dev/hhd/raw/master/install.sh | bash

```
+ Reboot once its done, hold vol up key while booting to go into boot menu and select the new RC kernel 

+ Enjoy HHD 

  





