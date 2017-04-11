---
layout: post
title:  "How to install a linux distro"
image: ''
date:   2017-03-15  01-03-01
tags:
- linux
- How to 
- How to install a linux distibute
- what is linux
description: ''
categories:
- Linux
---

<center><p>The number of Linux distributions is declining. In 2011, the Distrowatch database of active Linux distributions peaked at <b>323</b></p></center>
<img src="{{ "/assets/img/how-to-install-a-linux-distro/linux-logo.jpg"}}" alt="">

## How to install a linux distro ? 


<center>
<figure class="foto-legenda">
	<img src="{{ "/assets/img/how-to-install-a-linux-distro/Install-Linux-Mint-18-Dual-Boot-with-Windows-10.png"}}" alt="">
</figure>
</center>

Samply im select mint linux (becuase linux mint very similar windows user interface)

#Step 1: Shrink HDD Space for Dual-Boot
1.In case your computer comes pre-installed with Microsoft Windows on a single partition, logon to Windows system with a user who has administrator privileges, press [Win+r] keys to open run prompt and type the following command in order to open Disk Management tool.

diskmgmt.msc

<figure class="foto-legenda">
	<img src="{{ "/assets/img/how-to-install-a-linux-distro/Open-Windows-Disk-Management.png"}}" alt="">
</figure>

2.Right click on C: partition and select Shrink Volume in order to resize the partition.
The OS is comprised of a number of pieces: 

<figure class="foto-legenda">
	<img src="{{ "/assets/img/how-to-install-a-linux-distro/Shrink-Windows-Partition.png"}}" alt="">
</figure>


3.Use a value best-suited for you, depending on your HDD size, on the amount of space to shrink MB field (minimum 20000 MB recommended) and hit Shrink button to start the process of resizing the partition.

<figure class="foto-legenda">
	<img src="{{ "/assets/img/how-to-install-a-linux-distro/Assign-Partition-Size.png"}}" alt="">
</figure>

4.When the process finishes a new unallocated space will appear on the hard drive.

<figure class="foto-legenda">
	<img src="{{ "/assets/img/how-to-install-a-linux-distro/Unallocated-Partition.png"}}" alt="">
</figure>

Close Disk Management utility, place Linux Mint DVD or USB bootable image in the appropriate drive and reboot the computer in order to start with Linux Mint 18 installation.

In case you’re booting Linux Mint for installation from a USB dive in UEFI mode make sure you’ve created the bootable USB stick using a utility such as Rufus, which is UEFI compatible, otherwise your USB bootable drive won’t boot.

<hr>

#Step 2: Installation of Linux Mint 18

5.After reboot, press the special function key and instruct the machine firmware (UEFI) to boot-up from the appropriate DVD or USB drive (the special function keys usually are F12, F10 or F2 depending on the motherboard manufacturer).

Once the media boots-up a new screen should appear on your monitor. Choose Start Linux Mint 18 Cinnamon and hit Enter to continue.

<figure class="foto-legenda">
	<img src="{{ "/assets/img/how-to-install-a-linux-distro/Select-Start-Linux-Mint-Cinnamon-Install.png"}}" alt="">
</figure>

6.Wait until the system loads into RAM in order to run in live-mode and open the installer by double clicking on Install Linux Mint icon.

Choose the language you wish to perform the installation and click on Continue button to proceed further.

<figure class="foto-legenda">
	<img src="{{ "/assets/img/how-to-install-a-linux-distro/Select-Install-Linux-Mint.png"}}" alt="">
</figure>

<figure class="foto-legenda">
	<img src="{{ "/assets/img/how-to-install-a-linux-distro/Select-Installation-Language.png"}}" alt="">
</figure>


7.On the next screen hit on Continue button to proceed further. Third-party software can be automatically download and installed on this step by checking the check-box.

The recommendation would be to leave the box unchecked for the moment and manually install proprietary software later, after the installation process completes.


<figure class="foto-legenda">
	<img src="{{ "/assets/img/how-to-install-a-linux-distro/Preparing-to-Install-Linux-Mint-18.png"}}" alt="">
</figure>


8.At the next screen you can choose the Installation Type. If Windows Boot manager is automatically detected you can choose to Install Linux Mint alongside Windows Boot Manager. This option ensures that the HDD will be automatically partitioned by the installer without any data loss.

The second option, Erase disk and install Ubuntu, should be avoided for dual-boot because is potentially dangerous and will wipe-out your disk.

For a more flexible partition layout you should go with Something else option and hit on Continue button to proceed further.

<figure class="foto-legenda">
	<img src="{{ "/assets/img/how-to-install-a-linux-distro/Select-Installation-Type-for-Linux-Mint-18.png"}}" alt="">
</figure>


9.Now let’s create the partition layout for Linux Mint 18. I would recommend that you create three partitions, one for / (root), one for /home accounts data and one partition for swap.

First create the swap partition. Select the free space and hit on the + icon from below. On this partition use the following settings and hit OK to create the partition:

{% highlight javascript %}
	Size = 1024 MB
	Type for the new partition = Primary
	Location for the new partition = Beginning of this space
	Use as = swap area
{% endhighlight %}

<figure class="foto-legenda">
	<img src="{{ "/assets/img/how-to-install-a-linux-distro/Select-Free-Partition-Space.png"}}" alt="">
