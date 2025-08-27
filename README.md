# Simple AutoScript V2Ray & Xray core
<p align="center">
  <a href="https://github.com/AxFrds/SakataScript" target="_blank" rel="noopener noreferrer" >
    <img src="https://raw.githubusercontent.com/AxFrds/SakataScript/master/screenshot/IMG_20250814_012044.jpg" alt="SakataScript screenshot" width="600" height="auto">
  </a>
</p>

### Installation
**First time to install**
```
apt-get update -y && apt-get upgrade -y && apt-get install wget -y
```

**Install / Update core**
```
wget -q https://raw.githubusercontent.com/AxFrds/SakataScript/master/setup && chmod +x setup && ./setup && rm -f setup
```

### Usage
- menu: Show panel menu

### Support OS
- Debian based (Debian/Ubuntu)
- RHEL based (AlmaLinux/Rocky Linux/CentOS/Fedora)
- openSUSE
- Recommended to use the latest OS version!

### Requirements
- x86_64 architecture
- KVM virtualization
- Root access server
- Valid domain name
- Valid Certificate SSL (put cert.crt & cert.key in /etc/xray/cert/)

### Features
- Vmess WS, gRPC & HTTPUpgrade
- Vless WS, gRPC & HTTPUpgrade
- Trojan WS, gRPC & HTTPUpgrade
- Shadowsocks WS, gRPC & HTTPUpgrade

### Port
- WS TLS: 443
- WS HTTP/NonTLS: 80
- gRPC: 443
- HTTPUpgrade: 443

### Core
- [V2Ray](https://github.com/v2fly/v2ray-core)
- [Xray](https://github.com/XTLS/Xray-core)

### Notes
- This script is FREE
- To register an IP, [contact me](https://t.me/AxFrds)
- V2Ray core does not support HTTPUpgrade
- Cannot add Shadowsocks client on V2Ray core, only support Xray core
