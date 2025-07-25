🚀 Bot Regis Script vps - Panduan Instalasi
Panduan lengkap untuk menghapus versi lama dan mengaktifkan bot baru menggunakan PM2.

---

1️⃣ Hapus Bot Lama (Jika Sebelumnya Pakai PM2)
```bash
pm2 stop botregis  
pm2 delete botregis  
pm2 unstartup  
pm2 save
```

---

2️⃣ Hapus Folder Bot Lama
```bash
cd /root  
rm -rf bot-regis-script
```

---

3️⃣ Upload File Bot Baru via Termius
Pindahkan file ZIP ke direktori `/root`, lalu:
```bash
cd /root  
unzip bot\ regis\ script.zip  
cd bot-regis-script
```

---

4️⃣ Install Dependensi
```bash
npm install
```

---

5️⃣ Jalankan Bot (Tanpa PM2)
```bash
node bot.js
```

---

🔁 Jalankan Bot Pakai PM2 (Agar Selalu Aktif)
```bash
npm install -g pm2  
pm2 start bot.js --name botregis  
pm2 save  
pm2 startup
```

Bot Kamu Sekarang Aktif dan Siap Digunakan!
