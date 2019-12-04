## 4. Kernel

A linux kernel is responsible for handling Process management, Memory Management, Users, Inter process communication etc.

1. Kernel mounts the root file system as specified in the `root=` attribute in `grub.cnf` file. 
2. Check your grub configuration file by running following command

        $ cat /boot/grub/grub.cfg | grep root=

    ![Locate `root=` attribute in `grub.cfg`](../../image/15_grub_configuration_root.png)

3. The kernel image is a compressed image like **zImage** (compressed image, less than 512 KB) or **bzImage** (big compressed image, greater than 512 KB).
4. Can you find your kernel image? Check the `/boot/` folder

    ![Locate kernel image](../../image/16_kernel.png)