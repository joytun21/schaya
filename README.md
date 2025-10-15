# 📖 AUTOSCRIPT V4.6

![Auto Script](https://raw.githubusercontent.com/joytun21/joy/main/image/VpnTunnel.jpg)

---

## 📱 Hubungi Saya

| Platform | Link |
|----------|------|
| Telegram Chat | [![Telegram-chat](https://img.shields.io/badge/Chat-Telegram-blue)](https://t.me/joyhayabuse/) |
| Telegram Grup | [![Telegram-grup](https://img.shields.io/badge/Grup-Telegram-blue)](https://t.me/+29-pKOGfLKwwYzI9) |
| Bot Telegram| [![Bot-Telegram](https://img.shields.io/badge/Telegram-Bot-green)](https://t.me/RegisAkses_bot/) |

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
```
## 💖 Dukung Pengembangan

Bantu saya terus kembangkan proyek ini agar tetap **gratis**, **stabil**, dan **berkembang lebih lanjut** 🚀  
Semua dukungan akan digunakan untuk biaya server, domain, dan pengembangan fitur baru.

| Platform Donasi | Link |
|------------------|------|
| Saweria | [![Saweria](https://img.shields.io/badge/Donasi-Saweria-orange?logo=buymeacoffee&logoColor=white)](https://saweria.co/Xtrimer) |

<p align="center">
  <img src="https://github.com/joytun21/joy/blob/main/image/ext.jpeg?raw=true" alt="QRIS Saweria" width="230" height="230">
</p>

> 💬 *Terima kasih banyak untuk setiap dukunganmu. Sedikit dari kamu sangat berarti untuk kelangsungan proyek ini!* 🙏
