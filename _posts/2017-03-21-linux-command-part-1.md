---
layout: post
title:  "Linux Command Part 1"
image: ''
date:  2017-03-15  01-45-39
tags:
- linux
- what is linux
- linux command
- important linux command
description: ''
category: Linux
---

<center><p>
	
	Terminal is your friend.

</p></center>
<img src="{{ site.url }}/assets/img/linux-terminal/linux_terminal_tw.png" alt="">

## how to open terminal 

### Keyboard Shortcuts

{% highlight javascript %}

	Ctrl + Alt + t

{% endhighlight %}

<center>
		<b>Please Watch video</b>
		<br>
		<div class="video">
			<div id="14920177592009820"><script type="text/JavaScript" src="https://www.aparat.com/embed/p2XTf?data[rnddiv]=14920177592009820&data[responsive]=yes"></script></div>
		</div>
		<br><br>

</center>

## File and Folder Managment

<center>
		<b>Please Watch video</b>
		<br>
		<div class="video">
			<div id="14920175432778242"><script type="text/JavaScript" src="https://www.aparat.com/embed/XpeDg?data[rnddiv]=14920175432778242&data[responsive]=yes"></script></div>
		</div>
		<br><br>
</center>



## System Info

<p>
 <strong>date</strong> → Show the current date and time<br>
 <strong>cal</strong> → Show this month's calendar<br>
 <strong>uptime</strong> → Show current uptime<br>
 <strong>w</strong> → Display who is online<br>
 <strong>whoami</strong> → Who you are logged in as<br>
 <strong>finger <em>user</em></strong> → Display information about <em><strong>user</strong></em><br>
 <strong>uname -a</strong> → Show kernel information<br>
 <strong>cat /proc/cpuinfo</strong> → CPU information<br>
 <strong>cat /proc/meminfo</strong> → Memory information<br>
 <strong>df</strong> <strong>-h</strong> → Show disk usage<br>
 <strong>du</strong> → Show directory space usage<br>
 <strong>free</strong> → Show memory and swap usage</p>

<center>
		<b>Please Watch video</b>
		<br>
		<video onclick="this.paused ? this.play() : this.pause();" controls width="50%" poster="../assets/img/static/videoposter.jpg" height="50%" src="../assets/img/linux-terminal/How-to-check-Linux-System-Info-43.mp4">
			Video Tag Not Support
		</video>

</center>

## Keyboard Shortcuts

<p>
 <strong>Enter</strong> → Run the command<br>
 <strong>Up Arrow</strong> → Show the previous command<br>
 <strong>Ctrl + R</strong> → Allows you to type a part of the command you're looking for and finds it</p>


## Learn the Commands

<p>
 <strong>apropos</strong><em><strong> subject</strong></em> → List manual pages for <strong><em>subject</em></strong><br>
 <strong>man -k <em>keyword</em></strong> → Display man pages containing <em><strong>keyword</strong></em><br>
 <strong>man <em>command</em></strong> → Show the manual for <strong><em>command</em></strong><br>
 <strong>man -t <em>man</em> | ps2pdf - &gt; <em>man.pdf</em></strong>&nbsp; → Make a pdf of a manual page<br>
 <strong>which </strong><em><strong>command</strong></em> → Show full path name of <strong><em>command</em></strong><br>
 <strong>time <em>command</em></strong> → See how long a <strong><em>command</em></strong> takes</p>

 <p>
 <strong>whereis <em>app</em></strong> → Show possible locations of <em><strong>app</strong></em><br>
 <strong>which <em>app</em></strong> → Show which <em><strong>app</strong></em> will be run by default; it shows the full path</p>

## Searching

