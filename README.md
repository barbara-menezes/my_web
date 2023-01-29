# my_web
Virtual Machines Administration

It started by installing a virtualization software, the one chose was the VirtualBox.
Download Archlinux’s ISO and Insert the Archlinux’s ISO in your VM’s drive and restart it.

Create the first VM with the values requested:


To verify the internet acess use the command 'ip a'.
Verify the disks using the command 'fdisk -l'.
And select the disk yoou want to do the partitioning with 'fdisk /dev/thenameofthedisk', you will be directed to the fdisk prompt.
Create a partition table, in my case I used the DOS one and it has up to 4 partitions available.
Then separete the partions as request, following the menu for help.


After, type the extensions using mkfs and mkswap.
Example: 
mkfs.ext4 /dev/sda1 (ext4 are just for partitions that are not bootable, in this case you can use ext2)
mkswap /dev/sda4 (then) swapon /dev/sda4


Nos, is time to mount the partition, remeber to that the “root” partition is always the first to be started.

