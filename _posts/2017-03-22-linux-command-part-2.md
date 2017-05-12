---
layout: post
title:  "Linux Command Part 2"
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
	
	Terminal is powerful hand.

</p></center>
<img  src="{{ site.url }}/assets/img/linux-terminal/Imitate-Fake-Hollywood-Terminal-Hacking-Melodrama-with-this-Amazing-App-for-Ubuntu-467788-3.jpg" alt="">

## List of Tips



✓ <a href="#afterthing">20 thing after install </a>

✓ <a href="#tfun">terminal fun </a>

✓ <a href="#music_t">play music from terminal </a>

✓ <a href="#monitor">process monitor </a>

✓ <a href="#tmux">Terminal Multiplexer</a>

✓ <a href="#sublime3">Sublime installation</a>

✓ <a href="#youtube-dl">download from youtube </a>

✓ <a href="#poweroff">power off linux </a>



<img src="{{ site.url }}/assets/img/linux-terminal/linux-mint-17-qiana-640x361.png" alt="">


## 20 thing install after install linux mint.

<h4 id="afterthing">fast and easy way</h4>
<em>because post is long compress content and download pdf (sorry)</em>
<a href="{{ site.url }}/assets/img/linux-terminal/binarytides_com.pdf">20thing</a>

<img src="{{ site.url }}/assets/img/linux-terminal/asciiview.png" alt="">


## How to funny work with terminal.

<h4 id="tfun">Fun</h4>

<em>for very funny in section nothing image</em>

<h4>sl - Steam Locomotive</h4>

With the sl command, a steam locomotive will run across your terminal from right to left

{% highlight javascript %}
	$ sudo apt-get install sl
{% endhighlight %}


<h4>cmatrix - The MATRIX</h4>

{% highlight javascript %}
	$ sudo apt-get install cmatrix
{% endhighlight %}

The command cmatrix draws the Neo style matrix on your terminal and makes you feel a little more geekier.

<em>very beautifully</em>

<h4>Watch Star Wars</h4>

This is not actually a command, but a text animation broadcasted at towel.blinkenlights.nl and can be played inside the terminal by telnetting to the server.

{% highlight javascript %}
	$ telnet towel.blinkenlights.nl
{% endhighlight %}


more information <a target="_blank" href="http://www.binarytides.com/linux-fun-commands/">binarytides.com</a>




<img src="{{ site.url }}/assets/img/linux-terminal/sound.png" alt="">


## How To Play Music From Command Line (Terminal)

<h4 id="music_t"><a target="_blank" href="https://en.wikipedia.org/wiki/Geek
">Geek</a> way</h4>


Most people like me prefer using Command Line in everyday life to Graphical User Interface (GUI) .

