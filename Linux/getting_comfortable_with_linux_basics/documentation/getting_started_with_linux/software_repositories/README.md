## Software Repositories

On Linux, software is distributed through software repositories. Sometimes, the default repository might not be sufficient, and we might have to add additional repositories to access additional functionality.

By default, repositories are stored into the `/etc/apt` folder.

1. See the default set of repositories configured for your distribution

        $ cat /etc/apt/sources.list | grep -v "#"

    ![Default repository](../../image/getting_started_with_linux/4_default_repository.png)

    Notice the use of the terms `main`, `restricted`, `universe`, and `multiverse`.

    * **Main** – officially supported, open-source software
    * **Restricted** – officially supported, closed-source software
    * **Universe** – community-maintained, open-source software
    * **Multiverse** – unsupported, closed-source and patent-encumbered software
    <br/>

2. View the contents of **sources.list.d** folder

        $ ll /etc/apt/sources.list.d/

    ![View sources.list.d folder contents](../../image/getting_started_with_linux/5_sourcesListD.png)

    *Note:* 
    * `sources.list.d` may contain *custom* APT repositories
    * New repositories could be added by putting a file with a unique name and the same format as `/etc/apt/sources.list` into the **folder** `/etc/apt/sources.list.d`.
    * Names of files in `/etc/sources.list.d` must end in `.list`
    <br/>

3. Add a custom APT repository
    
    * Run the following commands:

            $ sudo touch /etc/apt/sources.list.d/custom.list
            $ sudo nano /etc/apt/sources.list.d/custom.list

    * Now, add an entry for the custom repository: `deb https://packages.grafana.com/oss/deb stable main`
    * Import GPG keys, if you want to install packages securely

            $ sudo wget -q -O https://packages.grafana.com/gpg.key | sudo apt-key add

    * Update your APT cache in order for the changes to be applied

            $ sudo apt update