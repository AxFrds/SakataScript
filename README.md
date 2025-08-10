# Simple AutoScript V2Ray & Xray core

### Installation
First time to install
```
apt-get update -y && apt-get upgrade -y && apt-get install wget -y
```

Install / Update core
```
wget -q https://raw.githubusercontent.com/AxFrds/AutoScript-V2RAY-XRAY/master/setup.sh && chmod +x setup.sh && ./setup.sh && rm -f setup.sh
```

### Supports OS
Tested
- Ubuntu 24.04
- Debian 12

### Features
- Vmess WS & gRPC
- Vless WS & gRPC
- Trojan WS & gRPC
- Shadowsocks WS & gRPC

### Port
- WS TLS: 443
- WS HTTP/NonTLS: 80
- gRPC: 443

### Core
- [V2Ray](https://github.com/v2fly/v2ray-core)
- [Xray](https://github.com/XTLS/Xray-core)

### Notes
- This script is FREE
- To register an IP, [contact me](https://t.me/AxFrds)
- Cannot add Shadowsocks client on V2Ray core, only support Xray core
