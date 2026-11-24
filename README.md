# DENZZMODZ Admin Panel
Starter Node.js/Express bertema ungu dengan login Access Key, dashboard, pengelolaan subscription/account, dan toggle status maintenance.

## Jalankan
1. Gunakan Node.js 20+.
2. `npm install`
3. Set environment variables `ADMIN_ACCESS_KEY` (acak, minimal 16 karakter) dan `SESSION_SECRET` (acak, minimal 32 karakter).
4. `npm start`, lalu buka port 3000.

## Deploy Railway
Upload repository ini ke GitHub lalu deploy sebagai service Railway. Tambahkan `ADMIN_ACCESS_KEY`, `SESSION_SECRET`, dan `NODE_ENV=production` pada Variables. Tambahkan Railway Volume dan set `DATA_DIR=/data` agar data JSON bertahan saat redeploy.

## Penting
- Jangan simpan Access Key atau SESSION_SECRET di source code.
- Express MemoryStore session bawaan hanya cocok untuk starter/testing; ganti dengan session store persisten sebelum penggunaan produksi serius.
- Toggle maintenance saat ini hanya menyimpan status pada dashboard, belum memblokir situs publik.
- Data disimpan sebagai JSON; untuk penggunaan besar gunakan database.
- Ini website baru; tidak mengubah deployment CHIKO H4X dan tidak menyalin backend/database lamanya.
