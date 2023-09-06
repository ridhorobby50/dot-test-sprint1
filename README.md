# Dot Test Sprint 1

Aplikasi ini dibuat untuk tujuan test DOT PHP Developer dan untuk soal Sprint 1, Lakukan langkah dibawah untuk menginstal aplikasi


## Instalasi
- Pastikan anda telah membuat database untuk menampung data migration dari Laravel
- Copy isi dari .env.example dan buatlah file .env. Pastekan isi dari .env.example ke file .env yang baru dibuat
- Ubah Detail pada env dari DB_HOST sampai DB_PASSWORD sesuai environtment pada perangkat anda
- Pastikan juga terdapat env URL_API dan TOKEN_RAJAONGKIR dengan value yang sesuai tertera pada soal.URL_API bervalue 'https://api.rajaongkir.com/starter/'
- Setelah selesai, lakukan composer install untuk menginstall third party dan dependecies yang dibutuhkan.
- Selanjutnya jalankan perintah 'php artisan init:sprint1' (tanpa tanda petik) untuk menjalankan migrasi dan sinkronisasi data province dan city dari Rajaongkir.
- Maka, table akan otomatis tercreate dan terisi data province dan city dari data RajaOngkir.
- Jalankan aplikasi menggunakan php artisan serve.
- Lakukan akses percobaan dengan endpoint {HOST}/api/v1/search/provinces untuk melakukan pencarian provinsi, tambahkan ?id={province_id} untuk mencari spesifik 1 data berdasarkan id province, contoh : localhost:8000/api/v1/search/provinces?id=1
- Lakukan akses percobaan dengan endpoint {HOST}/api/v1/search/cities?id={city_id}  untuk melakukan pencarian city, tambahkan ?id={city_id} untuk mencari spesifik 1 data berdasarkan id city, contoh : localhost:8000/api/v1/search/cities?id=1