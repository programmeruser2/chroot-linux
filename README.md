> This project isn't in active development nor is it out of alpha. This was made as an experiment and probably will always remain as one. Please don't use this in production. Pull requests and issues are still welcome though.
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
