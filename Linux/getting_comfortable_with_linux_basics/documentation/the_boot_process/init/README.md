## 5. Init

After the kernel is booted and initialized, it calls first user-space application called as `init`. As it is the 1st program to be executed by Linux Kernel, hence, it has the process id (PID) of `1`. 

1. Check the process ID of `init`

        $ ps -ef | grep init

    ![`init` process](../../image/17_init_process.png)

2. Find out if your system is using `SysV`, `Upstart` or `Systemd` based *init*

        $ ps -p 1

    ![](../../image/21_processNameFromPID.png)