</figure>

<figure class="foto-legenda">
	<img src="{{ "/assets/img/how-to-install-a-linux-distro/Create-Swap-Partition.png"}}" alt="">
</figure>

10.Using the same steps as above create the /(root) partition with the below settings:

{% highlight javascript %}
	Size = minimum 20 GB
	Type for the new partition = Primary
	Location for the new partition = Beginning of this space
	Use as = EXT4 journaling file system
	Mount point = /
{% endhighlight %}

<figure class="foto-legenda">
	<img src="{{ "/assets/img/how-to-install-a-linux-distro/Select-Free-Space.png"}}" alt="">
</figure>

<figure class="foto-legenda">
	<img src="{{ "/assets/img/how-to-install-a-linux-distro/Create-Root-Partition.png"}}" alt="">
</figure>

11.Finally, create the home slice with the below settings (use all the available free space to create home partition).

Home partition is the place where all documents for user accounts will be stored by default, except the root account. In case of a system failure you can reinstall the operating system for scratch without touching or losing the settings and documents of all users.

{% highlight javascript %}
	Size = remaining free space
	Type for the new partition = Primary
	Location for the new partition = Beginning 
	Use as = EXT4 journaling file system
	Mount point = /home
{% endhighlight %}

<figure class="foto-legenda">
	<img src="{{ "/assets/img/how-to-install-a-linux-distro/Create-Home-Partition.png"}}" alt="">
</figure>

12.After finishing creating the partition layout, select Windows Boot Manager as the device for installing the Grub boot loader and hit on Install Now button in order to commit changes to disk and proceed with the installation.

Next a new pop-up window will ask you if you agree with committing changes to disk. Hit on Continue to accept changes and the installer will now start to write changes to disk.

<figure class="foto-legenda">
	<img src="{{ "/assets/img/how-to-install-a-linux-distro/Linux-Mint-18-Installation-Summary.png"}}" alt="">
</figure>

<figure class="foto-legenda">
	<img src="{{ "/assets/img/how-to-install-a-linux-distro/Accept-Write-Changes-to-Disk.png"}}" alt="">
</figure>

13.On the next screen choose your nearest physical location from the map and hit Continue.

<figure class="foto-legenda">
	<img src="{{ "/assets/img/how-to-install-a-linux-distro/Select-Country-Zone.png"}}" alt="">
</figure>

14.Next you should select your keyboard layout and click on Continue button.

<figure class="foto-legenda">
	<img src="{{ "/assets/img/how-to-install-a-linux-distro/Select-Keyboard-Layout.png"}}" alt="">
</figure>


15.Enter a username and a password for the first account with root privileges, choose your system hostname by filling the computer’s name field with a descriptive value and hit Continue to finalize the installation process.

<figure class="foto-legenda">
	<img src="{{ "/assets/img/how-to-install-a-linux-distro/Create-User-Account.png"}}" alt="">
</figure>


16.The installation process will take a while and when it reaches the final step it will ask you to hit on Restart Now button to complete the installation.

<figure class="foto-legenda">
	<img src="{{ "/assets/img/how-to-install-a-linux-distro/Linux-Mint-18-Installation-Completed.png"}}" alt="">
</figure>


17.After reboot, the system will first boot-up in Grub, with Linux Mint as the first boot option which will be automatically started after 10 seconds. Form here you can further instruct the computer to boot in Windows or Linux.

On computers with newer UEFI firmware the Grub boot loader won’t be displayed by default and the machine will automatically boot-up in Windows.

In order to boot into Linux you must press the special function boot key after restart and from there to further select what OS you wish to start.

In order to change the default boot order enter UEFI settings, select your default OS and save the changes. Review the vendor’s manual in order to detect the special function keys used for boot or for entering UEFI settings.

18.After the system finishes loading, log in to Linux Mint 18 by using the credentials created during the installation process. Fire-up a Terminal window and start the update process from command line by running the following commands:

{% highlight javascript %}

	$ sudo apt-get update
	$ sudo apt-get upgrade

{% endhighlight %}

That’s it! You have successfully installed the latest version of Linux Mint 18 on your device. You will find Linux Mint platform to be very robust, fast, flexible, enjoyable, easy to use, with a ton of software required for a normal user already installed and very stable.

### Finaly Please watch video for better install linux 

<center>
	<b>Please Watch video</b>
	<br>
	<video onclick="this.paused ? this.play() : this.pause();" controls width="50%" poster="../assets/img/static/videoposter.jpg" height="50%" src="../assets/img/how-to-install-a-linux-distro/c0c895766d20ae5de27f91853edacf565943209-360p__57279.mp4">
		Video Tag Not Support
	</video>

</center>

{% include content_option.html %}


<center>♥♥♥♥♥♥♥♥♥♥
<br><b>Please Gaming and give point for end of document your uderstand top linux command</b><br>
</center>
<hr>
<span>Draw back an arrow and launch it(center give point till 3 success launche)!</span>

<!---
{% highlight javascript %}
use admin
db.createUser{
	user: "bonitao",
	pwd: "2016bonitao",
	roles: [{role: "userAdminAnyDatabase", db: "admin"}]
}
{% endhighlight %}
-->

{% include game_include.html %}