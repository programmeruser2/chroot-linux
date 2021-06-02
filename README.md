# chroot-linux
Install and manage Linux inside a chroot.
# Installation
```bash
sudo curl -fsSL https://github.com/programmeruser2/chroot-linux/raw/main/chroot-linux > /usr/local/bin/chroot-linux
chmod +x /usr/local/bin/chroot-linux 
```
# FAQ
## Where are the chroots stored?
In `/var/lib/chroot-linux`.
## Why isn't DNS resolving working?
This is likely because your `/etc/resolv.conf` file is not configured. You can copy this from your host:
```bash
sudo cp /etc/resolv.conf /var/lib/chroot-linux/chrootname/etc/resolv.conf
``` 
