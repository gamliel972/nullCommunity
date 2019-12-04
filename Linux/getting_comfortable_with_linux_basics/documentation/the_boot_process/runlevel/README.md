## 6. Runlevel

A run level is an operating system **state** on Linux system. There are seven runlevels, numbered from `0` to `6`. A system can be booted into any of the given runlevel.

Each runlevel designates a different system configuration and allows access to a different combination of processes. By default Linux boots either on runlevel 3 or runlevel 5.

As soon as the kernel executes the init process, it will look at the `/etc/inittab` configuration file to see the default run level.

