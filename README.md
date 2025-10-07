# AUTOSCRIPT V4.6

![Auto Script](https://raw.githubusercontent.com/joytun21/joy/main/image/VpnTunnel.jpg)

---

## 📱 Hubungi Saya

| Platform | Link |
|----------|------|
| Telegram Chat | [![Telegram-chat](https://img.shields.io/badge/Chat-Telegram-blue)](https://t.me/joyhayabuse/) |
| Telegram Grup | [![Telegram-grup](https://img.shields.io/badge/Grup-Telegram-blue)](https://t.me/+29-pKOGfLKwwYzI9) |
| WhatsApp Chat | [![WhatsApp-Chat](https://img.shields.io/badge/Chat-WhatsApp-green)](https://wa.me/62/) |

---

## 🖥 Tested OS

- **Debian:** 10 / 11 / 12 / 13  
- **Ubuntu:** 20 / 22 / 24 / 25  

---

## ⚡ Deskripsi

AUTOSCRIPT V4.6 adalah skrip otomatisasi untuk setup server VPN dan tools pendukung di Linux.  
Skrip ini dirancang agar **mudah digunakan**, **cepat diinstal**, dan **stabil di berbagai versi Debian & Ubuntu**.  

---

## 🛠 Fitur

- Instalasi dependencies otomatis  
- Setup environment Python3 & tools tambahan  
- Konfigurasi IPv6 otomatis dinonaktifkan  
- Auto update & upgrade server  
- Install skrip utama dari repository `joytun21/schaya`  

---

## 📝 Instalasi (via WGET)

Jalankan perintah berikut di terminal server Anda:

```bash
sysctl -w net.ipv6.conf.all.disable_ipv6=1 && \
sysctl -w net.ipv6.conf.default.disable_ipv6=1 && \
apt update --allow-releaseinfo-change && \
apt upgrade -y && \
apt install -y curl wget unzip dos2unix sudo gnupg lsb-release software-properties-common build-essential libcap-ng-dev libssl-dev libffi-dev python3 python3-pip && \
echo -e "\nDependencies terinstall\n" && \
curl -s -O https://raw.githubusercontent.com/joytun21/schaya/main/mahbub && \
chmod +x mahbub && \
./mahbub