<p>
 <strong>grep <em>pattern</em> <em>files</em></strong> → Search for <em><strong>pattern</strong></em> in <em><strong>files</strong></em><br>
 <strong>grep -r <em>pattern</em> <em>dir</em></strong> → Search recursively for <strong><em>pattern</em></strong> in <em><strong>dir</strong></em><br>
 <em><strong>command | </strong></em><strong>grep</strong><em><strong> pattern</strong></em> → Search for <em><strong>pattern</strong></em> in the output of <em><strong>command</strong></em><br>
 <strong>locate <em>file</em></strong> → Find all instances of <em><strong>file</strong></em><br>
 <strong>find / -name <em>filename</em></strong> → Starting with the root directory, look for the file called <em><strong>filename</strong></em><br>
 <strong>find / -name ”*<em>filename</em>*”</strong> → Starting with the root directory, look for the file containing the string <em><strong>filename</strong></em><br>
 <strong>locate <em>filename</em></strong> → Find a file called <em><strong>filename</strong></em> using the locate command; this assumes you have already used the command <strong>updatedb</strong> (see next)<br>
 <strong>updatedb</strong> → Create or update the database of files on all file systems attached to the Linux root directory<br>
 <strong>which <em>filename</em></strong> → Show the subdirectory containing the executable file&nbsp; called <em><strong>filename</strong></em><br>
 <strong>grep <em>TextStringToFind</em> /<em>dir</em></strong> → Starting with the directory called <em><strong>dir</strong></em>, look for and list all files containing <em><strong>TextStringToFind</strong></em></p>

<center>
		<b>Please Watch video</b>
		<br>
		<div class="video">
			<div id="14920178899577480"><script type="text/JavaScript" src="https://www.aparat.com/embed/rx2bk?data[rnddiv]=14920178899577480&data[responsive]=yes"></script></div>
		</div>
		<br><br>

</center>


## File Permissions

<p>
 <strong>chmod <em>octal</em> <em>file</em></strong> → Change the permissions of <em><strong>file</strong></em> to <em><strong>octal</strong></em>, which can be found separately for user, group, and world by adding: 4 → read (r), 2 → write (w), 1 → execute (x)<br>
 Examples:<br>
 <strong>chmod 777</strong> → read, write, execute for all<br>
 <strong>chmod 755</strong> → rwx for owner, rx for group and world<br>
 For more options, see <strong>man chmod</strong>.</p>

<center>
		<b>Please Watch video</b>
		<br>
		<div class="video">
			<div id="1492017983546790"><script type="text/JavaScript" src="https://www.aparat.com/embed/E9cLS?data[rnddiv]=1492017983546790&data[responsive]=yes"></script></div>
		</div>
		<br><br>

</center>


## Compression

<p>
 <strong>tar cf <em>file.tar files</em></strong><em> </em>→ Create a tar named <em><strong>file.tar</strong></em> containing <em><strong>files</strong></em><br>
 <em><strong>tar xf file.tar</strong></em> → Extract the files from <em><strong>file.tar</strong></em></p>
<br>	
 <p>
 <strong>tar czf <em>file.tar.gz files</em></strong> → Create a tar with Gzip compression<br>
 <strong>tar xzf <em>file.tar.gz</em> </strong>→ Extract a tar using Gzip</p>
<br>
<p>
 <em><strong>tar cjf file.tar.bz2</strong></em> → Create a tar with Bzip2 compression<br>
 <strong>tar xjf <em>file.tar.bz2</em></strong> → Extract a tar using Bzip2</p>
 <br>
 <p>
 <strong>gzip <em>file</em></strong> → Compresses <strong><em>file</em></strong> and renames it to <strong><em>file.gz</em></strong><br>
 <strong>gzip -d <em>file.gz</em></strong> → Decompresses <strong><em>file.gz</em></strong> back to <strong><em>file</em></strong></p>

<center>
		<b>Please Watch video</b>
		<br>
		<video onclick="this.paused ? this.play() : this.pause();" controls width="50%" poster="../assets/img/static/videoposter.jpg" height="50%" src="../assets/img/linux-terminal/Linux-Commands-6-File-CompressionDecom-pression-zip-unzip-tar-43.mp4">
			Video Tag Not Support
		</video>

</center>



## Printing

<p>
 <strong>/etc/rc.d/init.d/lpd start</strong> → Start the print daemon<br>
 <strong>/etc/rc.d/init.d/lpd stop</strong> → Stop the print daemon<br>
 <strong>/etc/rc.d/init.d/lpd status</strong> → Display status of the print daemon<br>
 <strong>lpq</strong> → Display jobs in print queue<br>
 <strong>lprm</strong> → Remove jobs from queue<br>
 <strong>lpr</strong> → Print a file<br>
 <strong>lpc</strong> → Printer control tool<br>
 <strong>man <em>subject</em> | lpr</strong> → Print the manual page called <strong><em>subject</em></strong> as plain text<br>
 <strong>man -t <em>subject</em> | lpr</strong> → Print the manual page called <strong><em>subject</em></strong> as Postscript output<br>
 <strong>printtool</strong> → Start X printer setup interface</p>

