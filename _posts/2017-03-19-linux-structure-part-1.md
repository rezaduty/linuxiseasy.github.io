---
layout: post
title:  "Linux Structure Part 1"
image: ''
date:  2017-03-15  01-45-39
tags:
- linux
- what is linux
- linux structure
- linux file system
- Kernel
description: ''
categories:
- Linux
- Linux Structure
---

<center><p>
	Linux is one of popular version of UNIX operating System. It is open source as its source code is freely available. It is free to use. Linux was designed considering UNIX compatibility. Its functionality list is quite similar to that of UNIX.
</p></center>
<img src="{{ "/assets/img/linux-structure/20161010142555_Linux-ANGRY.png"}}" alt="">

## Components of Linux System
 
Linux Operating System has primarily three components

→ <strong>Kernel</strong> − Kernel is the core part of Linux. It is responsible for all major activities of this operating system. It consists of various modules and it interacts directly with the underlying hardware. Kernel provides the required abstraction to hide low level hardware details to system or application programs.

→ <strong>System Library</strong> − System libraries are special functions or programs using which application programs or system utilities accesses Kernel's features. These libraries implement most of the functionalities of the operating system and do not requires kernel module's code access rights.

→ <strong>System Utility</strong> − System Utility programs are responsible to do specialized, individual level tasks.

<img src="{{ "/assets/img/linux-structure/linux_os.jpg"}}" alt="">

## Kernel Mode vs User Mode

Kernel component code executes in a special privileged mode called <strong>kernel mode</strong> with full access to all resources of the computer. This code represents a single process, executes in single address space and do not require any context switch and hence is very efficient and fast. Kernel runs each processes and provides system services to processes, provides protected access to hardware to processes.

Support code which is not required to run in <strong>kernel</strong> mode is in System Library. User programs and other system programs works in User Mode which has no access to system hardware and kernel code. User programs/ utilities use System libraries to access Kernel functions to get system's low level tasks.


## Basic Features

Following are some of the important features of Linux Operating System.

→ <strong>Portable</strong> − Portability means software can works on different types of hardware in same way. Linux kernel and application programs supports their installation on any kind of hardware platform.

→ <strong>Open Source</strong> − Linux source code is freely available and it is community based development project. Multiple teams work in collaboration to enhance the capability of Linux operating system and it is continuously evolving.

→ <strong>Multi-User</strong> − Linux is a multiuser system means multiple users can access system resources like memory/ ram/ application programs at same time.

<strong>Multiprogramming</strong> − Linux is a multiprogramming system means multiple applications can run at same time.

→ <strong>Hierarchical File System</strong> − Linux provides a standard file structure in which system files/ user files are arranged.

→ <strong>Shell</strong> − Linux provides a special interpreter program which can be used to execute commands of the operating system. It can be used to do various types of operations, call application programs. etc.

→ <strong>Security</strong> − Linux provides user security using authentication features like password protection/ controlled access to specific files/ encryption of data.


##Architecture

The following illustration shows the architecture of a Linux system


<img src="{{ "/assets/img/linux-structure/linux_architecture.jpg"}}" alt="">


The architecture of a Linux System consists of the following layers −

→ <strong>Hardware layer</strong> − Hardware consists of all peripheral devices (RAM/ HDD/ CPU etc).

→ <strong>Kernel</strong> − It is the core component of Operating System, interacts directly with hardware, provides low level services to upper layer components.

→ <strong>Shell</strong> − An interface to kernel, hiding complexity of kernel's functions from users. The shell takes commands from the user and executes kernel's functions.

→ <strong>Utilities</strong> − Utility programs that provide the user most of the functionalities of an operating systems.

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