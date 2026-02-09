Hello, user!

This is **Linux Penguin 1.0**, a Linux-based OS by orca.pet3910YT!

Please make sure the computer you install this on is NOT one that is essential for anything because it will have data wiped on the selected disk, so don't make any mistake when typing the drive!

## Will this work on my machine?

Maybe. As of now, the installer has only been tested on a VirtualBox machine, so I can't be sure it will always work.

## Can I access the internet?

No. There is no internet driver on this OS.

## How do I make sure I can recover the OS after selecting the wrong drive?

Please **make a backup or installation media drive**. The OS is meant to be installed if you know what you're doing.

## Can I install this on real hardware or a server?

Technically, yes. Practically, please don't. The Linux kernel Penguin operates on is modified and has crash dump SysRq sequences fully enabled.

That means every user, malicious or no, might intentionally crash the OS and corrupt data, even by just connecting a keyboard and pressing SysRq c (lowercase C) or SysRq A (uppercase A).

## Wait, SysRq A?

Yes, SysRq A. The modified kernel has a new key assigned, which, as a joke, causes a kernel panic with the message "This PC is ass." Great if you want to laugh with a couple friends. Not if you're writing data.

## Ok, how do I install this then?

### Notes before installing

Please make sure your virtualization software or physical computer use an x86_64-compatible CPU. The installer, as well as OS use 64-bit binaries and kernel images. Also, make sure you use 64-bit UEFI (**not** IA32, **not** BIOS), as the image will be seen as unbootable otherwise.

### The install process

Use `grub-rescue` to build an ISO from the source, or use one of the releases I tagged (newest if possible).

Then, insert the ISO image into your virtualization software's CD-ROM drive. You can burn the image onto a real CD but... why?

You'll be prompted to read a warning. Press any key. Then type the /dev path to your hard disk, non-R/O optical media, tape drive, SD card (preferably not) or USB flash drive. Then press enter and again any key.

The install will take about 15 seconds (suprising, isn't it?). Later you'll be prompted for your root password. Don't worry if you don't see anything while typing - that's normal and intended for security in case people are looking (you never know!)

Then, before rebooting, make sure you see on the bottom of your screen "Emergency Sync complete". Then eject your CD and press Ctrl-Alt-Del to boot into your fresh install. Enjoy!
