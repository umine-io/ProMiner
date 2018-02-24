# ProMiner

## How to start up the machine and mining.


## Default account settings

The default user is `umine`, and password is `novotech`. `root` user is not setup, but you can use sudo command instead.

## How to enter R/W mode on U mine system (base on Ubuntu 16.04)

This system by default has a ram overlay filesystem on top of ext4. Your writes will be lost if rebooted. You need to do the following step to disable protection temporarily.

Startup the machine, the boot menu should be like this.

![Image](images/syspro1.jpg)

The first item is protected mode, the second one is unprotected writable mode. You can do write operation on system partition by booting from this item until shutdown. Notice that in this mode system will not be protected from power failure, you should do normal shutting down, by using poweroff command or power off button on GUI.

## How to detect the protection mode on the system

When root partition (/) is mounted on /dev/sda2, the system is on writable (unprotected) mode. In this mode, you should do normal shutdown process to prevent data loss.

![Image](images/syspro2.jpg)

When root partition is mounted on overlayroot, the system is on read-only (protected) mode.

![Image](images/syspro3.jpg)
