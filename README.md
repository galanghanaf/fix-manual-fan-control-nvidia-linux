# Fix Manual Fan Control Nvidia on Linux
## Ubuntu 22.04
```
sudo vim /etc/X11/Xwrapper.config

Add these lines before allowed_users=console:
needs_root_rights=yes

Save file
Reboot
```
## Fedora 35 Workstation
```
Fedora installer does not create Xwrapper.config

sudo vim /etc/X11/Xwrapper.config

Add these two lines:
needs_root_rights=yes
allowed_users=console

Save file
Reboot
```