<center>
		<b>Please Watch video</b>
		<br>
		<div class="video">
			<div id="14920141622173599"><script type="text/JavaScript" src="https://www.aparat.com/embed/vAGDH?data[rnddiv]=14920141622173599&data[responsive]=yes"></script></div>
		</div>
		<br><br>
</center>



## Network

<p>
 <strong>ifconfig</strong> → List IP addresses for all devices on the local machine<br>
 <strong>iwconfig</strong> → Used to set the parameters of the network interface which are specific to the wireless operation (for example: the frequency)<br>
 <strong>iwlist</strong> → used to display some additional information from a wireless network interface that is not displayed by <strong>iwconfig</strong><br>
 <strong>ping</strong><em><strong> host</strong></em> → Ping <strong><em>host</em></strong> and output results<br>
 <strong>whois <em>domain</em></strong> → Get whois information for <em><strong>domain</strong></em><br>
 <strong>dig <em>domain</em></strong> → Get DNS information for <em><strong>domain</strong></em><br>
 <strong>dig -x</strong><em><strong> host</strong></em> → Reverse lookup <em><strong>host</strong></em><br>
 <strong>wget <em>file</em></strong> → Download <em><strong>file</strong></em><br>
 <strong>wget -c</strong><em><strong> file</strong></em> → Continue a stopped download</p>

<center>
		<b>Please Watch video</b>
		<br>
		<div class="video">
			<div id="14920177136846397"><script type="text/JavaScript" src="https://www.aparat.com/embed/F2PIh?data[rnddiv]=14920177136846397&data[responsive]=yes"></script></div>
		</div>
		<br><br>
</center>


## SSH

<p class="">
 <strong>ssh <em>user</em>@<em>host</em></strong> → Connect to <strong><em>host</em></strong> as <em><strong>user</strong></em><br>
 <strong>ssh -p <em>port user</em>@<em>host</em></strong> → Connect to <em><strong>host</strong></em> on port <em><strong>port</strong></em> as <em><strong>user</strong></em><br>
 <strong>ssh-copy-id <em>user</em>@<em>host</em></strong> → Add your key to <em><strong>host</strong></em> for <em><strong>user</strong></em> to enable a keyed or passwordless login</p>


<center>
		<b>Please Watch video</b>
		<br>
		<div class="video">
			<div id="14920179289918513"><script type="text/JavaScript" src="https://www.aparat.com/embed/mGSxL?data[rnddiv]=14920179289918513&data[responsive]=yes"></script></div>
		</div>
		<br><br>

</center>


## User Administration


<p>
 <strong>adduser </strong><em><strong>accountname</strong></em> → Create a new user call <em><strong>accountname</strong></em><br>
 <strong>passwd <em>accountname</em></strong> → Give <em><strong>accountname</strong></em> a new password<br>
 <strong>su</strong> → Log in as superuser from current login<br>
 <strong>exit</strong> → Stop being superuser and revert to normal user</p>

<center>
		<b>Please Watch video</b>
		<br>
		<div class="video">
			<div id="14920545979830099"><script type="text/JavaScript" src="https://www.aparat.com/embed/uWlMz?data[rnddiv]=14920545979830099&data[responsive]=yes"></script></div>
		</div>
		<br><br>

</center>


## Process Management


<p>
 <strong>ps</strong> → Display your currently active processes<br>
 <strong>top</strong> → Display all running processes<br>
 <strong>kill <em>pid</em></strong> → Kill process id <em><strong>pid</strong></em><br>
 <strong>killall <em>proc</em></strong> → Kill all processes named <em><strong>proc</strong></em> (use with extreme caution)<br>
 <strong>bg</strong> → Lists stopped or background jobs; resume a stopped job in the background(Ctrl+Z and type bg or fg)<br>
 <strong>fg</strong> → Brings the most recent job to foreground<br>
 <strong>fg</strong><em><strong> n</strong></em> → Brings job <em><strong>n</strong></em> to the foreground</p>

<center>
		<b>Please Watch video</b>
		<br>
		<div class="video">
			<div id="14920183169022237"><script type="text/JavaScript" src="https://www.aparat.com/embed/jrHWR?data[rnddiv]=14920183169022237&data[responsive]=yes"></script></div>
		</div>
		<br><br>

</center>


## Online installation:

### 1. Through software manager(linux mint)/software center(ubuntu):

