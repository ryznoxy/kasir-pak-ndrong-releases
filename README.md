# Kasir Pak Ndrong — Rilis APK

Repo ini hanya menampung **file APK rilis** aplikasi Kasir Pak Ndrong.
Kode sumber ada di repo privat terpisah.

## Cara memasang

1. Buka tab **Releases** di repo ini.
2. Unduh file `.apk` pada rilis terbaru.
3. Buka file tersebut di HP Android, izinkan "instal dari sumber tidak dikenal" bila diminta.
4. Data kasir yang sudah ada **tidak terhapus** saat pembaruan.

Aplikasi juga menampilkan notifikasi versi baru di layar Kasir, lengkap dengan tombol Unduh.

## Untuk pengembang

```bash
eas build -p android --profile preview
gh release create v1.1.0 kasir-pak-ndrong-v1.1.0.apk \
  --repo ryznoxy/kasir-pak-ndrong-releases \
  --title "Kasir Pak Ndrong v1.1.0" \
  --notes "Perbaikan dan fitur baru."
```

Nomor versi pada tag **harus** sama dengan `version` di `app.json` milik repo sumber,
karena aplikasi membandingkan tag rilis dengan versi yang terpasang.
