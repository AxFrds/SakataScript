# SakataScript

<p align="center">
  <a href="https://github.com/AxFrds/SakataScript" target="_blank" rel="noopener noreferrer">
    <img src="https://raw.githubusercontent.com/AxFrds/SakataScript/refs/heads/master/screenshot/1781121164310.jpg" alt="SakataScript preview" width="600">
  </a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/platform-Linux-blue" alt="Platform">
  <img src="https://img.shields.io/badge/architecture-x86__64-lightgrey" alt="Architecture">
  <img src="https://img.shields.io/badge/core-V2Ray%20%7C%20Xray-green" alt="Core">
  <img src="https://img.shields.io/badge/protocol-VMess%20%7C%20VLESS%20%7C%20Trojan%20%7C%20Shadowsocks-orange" alt="Protocols">
</p>

**SakataScript** is a simple Linux VPS autoscript for installing and managing **V2Ray** and **Xray** services through a terminal-based menu panel.

It supports VMess, VLESS, Trojan, and Shadowsocks accounts over WebSocket, gRPC, and HTTPUpgrade transports.

---

## Features

- Terminal-based management panel with the `menu` command
- V2Ray and Xray core support
- VMess account management
- VLESS account management
- Trojan account management
- Shadowsocks account management
- WebSocket, gRPC, and HTTPUpgrade transport support
- Nginx reverse proxy configuration
- Automatic service restart from the panel
- Multi-distro Linux support

---

## Supported Operating Systems

| Family | Distribution |
|---|---|
| Debian-based | Debian, Ubuntu |
| RHEL-based | CentOS, Fedora, AlmaLinux, Rocky Linux |
| SUSE-based | openSUSE |

> Using the latest stable OS release is recommended.

---

## Requirements

Before installation, make sure your VPS meets these requirements:

- x86_64 architecture
- KVM virtualization
- Root access
- Registered server IP
- Valid domain name
- Valid SSL certificate files:
  - `/etc/xray/cert/cert.crt`
  - `/etc/xray/cert/cert.key`

To register an IP, contact: [@AxFrds](https://t.me/AxFrds)

---

## Installation

### Debian / Ubuntu

```bash
apt-get update -y && apt-get upgrade -y && apt-get install wget -y
```

### CentOS / Fedora / AlmaLinux / Rocky Linux

```bash
yum upgrade -y && yum install wget -y
```

### openSUSE

```bash
zypper refresh && zypper update -y && zypper install -y wget
```

### Install or Update SakataScript

```bash
wget -q https://raw.githubusercontent.com/AxFrds/SakataScript/master/setup && chmod +x setup && ./setup && rm -f setup
```

---

## Usage

Run the panel menu:

```bash
menu
```

The panel provides access to account creation, account deletion, account listing, core switching, domain switching, log cleanup, service restart, and uninstall options.

---

## Supported Protocols

| Protocol | WebSocket | gRPC | HTTPUpgrade |
|---|---:|---:|---:|
| VMess | Yes | Yes | Yes |
| VLESS | Yes | Yes | Yes |
| Trojan | Yes | Yes | Yes |
| Shadowsocks | Yes | Yes | Yes |

---

## Ports

| Transport | Port |
|---|---:|
| WebSocket TLS | 443 |
| WebSocket HTTP / Non-TLS | 80 |
| HTTPUpgrade TLS | 443 |
| HTTPUpgrade HTTP / Non-TLS | 80 |
| gRPC TLS only | 443 |

---

## Logs

Generated account information is saved in:

```text
/etc/log-create-vmess.log
/etc/log-create-vless.log
/etc/log-create-trojan.log
/etc/log-create-shadowsocks.log
```

---

## Core Projects

SakataScript uses the following upstream core projects:

- [V2Ray Core](https://github.com/v2fly/v2ray-core)
- [Xray Core](https://github.com/XTLS/Xray-core)

---

## Important Notes

- This script is free to use.
- V2Ray core does not support HTTPUpgrade.
- Shadowsocks account creation is only supported on Xray core.
- Make sure your domain already points to your VPS IP before installation.
- Make sure your SSL certificate files are placed correctly before using TLS services.

---

## Disclaimer

This project is provided as-is. Use it responsibly and make sure you comply with the laws, rules, and policies that apply in your country, hosting provider, and network environment.