Today i`am going to show you how play music files from the Command Line using one of the best Command Line players (SoX) which supports most audio formats. Such as: <em>wav, mp3, mpg, mp3, ogg, flac, etc</em>.


<strong>SoX</strong> – Sound eXchange from the <em>$ man sox</em>  is described as , <em>the Swiss Army knife of audio manipulation</em>. 

Let’s get started, to install SoX:

1. Launch the terminal <em>(Ctrl + Alt +T)</em> type the command below and strike enter:

{% highlight javascript %}
	sudo apt-get install sox
{% endhighlight %}

After installation has been completed, run the command below to make SoX play .mp3 and other audio file formats.

{% highlight javascript %}
	sudo apt-get install sox libsox-fmt-all
{% endhighlight %}

To play all .mp3 files in any directory, change directory and use this command:

{% highlight javascript %}
	play *mp3
{% endhighlight %}

To play a specific file, type play file-name.extension (will play only this file)

{% highlight javascript %}
	play Aqua_Barbie_Girl.mp3 
{% endhighlight %}

To play next track Press <<em>Ctrl + c</<em> once and to stop or quit player, Press <<em>Ctrl</<em> and hit <<em>c</<em> twice.



<img src="{{ site.url }}/assets/img/linux-terminal/xtop.png.pagespeed.gp+jp+jw+pj+ws+js+rj+rp+rw+ri+cp+md.ic.b5G8p2Z1Tv.png" alt="">


## How to view your active processes in Terminal.

<h4 id="monitor">Power off Linux system</h4>

Type in the word top and you should see a nice list of processes and how much ram they are using.<br>

{% highlight javascript %}
	top	
{% endhighlight %}

<img src="{{ site.url }}/assets/img/linux-terminal/power-button.jpg" alt="">

## How to Shutdown ,reboot,halt linux system.

<h4 id="poweroff">Shutdown ,reboot,halt</h4>

<h3>1. shutdown command</h3>
<h4> Shutdown linux</h4>

To shutdown a machine call the shutdown command like this

{% highlight javascript %}
	# shutdown -h now

	or 

	# poweroff
{% endhighlight %}

The h option is for <em>halt</em> which means to stop. The second parameter is the time parameter. "now" means that shutdown the system right away.

The time parameter can be specified in minutes or hours also. For example

{% highlight javascript %}
	
	# shutdown -h +5 "Server is going down for upgrade. Please save your work."

{% endhighlight %}

<h4> Restart linux</h4>

The shutdown command can be used to restart a system with the r option instead of the h option. Usage is same as before. Just replace the h option with r option.

{% highlight javascript %}
	
	# shutdown -r +5 "Server will restart in 5 minutes. Please save your work."

{% endhighlight %}

All other logged in users will see a broadcast message in their terminal like this

{% highlight javascript %}
	
	[root@dhcppc1 ~]# 
	Broadcast message from root@dhcppc1
	        (/dev/tty1) at 21:35 ...

	The system is going down for reboot in 5 minutes!
	Server will restart in 5 minutes. Please save your work.
	At this point a shutdown can be cancelled by calling shutdown with "c" option.

{% endhighlight %}

{% highlight javascript %}
	
	# shutdown -c

{% endhighlight %}

<h3>2. reboot command</h3>

Next command is the reboot command. It can be used to shutdown or <em>reboot linux</em>.

The following command will <em>shutdown linux</em>.

{% highlight javascript %}
	
	# reboot -p

{% endhighlight %}

The "p" options stands for poweroff.

To <em>reboot linux</em> just call the reboot command directly without any options.

{% highlight javascript %}
	
	# reboot

{% endhighlight %}

This will perform a graceful shutdown and restart of the machine. This is what happens when you click restart from your menu.

Reboot linux forcibly
The following command will forcefully reboot the machine. This is similar to pressing the power button of the CPU. No shutdown takes place. The system will reset instantly.

{% highlight javascript %}
	
	# reboot -f

{% endhighlight %}

The man page explains it as follows

When called with --force or when in runlevel 0 or 6, this tool invokes the reboot(2) system call itself (with REBOOTCOMMAND argument passed) and directly reboots the system. Otherwise this simply invokes the shutdown(8) tool with the appropriate arguments without passing REBOOTCOMMAND argument.



<img src="{{ site.url }}/assets/img/linux-terminal/youtube-dl.png" alt="">


## How to Download Youtube Video

<h4 id="youtube-dl">Download from youtube</h4>

First you have to install youtube-dl with this command

Run

{% highlight javascript %}
	sudo apt-get install youtube-dl
	
	Or

	sudo pip install youtube-dl
{% endhighlight %}


to install command line mode downloader for YouTube. 
Then run

{% highlight javascript %}
	youtube-dl YouTube-(or-other-website)-video-link
{% endhighlight %}

once parameter very important is 

<em>-f</em>

<b>for example</b>

{% highlight javascript %}
	youtube-dl -f 18 YouTube-(or-other-website)-video-link
{% endhighlight %}


so it will download the video.


You can also take a look at <a target="_blank" href="https://github.com/rg3/youtube-dl/blob/master/README.md#readme">this</a> for very in-depth documentation on how to use it.


<img src="{{ site.url }}/assets/img/linux-terminal/terminator.png" alt="">


## How to Install tmux and Manage Multiple Linux Terminals(Terminal Multiplexer).

<h4 id="tmux">Install and Manage</h4>


{% highlight javascript %}
	$ sudo apt-get install tmux
{% endhighlight %}

<img src="{{ site.url }}/assets/img/linux-terminal/tmux_default.png" alt="">

<strong>Splitting tmux vertically</strong>

To split tmux vertically, just press <em>(Ctrl-b) + %</em> . Then the screen will be separated vertically.

<img src="{{ site.url }}/assets/img/linux-terminal/tmux_split_vertically.png" alt="">

<strong>Splitting tmux horizontally</strong>


To split tmux horizontally, press <em>(Ctrl-b) + “</em> . Then the sceen will be separated horizontally.

<img src="{{ site.url }}/assets/img/linux-terminal/tmux_split_vertically.png" alt="">

But of course we can mix them. Here’s another example.

<img src="{{ site.url }}/assets/img/linux-terminal/tmux_split_more.png" alt=""><br>

<h4>Moving between panes</h4>

Of course you will need move between panes. Otherwise, there is no use to create panes. By default, Linux console does not support mouse. So we need to know how to move between panes manually. There are some ways move between panes. Here’s a list how to to that.

→ <strong>Move Left</strong> : (Ctrl-b) + Left arrow <em>OR</em> (Ctrl-b) + {<br>
→ <strong>Move Right </strong>: (Ctrl-b) + Right arrow <em>OR</em> (Ctrl-b) + }<br>
→ <strong>Move Up</strong> : (Ctrl-b) + + Up arrow<br>
→ <strong>Move Down</strong> : (Ctrl-b) + Down arrow<br>
→ <strong>Move to the next pane</strong> : (Ctrl-b) + o<br>
→ <strong>Show number for each panes and press the number</strong> : (Ctrl-b) + b q + pane number. For example : (Ctrl-b) + b q + 1 will move you to pane number 1<br>

but find more information and tmux goto <a target="_blank" href="http://lukaszwrobel.pl/blog/tmux-tutorial-split-terminal-windows-easily">tmux Tutorial - Split Terminal Windows Easily</a>



<img src="{{ site.url }}/assets/img/linux-terminal/monokai_cobalt_for_sublime_text_by_felipetiza-d6yf31y.png" alt="">

## How to install sublime 3 [3083].

<h4 id="youtube-dl">Installation instructions:r</h4>


In order to successfully install Sublime Text 3 on Ubuntu 16.04 Xenial Xerus, Ubuntu 15.10 Wily Werewolf, Ubuntu 14.04 Trusty Tahr, Linux Mint 17.x, Elementary OS 0.3 Freya and other Ubuntu derivative systems, you have to add the PPA to your system, update the local repository index and install the sublime-text-installer:

{% highlight javascript %}
	
	$ sudo add-apt-repository ppa:webupd8team/sublime-text-3

	$ sudo apt-get update

	$ sudo apt-get install sublime-text-installer

{% endhighlight %}


Optional, to remove sublime text, do:

{% highlight javascript %}
	
	$ sudo apt-get remove sublime-text-installer

{% endhighlight %}


{% include content_option.html %}

<center>♥♥♥♥♥♥♥♥♥♥
<br><b>Please Gaming and give point for end of document your uderstand top linux command</b><br>
</center>
<hr>
<span>Draw back an arrow and launch it(center give point till 3 success launche)!</span>


{% include game_include.html %}