# comms-web

Salinan statis halaman utama comms.ltd (disimpan dengan SingleFile, 27 Sep 2026), dipecah menjadi struktur repo:

```
index.html        # markup halaman
css/style.css     # semua <style> yang sebelumnya inline
assets/img/       # gambar hasil ekstraksi base64
assets/fonts/     # font Geist Sans / Geist Mono hasil ekstraksi base64
```

## Menjalankan

```bash
python -m http.server 8000
# atau
npx serve .
```

Lalu buka http://localhost:8000

## Catatan

- Snapshot hasil render: data live (nomor blok, daftar token, status wallet) adalah nilai statis saat halaman disimpan.
- JavaScript asli (Next.js) tidak ikut tersimpan, jadi interaksi seperti Connect Wallet, dropdown, dan drag pada globe tidak berfungsi.
