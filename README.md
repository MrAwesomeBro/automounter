## Bypass an issue on automounting NFS drives on Debian

This scripot was written for an issue that NFS drives don't get automounted on debian 
servers from the */etc/fstab*. Even if the *mount -a* works and the drive does not get 
automounted on boot-up you will have to find an alternative. Use this.

## Usage

Copy the script to your wanted path (I suggest to use /opt/scripts) and add this line
to your */etc/rc.local*:

    /opt/scripts/automounter

Give the script the executive permissions:

    chmod +x /opt/scripts

Reboot and check *df -h*. That's it. Enjoy.
