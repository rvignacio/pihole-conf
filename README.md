# PiHole configuration

## Install on Ubuntu
1. Disable dns service
```
# systemctl disable systemd-resolved.service
# systemctl stop systemd-resolved.service
```
2. Add dns=default to `/etc/NetworkManager/NetworkManager.conf`
```
[main]
plugins=ifupdown,keyfile
dns=default
```
3. Restart network manager
```
# service network-manager restart
```

## Setup guide
https://www.smarthomebeginner.com/pi-hole-setup-guide/#Configuring_Your_Router_8211_Whole_Home_Ad_Blocking

## List
https://www.reddit.com/r/oisd_blocklist/comments/dwxgld/dbloisdnl_internets_1_domain_blocklist/
