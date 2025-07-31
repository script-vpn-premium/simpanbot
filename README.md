Bot Regis Script vps - Panduan Instalasi
Panduan lengkap untuk menghapus versi lama dan mengaktifkan bot baru menggunakan PM2.
---

1️⃣ Hapus Bot Lama
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
🔁 Pakai PM2 Agar Selalu Aktif
```bash
npm install -g pm2  
pm2 start bot.js --name botregis  
pm2 save  
pm2 startup
```
✅ Bot Sekarang Aktif dan
---
✅ Siap Digunakan!
---

# 🤖 SimpleBot WhatsApp - Create Akun VPN Otomatis

Bot WhatsApp berbasis **Baileys** yang digunakan untuk membuat akun VPN secara otomatis via WhatsApp. Mendukung akun:

- VLESS
- VMess
- Trojan
- SSH

---

## 📦 Fitur

✅ Perintah lewat WhatsApp  
✅ Link VPN + akun premium  
✅ Hanya admin tertentu yang bisa pakai  
✅ Bisa jalan terus di VPS (PM2)  

---

## 🛠 Persiapan VPS

Langkah Menjalankan SimpleBot  Wa di VPS

🛠 Persiapan VPS:
 
1
```bash
sudo apt update
sudo apt install nodejs npm -y
```

2. Upload file ke VPS atau clone dari 
Git jika ada. Jika kamu upload file 
ZIP, ekstrak di VPS:

```bash
unzip Simplebot.zip
cd Simplebot
```

3. Install dependensi:
```bash
npm install
```
4. Jalankan bot:
```bash
node index.js
```
Jika index.js membutuhkan login WhatsApp
(misalnya pakai Baileys),

---
✅ Tips Tambahan:

Untuk menjaga bot tetap aktif, gunakan pm2:
```bash
sudo npm install -g pm2
pm2 start index.js --name simplebot
pm2 save
pm2 startup
```


Hapus bot lama
```bash
pm2 delete simplebot && rm -rf /root/Simplebot && pm2 save && echo "✅ Bot simplebot berhasil dihapus dari PM2 dan folder /root/Simplebot dihapus."
```
Untuk mengedit pengaturan, buka settings.js 
dan sesuaikan token, owner, dll.


