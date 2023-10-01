# Basic Terminologies

#### What is a kernel? <a href="#what-is-a-kernel" id="what-is-a-kernel"></a>

A **kernel** is a part of an OS that facilitates interactions between the hardware and software. It's an essential element of an operating system for a computer.

The core of the OS alone is responsible for providing all other components with necessary services. It helps with device control, networking, file system management, process and memory management, and it acts as the main interface between the OS and the hardware.

<figure><img src="https://www.freecodecamp.org/news/content/images/2022/09/image-11-1.png" alt="image-11-1" height="400" width="600"><figcaption><p><a href="https://d1m75rqqgidzqn.cloudfront.net/wp-data/2022/08/04135248/image-11.png">kernel</a></p></figcaption></figure>

#### What is a Shell? <a href="#what-is-a-shell" id="what-is-a-shell"></a>

A shell is a computer interface to an operating system. The shell exposes the services of the OS to users or other programs. The shell takes your commands and gives them to the OS so it can perform them.

It's named a shell because its the outer layer around the OS – like the shell around an oyster!

#### What is the Terminal? <a href="#what-is-the-terminal" id="what-is-the-terminal"></a>

A terminal is a program that runs a shell. This is where we run most of our commands that tell the OS what to do.

You install the terminal in the following ways on different operating systems:

* **Linux Distro users** – the Bash shell is installed by default
* **Mac Users** – Terminal is installed by default and can execute similar Linux commands
* **Windows Users** – Download [Windows Subsystem for Linux (WSL)](https://www.freecodecamp.org/news/how-to-install-wsl2-windows-subsystem-for-linux-2-on-windows-10/) or use `git bash` and run all Linux command from there.

### What are Linux Distributions? <a href="#what-are-linux-distributions" id="what-are-linux-distributions"></a>

Linux distributions (popularly called **distros)** are flavors of the Linux operating system. These distros are built based on Linux's open source software.

Some examples of these are:

#### Debian Family <a href="#debian-family" id="debian-family"></a>

Since it was founded in 1993, Debian has released new versions far more slowly than Ubuntu and mint. It is one of the most reliable Linux distributors as a result.

Debian is the foundation of Ubuntu, which was created to expeditiously enhance Debian's fundamental components and make it more user-friendly.

Ubuntu was created by Canonical in 2004 and gained popularity immediately. Canonical wants Ubuntu to be used as a simple, command-line-free graphical Linux desktop. It's the most well-known Linux distribution.

Ubuntu is simple for beginners to use. It has a large number of pre-installed applications and convenient repository libraries.

#### Red Hat Family <a href="#red-hat-family" id="red-hat-family"></a>

Red Hat is a professional Linux distributor. Red Hat Enterprise Linux (RHEL) and Fedora are their products, both of which are open source.

Fedora offers faster updates and no support, but RHEL is thoroughly tested before release and supported for seven years after the release.

Red Hat uses trademark law to stop the redistribution of its software. Red Hat Enterprise Linux source is used in CentOS, a community effort that eliminates all of Red Hat's trademarks and makes it publicly available. In other words, it is a free version of RHEL and offers a long-lasting reliable platform.

#### SUSE Family <a href="#suse-family" id="suse-family"></a>

SUSE created its own operating system for computers. It is supplied with system and application software from other open source projects and is developed on top of the free and open source Linux kernel.

SUSE Linux was primarily developed in Europe and is of German origin. The name SUSE is an acronym for "Software und System-Entwicklung." SUSE is one of the oldest commercial distributions still in use because the initial version debuted in early 1994.

#### Fedora Family <a href="#fedora-family" id="fedora-family"></a>

This is a project that offers the most recent software versions and mostly focuses on free software. It uses 'upstream' applications instead of developing its own desktop environment. It comes with the GNOME3 desktop environment by default. Although less reliable, it offers the newest information.

### How to Choose a Linux Distribution <a href="#how-to-choose-a-linux-distribution" id="how-to-choose-a-linux-distribution"></a>

| DISTRIBUTION       | REASON TO USE                                               |
| ------------------ | ----------------------------------------------------------- |
| Ubuntu             | It works like Mac OS and easy to use.                       |
| CentOS             | If you want to use red hat but without its trademark.       |
| Fedora             | If you want to use red hat and latest software.             |
| Red hat enterprise | Used commercially.                                          |
| OpenSUSE           | It works same as Fedora but slightly older and more stable. |
| Arch Linux         | It is not beginner friendly.                                |

Now let's talk about some commands you can run to interact with the shell.
