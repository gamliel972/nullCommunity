## 5. Init

After the kernel is booted and initialized, it calls first user-space application called as `init`. Kernel executes the `/sbin/init` program. 

As it is the 1st program to be executed by Linux Kernel, hence, it has the process id (PID) of `1`. 

* Run the following command to check the process ID of `init`

        $ ps -ef | grep init

    ![`init` process](../../image/17_init_process.png)
