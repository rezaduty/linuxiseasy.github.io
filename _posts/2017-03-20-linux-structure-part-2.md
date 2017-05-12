---
layout: post
title:  "Linux Structure Part 2"
image: ''
date:  2017-03-15  01-45-39
tags:
- linux
- what is linux
- linux structure
- linux file system
- Kernel
description: ''
category: Linux
---

<center><p>
	
	For any person, who does not have a sound knowledge of Linux Operating System and Linux File System, dealing with the files and their location, their use may be horrible, and a newbie may really mess up.

</p></center>
<img src="{{ site.url }}/assets/img/linux-structure/20161010142555_Linux-ANGRY.png" alt="">

## Linux Directory Structure Diagram
 
Linux Operating System has primarily three components

A standard Linux distribution follows the directory structure as provided below with Diagram and explanation.


<img src="{{ site.url }}/assets/img/linux-structure/Linux-Directory-Structure.jpeg" alt="">



Each of the above directory (which is a file, at the first place) contains important information, required for booting to device drivers, configuration files, etc. Describing briefly the purpose of each directory, we are starting hierarchically.

→ <strong>/bin</strong> : All the executable binary programs (file) required during booting, repairing, files required to run into single-user-mode, and other important, basic commands <val>viz</val>., <em>cat</em>, <em>du</em>, <em>df</em>, <em>tar</em>, <em>rpm</em>, <em>wc</em>, <em>history</em>, etc.<br>
→ <strong>/boot</strong> : Holds important files during <i>boot-up process</i>, including <em><b>Linux Kernel</b></em>.<br>
→ <strong>/dev </strong>: Contains device files for all the hardware devices on the machine e.g., <em>cdrom</em>, <em>cpu</em>, etc<br>
→ <strong>/etc </strong>: Contains Application’s configuration files, <em>startup, shutdown, start, stop</em> script for every individual program.<br>
→ <strong>/home</strong> : Home directory of the users. Every time a new user is created, a directory in the name of user is created within home directory which contains other directories like <em>Desktop, Downloads, Documents</em>, etc.<br>
→ <strong>/lib </strong>:</em> The Lib directory contains <em>kernel modules</em> and <em>shared library</em> images required to boot the system and run commands in root file system.<br>
→ <strong>/lost+found</strong> :</em> This Directory is installed during installation of <em>Linux</em>, useful for recovering files which may be broken due to unexpected <em>shut-down</em>.<br>
→ <strong>/media</strong> : Temporary mount directory is created for removable devices viz., <em>media/cdrom</em>.<br>
→ <strong>/mnt</strong> : Temporary mount directory for <em>mounting file system</em>.<br>
→ <strong>/opt</strong> : Optional is abbreviated as opt. Contains third party application software. Viz., <em>Java</em>, etc.<br>
→ <strong>/proc</strong> : A virtual and pseudo file-system which contains information about <em>running process</em> with a particular <em>Process-id</em> aka <em>pid</em>.<br>
→ <strong>/root</strong> : This is the home directory of root user and should never be confused with ‘/‘<br>
→ <strong>/run</strong> : This directory is the only clean solution for <em>early-runtime-dir</em> problem.<br>
→ <strong>/sbin</strong> : Contains binary executable programs, required by <em>System Administrator</em>, for <em>Maintenance</em>. Viz., <em>iptables</em>, <em>fdisk</em>, <em>ifconfig</em>, swapon, reboot, etc.<br>
→ <strong>/srv</strong> : Service is abbreviated as <em>‘srv‘</em>. This directory contains server specific and service related files.<br>
→ <strong>/sys</strong> : Modern Linux distributions include a <em>/sys</em> directory as a <em>virtual filesystem</em>, which stores and allows modification of the devices connected tothe system.<br>
→ <strong>/tmp</strong> :System’s Temporary Directory, Accessible by users and root. Stores temporary files for <em>user</em> and <em>system</em>, till next boot.<br>
→ <strong>/usr</strong> : Contains executable <em>binaries, documentation, source code, libraries</em> for second level program.<br>
→ <strong>/var</strong> : Stands for variable. The contents of this file is expected to grow. This directory contains <em>log, lock, spool, mail</em> and <em>temp</em> files.<br>


## Exploring Important file, their location and their Usability

<em>Linux</em> is a complex system which requires a more complex and efficient way to <em>start</em>, <em>stop</em>, <em>maintain</em> and <em>reboot</em> a system unlike <em>Windows</em>. There is a well defined configuration <em>files</em>, <em>binaries</em>, <em>man pages</em>, <em>info files</em>, etc. for every <em>process</em> in <em>Linux</em>.



