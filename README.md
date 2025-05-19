

# Absensi Wajah (Face Attendance App)

Aplikasi berbasis web untuk pencatatan kehadiran menggunakan pengenalan wajah (face recognition). Dibuat dengan Python (Flask), menggunakan file JSON sebagai penyimpanan data pengguna dan kehadiran.

🎯 Fitur Utama

* Tambah pengguna dengan nama dan foto manual (CRUD).
* Monitoring kehadiran lengkap dengan hari dan jam kehadiran.
* UI modern dan responsif (seperti Blynk) menggunakan Bootstrap 5.
* Dashboard interaktif dengan tampilan pengguna dalam bentuk kartu.
* Penyimpanan data kehadiran dan pengguna dalam file JSON.

🖼️ Tampilan UI

* Navbar modern berwarna gradien biru.
* Tampilan pengguna berupa kartu (card) dengan gambar.
* Tabel monitoring kehadiran yang rapi dan interaktif.
* Form input modern untuk tambah pengguna baru.

📦 Struktur Folder

```
.
├── app.py
├── data
│   ├── users.json         # Data pengguna
│   └── attendance.json    # Data kehadiran
├── static
│   └── uploads/           # Folder foto pengguna
├── templates
│   ├── layout.html        # Template dasar dengan Bootstrap
│   ├── users.html         # Halaman daftar pengguna
│   ├── add_user.html      # Form tambah pengguna
│   └── monitor.html       # Monitoring kehadiran
└── README.md
```

🚀 Cara Menjalankan Aplikasi

1. Pastikan kamu sudah install Python 3.10+ dan pip.
2. Install dependency:

```bash
pip install flask
```

3. Jalankan aplikasi:

```bash
python app.py
```

4. Buka di browser:

```
http://127.0.0.1:5000
```

📤 Menambahkan Pengguna

* Klik tombol “+ Tambah User” di halaman /users
* Masukkan nama dan upload foto wajah
* Foto akan disimpan ke folder /static/uploads/
* Data nama akan disimpan di data/users.json

📊 Monitoring Kehadiran

* Halaman monitoring dapat diakses di /monitor
* Data hadir disimpan dalam data/attendance.json
* Format data:

```json
{
  "name": "Ludang",
  "day": "Senin",
  "timestamp": "2025-05-11 09:10:32"
}
```

🧠 Teknologi yang Digunakan

* Python + Flask
* HTML + CSS (Bootstrap 5)
* JSON untuk penyimpanan
* Frontend responsif dan mobile-friendly

🛠️ Catatan Tambahan

* Proyek ini masih menggunakan penyimpanan lokal (bukan database)
* Gunakan di jaringan lokal atau integrasikan dengan OpenCV untuk absensi otomatis
* Pastikan folder /data dan /static/uploads memiliki izin write

📄 Lisensi

Proyek ini bebas digunakan untuk keperluan edukasi dan non-komersial.

👤 Dibuat oleh: Nugra21

—

Jika kamu ingin saya bantu upload awal dan commit awal ke GitHub, beri tahu juga apakah kamu ingin file zip atau petunjuk git init & push pertama kali. Mau saya bantu buatkan .gitignore juga?
