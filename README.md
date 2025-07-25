## 1️⃣ Hapus Bot Lama (PM2)
```
pm2 stop botregis  
pm2 delete botregis  
pm2 unstartup  
pm2 save```

## 2️⃣ Hapus Folder Bot Lama
```
cd /root  
rm -rf bot-regis-script```

## 3️⃣ Upload ke /root via Termius 
```
cd /root  
unzip bot\ regis\ script.zip  
cd bot-regis-script```

## 4️⃣ Install Dependensi
```
npm install
```

## 5️⃣ Jalankan Bot
```
node bot.js```

## 🔁 pakai PM2: Agar bot tetep aktip
```npm install -g pm2  
pm2 start bot.js --name botregis  
pm2 save  
pm2 startup```
✅ Bot Kamu Aktif Kembali
