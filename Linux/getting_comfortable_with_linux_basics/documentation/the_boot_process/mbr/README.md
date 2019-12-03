## 2. Master Boot Record (MBR)

Master Boot Record (MBR) loads and executes the GRUB boot loader

![GRUB](../../image/6_gnu_grub.png)

* MBR is located in the 1st sector of the bootable disk. Typically `/dev/hda`, or `/dev/sda`
* This is the location that contains the program that will help our computer to load the operating system