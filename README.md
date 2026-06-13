# 📖 AUTOSCRIPT V4.6

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
apt install -y curl wget unzip sudo gnupg lsb-release build-essential libcap-ng-dev libssl-dev libffi-dev python3 python3-pip && \
curl -fsSL -O https://raw.githubusercontent.com/joytun21/schaya/main/mahbub && \
chmod +x mahbub && \
./mahbub
```
## 📈 Kernel News
```
sed -i '/fs.file-max/d; /net.core.default_qdisc/d; /net.ipv4.tcp_congestion_control/d' /etc/sysctl.conf
cat << 'EOF' >> /etc/sysctl.conf

# Optimasi batasan file dan antrean network
fs.file-max = 2097152
net.core.netdev_max_backlog = 250000
net.core.somaxconn = 65535

# Memperlebar Buffer RAM untuk Kirim/Terima Paket Data (Anti-Lemes)
net.core.rmem_default = 262144
net.core.wmem_default = 262144
net.core.rmem_max = 67108864
net.core.wmem_max = 67108864

# Optimasi Alokasi Memory TCP (Min, Default, Max)
net.ipv4.tcp_rmem = 4096 87380 67108864
net.ipv4.tcp_wmem = 4096 65536 67108864

# Mempercepat pembersihan koneksi yang menggantung (Time-Wait)
net.ipv4.tcp_fin_timeout = 15
net.ipv4.tcp_tw_reuse = 1
net.ipv4.tcp_max_syn_backlog = 65535
net.ipv4.tcp_max_tw_buckets = 2000000

# Mengaktifkan BBR dan Fast Open untuk menekan Ping
net.core.default_qdisc = fq
net.ipv4.tcp_congestion_control = bbr
net.ipv4.tcp_fastopen = 3
EOF

sysctl -p && ulimit -n 65535
```
## 📲 Prioritas IP4
```
sed -i 's/#precedence ::ffff:0:0\/96  100/precedence ::ffff:0:0\/96  100/' /etc/gai.conf
```
## ⚖️ MSG Deb-13
```
sed -i '/mesg n/d' ~/.bashrc ~/.profile 2>/dev/null
```
## 💎 DNS PING
```
echo "nameserver 1.1.1.1" > /etc/resolv.conf
bash -c 'echo -e "[Resolve]\nDNS=1.1.1.1" > /etc/systemd/resolved.conf && systemctl enable systemd-resolved'
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
