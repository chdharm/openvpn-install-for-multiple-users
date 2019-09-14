# OpenVPN Install for Multiple Users
Share the same client-certificate with everyone | Enabled duplicate-cn | Best for VPN startups
## Prerequisites
* Ubuntu 16.04 is no longer supported, use a latest version of OS
* Only works with Debian, Ubuntu or CentOS
* Enable 'tun' device before running this script
```
cat /dev/net/tun
cat: /dev/net/tun: File descriptor in bad state
```
* This script run on 'bash', not 'sh' for Debian users
```
echo {$BASH_VERSION}
```
* Run this as 'root'
```
sudo su
```

## Installation
Run this script
```
wget https://git.io/JeYgM -O openvpn-install.sh && bash openvpn-install.sh
```

## Remove
* Uninstall OpenVPN
```
sudo apt remove openvpn
```

* Remove it's dependencies
```
sudo rm -rfv /etc/openvpn
```