→ <strong>/boot/vmlinuz</strong> : The <em>Linux Kernel</em> file.<br>
→ <strong>/dev/hda</strong> : Device file for the first <em>IDE HDD</em> (<em>Hard Disk Drive</em>)<br>
→ <strong>/dev/hdc</strong> : Device file for the <em>IDE Cdrom</em>, commonly<br>
→ <strong>/dev/null</strong> : A pseudo device, that don’t exist. Sometime garbage output is redirected to <em>/dev/null</em>, so that it gets lost, forever.<br>
→ <strong>/etc/bashrc</strong> : Contains system <em>defaults</em> and <em>aliases</em> used by bash shell.<br>
→ <strong>/etc/crontab</strong> : A <a target="_blank" href="http://www.tecmint.com/category/bash-shell/" target="_blank">shell script</a> to run specified commands on a → predefined time Interval.<br>
→ <strong>/etc/exports</strong> : Information of the file system available on <em>network</em>.<br>
→ <strong>/etc/fstab</strong> : Information of <em>Disk Drive</em> and their mount point.<br>
→ <strong>/etc/group</strong> : Information of <em>Security Group</em>.<br>
→ <strong>/etc/grub.conf</strong> : grub <em>bootloader</em> configuration file.<br>
→ <strong>/etc/init.d</strong> : Service <em>startup</em> Script.<br>
→ <strong>/etc/lilo.conf</strong> : lilo <em>bootloader</em> configuration file.<br>
→ <strong>/etc/hosts</strong> : Information of <em>Ip addresses</em> and corresponding <em>host names</em>.<br>
→ <strong>/etc/hosts.allow</strong> : List of <em>hosts allowed</em> to access services on the local machine.<br>
→ <strong>/etc/host.deny</strong> : List of <em>hosts denied</em> to access services on the local machine.<br>
→ <strong>/etc/inittab</strong> : INIT process and their interaction at various<em> run level</em>.<br>
→ <strong>/etc/issue</strong> : Allows to edit the <em>pre-login</em> message.<br>
→ <strong>/etc/modules.conf</strong> : Configuration files for <em>system modules</em>.<br>
→ <strong>/etc/motd</strong> : <a target="_blank" href="http://www.tecmint.com/protect-ssh-logins-with-ssh-motd-banner-messages/" target="_blank">motd</a> stands for <em>→ Message Of The Day</em>, The Message users gets upon login.<br>
→ <strong>/etc/mtab</strong> : Currently mounted <em>blocks</em> information.<br>
→ <strong>/etc/passwd</strong> : Contains <em>password</em> of system <em>users</em> in a shadow file, a security implementation.<br>
→ <strong>/etc/printcap</strong> : <em>Printer</em> Information<br>
→ <strong>/etc/profile</strong> : Bash shell <em>defaults</em><br>
→ <strong>/etc/profile.d</strong> : Application script, executed after <em>login</em>.<br>
→ <strong>/etc/rc.d</strong> : Information about <em>run level</em> specific script.<br>
→ <strong>/etc/rc.d/init.d</strong> : Run Level <em>Initialisation</em> Script.<br>
→ <strong>/etc/resolv.conf</strong> : Domain Name Servers (<em>DNS</em>) being used by System.<br>
→ <strong>/etc/securetty</strong> : Terminal List, where <em>root</em> login is possible.<br>
→ <strong>/etc/skel</strong> : Script that populates new user <em>home</em> directory.<br>
→ <strong>/etc/termcap</strong> : An <em>ASCII</em> file that defines the behaviour of <em>Terminal</em>, <em>console</em> and <em>printers</em>.<br>
→ <strong>/etc/X11</strong> : Configuration files of <em>X-window</em> System.<br>
→ <strong>/usr/bin</strong> : Normal user <em>executable</em> commands.<br>
→ <strong>/usr/bin/X11</strong> : Binaries of <em>X windows</em> System.<br>
→ <strong>/usr/include</strong> : Contains include files used by ‘<em>c</em>‘ program.<br>
→ <strong>/usr/share</strong> : Shared directories of <em>man files</em>, <em>info files</em>, etc.<br>
→ <strong>/usr/lib</strong> : Library files which are required during program <em>compilation</em>.<br>
→ <strong>/usr/sbin</strong> : Commands for <em>Super User</em>, for System Administration.<br>
→ <strong>/proc/cpuinfo</strong> : <em>CPU</em> Information<br>
→ <strong>/proc/filesystems</strong> : File-system <em>Information</em> being used currently.<br>
→ <strong>/proc/interrupts</strong> : Information about the current <em>interrupts</em> being utilised currently.<br>
→ <strong>/proc/ioports</strong> : Contains all the <em>Input</em>/<em>Output</em> addresses used by devices on the server.<br>
→ <strong>/proc/meminfo</strong> : <em>Memory Usages</em> Information.<br>
→ <strong>/proc/modules</strong> : Currently using <em>kernel</em> module.<br>
→ <strong>/proc/mount</strong> : Mounted <em>File-system</em> Information.<br>
→ <strong>/proc/stat</strong> : Detailed<em> Statistics</em> of the current System.<br>
→ <strong>/proc/swaps</strong> : <em>Swap</em> File Information.<br>
→ <strong>/version</strong> : Linux <em>Version</em> Information.<br>
→ <strong>/var/log/lastlog</strong> : log of last <em>boot</em> process.<br>
→ <strong>/var/log/messages</strong> : log of messages produced by <em>syslog</em> daemon at boot.<br>
→ <strong>/var/log/wtmp</strong> : list login <em>time</em> and <em>duration</em> of each user on the system currently.<br>

<img src="{{ site.url }}/assets/img/linux-structure/Linux-file-system-hierarchy-v2.0-2480px-blackMORE-Ops.png" alt="">

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