# Infinix-Note-11s-X698-TWRP
TWRP RECOVERY FOR INFINIX NOTE 11S (X698)

UNLOCKING BOOTLOADER
After unlocking the bootloader, your internal storage will be WIPED.

1. Unlock developer options, first go to Settings -> My Phone then tap Build Number 7 times.
![image](https://user-images.githubusercontent.com/118900349/203546437-c977cdb7-7a8b-4516-82da-96bb6713f2b4.png)
2. Go to System -> Developer Option and enable OEM unlocking
![image](https://user-images.githubusercontent.com/118900349/203546624-39fd503c-e9cb-44f3-ab2e-c823286e3945.png)
![image](https://user-images.githubusercontent.com/118900349/203546646-5ea6ba21-7b1d-4744-a6ec-2070cdf3c84f.png)
3. On PC extract downloaded files then open DriverInstall.exe and install it
4. Plug your phone into PC and run "cmd-here.exe" on your PC.
5. Now type
adb devices
adb reboot-bootloader
fastboot flashing unlock
fastboot reboot
4. Your phone will reboot and you need to set up again
MAKE SURE YOU UNLOCKED BOOTLODER
NOTES: Please reade README.txt on the archive
1. Download and extract required files
2. Connect your phone into fastboot mode
3. Run "cmd-here.exe" from before on your PC.
4. Confirm if device is connected, type
fastboot devices
5. Flash the patched boot.img
fastboot flash boot {name of image}.img
6. MUST disable vbmeta boot verification
fastboot flash --disable-verity --disable-verification vbmeta vbmeta.img
7. Unplug and verify, do reboot to recovery with power + vol up combination.
