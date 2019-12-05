## 6. Runlevel

`systemd` takes over and continues to mount the host’s file systems and start services.

As soon as the kernel executes the init process, it will look at the configuration files to see the default run level.

A runlevel is a single-byte name for a particular system configuration. Runlevels for Debian and Ubuntu systems are generally as follows:

0 : System halt.
1 : Single-User mode.
2 : Graphical multi-user plus networking (DEFAULT)
3 : Same as "2", but not used.
4 : Same as "2", but not used.
5 : Same as "2", but not used.
6 : System reboot.
There are also a few pseudo-runlevels:

N : The previous runlevel cannot be determined.
S : Alias for Single-User mode.