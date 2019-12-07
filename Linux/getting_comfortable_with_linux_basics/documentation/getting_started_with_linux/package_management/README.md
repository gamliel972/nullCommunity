## Package Management

On Linux, packages are downloaded and installed from online repositories by a package manager.

1. Advanced Packaging Tool (APT)

    The `APT` package, providing the `apt` command-line management tool.

    `apt` is a command which uses the advanced packaging tool to interact with the operating system’s package system.

    1. To update the database of available packages, i.e., to allow system to find if a newer version of software is available, run following command

            $ sudo apt update

    2. To upgrade the installed packages to their newer versions, run following command

            $ sudo apt upgrade -y

    3. To upgrade the system as a whole, i.e., to upgrade packages with auto-handling of dependencies which might involve removing currently installed packages if needed, run following command

            $ apt full-upgrade

    4. View all `apt` command line options

            $ apt -h

        ![apt help](../../image/getting_started_with_linux/6_apt_help.png)

2. Installing new packages

   1. From Ubuntu repository
   2. From .deb
   3. From .tar
   4. From PPA

3. Uninstalling packages

4. Purging packages

5. Removing dangling dependencies