<p>
 first open the terminal and run this command to get the <strong>latest version</strong> of the software:</p>

 <p>
 <strong>sudo apt-get update</strong></p>

 <p>then</p>

 <p>
 1. open <strong>software manager/center</strong>. it&#39;s in the <strong>menu</strong>.</p>
<p>
 2. search your desired software in the <strong>search box</strong></p>
<p>
 3. if it&#39;s in the list then it will appear before you .<strong> if it&#39;s not in the list follow the instructions in the ppa installation section of this tutorial.</strong></p>
<p>
 4. now double click on the desired software entry and then click &quot;<strong>install</strong>&quot;.</p>
<p>
 5. it will be installed on your system as per your network connection speed.</p>
<p>

### 2. Through synaptic package manager:

<p>
 <span style="color:#008080;"><span style="font-size: 16px;"><span style="font-size: 12px;">if it is absent in your linux distribution then you will have to install it through software manager/center first.</span></span></span></p>
<p>
 <span style="font-size:16px;"><span style="font-size:12px;">to me it&#39;s the best way to install softwares in linux.</span></span></p>
<p>
 <span style="font-size:16px;"><span style="font-size:12px;">1. open <strong>synaptic package manager</strong></span></span>. click <strong>reload</strong> to get the latest version of the softwares.</p>
<p>
 <span style="font-size:16px;"><span style="font-size:12px;">2. search your desired software/s in the <strong>search box</strong>.</span></span></p>
<p>
 <span style="font-size:16px;"><span style="font-size:12px;">3. right click each software you want to install and <strong>mark them for installing</strong>. it will mark additional dependencies on it&#39;s own.</span></span></p>
<p>
 <strong>if your softwares not in the list follow the instructions in the ppa installation section of this tutorial.</strong></p>
<p>
 4. after marking for installing, click <strong>apply</strong></p>
<p>
 6. it will download and install the marked softwares.</p>
<p>
 <em><span style="color:#006400;"><span style="font-size: 14px;">additional info:</span></span></em></p>
<p>
 if you have a list of softwares then save the file with the list, with .list extension (this file should contain the exact package name one at every line with an extra string &quot;<strong>install</strong>&quot; included after each package name preceding by an space/tab). then go to file-&gt;read markings&nbsp; and then brows to the file and open it. synaptic will mark the softwares in the list automatically.</p>
<p>

### 3. Through terminal:

<p>
 if you know the exact name of the software then you can install it through terminal by simply entering the command:</p>
<p>
 <strong>sudo apt-get update</strong>&nbsp;&nbsp;&nbsp; (to get the latest version)</p>
<p>
 <strong>sudo apt-get install software-package-name</strong></p>
<p>
 that&#39;s it.....</p>
<p>
 <strong>if it says &quot;unable to locate package...&quot;&nbsp; then follow the instructions in the ppa installation section of this tutorial.</strong></p>
<p>

### 4. PPA installation:

<p>
 if your software&#39;s not in the software list then it may come from private package archives (PPA&#39;s).</p>
<p>
 <span style="color:#800000;">these are private development of softwares so use it at your own risk.</span></p>
<p>
 steps:</p>
<p>
 1. search google for the ppa address for your software. (like ppa for package-name)</p>
<p>
 2. then add it to the repository by entering this command in terminal:</p>
<p>
 <strong>sudo add-apt-repository ppa:.....whatever_it_is</strong></p>
<p>
 3. then run this command (must)</p>
<p>
 <strong>sudo apt-get update</strong></p>
<p>
 4. now your desired software is in the list. so you can follow one of the above processes (#1,#2,#3)</p>
<p>
 &nbsp;</p>

</p></p></p>



## Installation from source:

<p>
 <strong>./configure</strong><br>
 <strong>make</strong><br>
 <strong>make install</strong><br></p>
 <p>
 <span style="color:#008080;">if the first code fails to execute then run this code before above codes:</span></p>
<p>
 <strong>chmod +x configure</strong></p>
<p>
 <strong>dpkg -i</strong><em><strong> pkg.deb</strong></em> → install a DEB package (Debian / Ubuntu / Linux Mint)<br>
 <strong>rpm -Uvh <em>pkg.rpm</em></strong> → install a RPM package (Red Hat / Fedora)</p>

</p></p>
### 9. installing .sh files:

<p>
 some softwares come with a .sh file to install it</p>
<p>
 <strong>chmod +x filename.sh&nbsp; </strong></p>
<p>
 <strong>./filename.sh </strong>or<strong> <strong>sudo ./filename.sh</strong> </strong>(if it needs root permission)</p>
<p>
 or double click it and select <strong>run in terminal</strong> or <strong>run</strong>, whatever supports your software.</p>


### 10. installing .run files:

<p>
 some softwares come with a .run file to install it</p>
<p>
 <strong>chmod +x filename.run</strong></p>
<p>
 <strong>./filename.run </strong>or<strong> <strong>sudo ./filename.run</strong> </strong>(if it needs root permission)</p>
<p>
 or double click it and select <strong>run in terminal</strong> or <strong>run</strong>, whatever supports your software.</p>
<p>

<center>
		<b>Please Watch video</b>
		<br>
		<div class="video">
			<div id="1492018029143582"><script type="text/JavaScript" src="https://www.aparat.com/embed/BvIpg?data[rnddiv]=1492018029143582&data[responsive]=yes"></script></div>
		</div>
		<br><br>

</center>


<h3>Stopping and Starting</h3>

<p>
 <strong>shutdown -h now</strong> → Shutdown the system now and do not reboot<br>
 <strong>halt</strong> → Stop all processes - same as above<br>
 <strong>shutdown -r 5</strong> → Shutdown the system in 5 minutes and reboot<br>
 <strong>shutdown -r now</strong> → Shutdown the system now and reboot<br>
 <strong>reboot</strong> → Stop all processes and then reboot - same as above<br>
 <strong>startx</strong> → Start the X system</p><br>

<center>
		<b>Please Watch video</b>
		<br>
		<video onclick="this.paused ? this.play() : this.pause();" controls width="50%" poster="../assets/img/static/videoposter.jpg" height="50%" src="../assets/img/linux-terminal/Commands-to-shutdown-restart-in-linux-18.mp4">
			Video Tag Not Support
		</video>

</center>



<h3> Recommended reading</h3>

<br>❝<a target="_blank" href="https://en.wikipedia.org/wiki/Cheat_sheet
">Cheat sheet</a> is very fast way learning❞

<b><p>Cvak iranian linux was from isfehan and lpic1 cheatsheet<a href="/assets/img/linux-commands/c_lpic1.zip">&nbsp;sample</a></p></b><br>

<p>
<a target="_blank" href="http://www.cheat-sheets.org/#Linux">Cheat-Sheets.org</a> → All cheat sheets, round-ups, quick reference cards, quick reference guides and quick reference sheets in one page. The only one you need. <br>

<a target="_blank" href="http://www.linuxtutorialblog.com/post/tutorial-the-best-tips-tricks-for-bash">Tutorial: The best tips & tricks for bash, explained</a> → Linux Tutorial Blog / Quality Linux tutorials without clutter <br>

<a target="_blank" href="http://linuxcommand.org/">LinuxCommand.org</a> → Learning the shell, Writing shell scripts, Script library, SuperMan pages, Who, What, Where, Why <br>

<a target="_blank" href="http://linuxmanpages.com/">LinuxManPages.com</a> → General commands, System calls, Subroutines, Special files, File formats, Games, Macros and conventions, Maintenence commands, Most Popular Man Pages <br>

<a target="_blank" href="http://linux.die.net/man/">Linux Man Pages from die.net</a> → Man pages are grouped into sections, to see the full list of Linux man pages for a section, pick one. Or you can browse Linux man pages by name; choose the first letter of the name of the Linux command, function, or file you are interested in. <br>

<a target="_blank" href="http://www.unixguide.net/linux/linuxshortcuts.shtml">Linux Newbie Guide: Shorcuts and Commands</a> → Linux essential shortcuts and sanity commands; Common Linux commands - system info; Basic operations, network apps, file (de)compression; Process control; Basic administration commands, accessing drives/partitions; Network administration tools, music-related commands, graphics-related commands. <br>

<a target="_blank" href="http://www.gratisoft.us/sudo/man.html">Sudo Manual Pages</a> → Sudo (su "do") allows a system administrator to delegate authority to give certain users (or groups of users) the ability to run some (or all) commands as root or another user while providing an audit trail of the commands and their arguments. For more information, see the introduction to Sudo. Sudo is free software, distributed under an ISC-style license. <br>

<a target="_blank" href="http://linoxide.com/linux-command/linux-commands-cheat-sheet/">LinOxide.com</a> → Linux Commands Cheat Sheet in Black & White <br>




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