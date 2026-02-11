# Backend - AstroSyncs (Java)
Dokumentasi struktur folder, aturan penamaan, dan aturan kerja tim untuk backend AstroSyncs.

---

## Struktur Folder Backend (Java)
Semua file Java wajib berada di:

```txt
src/com/kontra/astrosyncs
```

---

## 1) Pembagian Folder

com.kontra.astrosyncs                                               <br>
│                                                                   <br>
├── config/          # konfigurasi (CORS, scheduler, security)      <br>
├── controller/      # endpoint REST API                            <br>
├── dto/             # request/response object                      <br>
│   ├── request/                                                    <br>
│   └── response/                                                   <br>
├── entity/          # class model (tabel database)                 <br>
├── enums/           # enum (Role, Status, dll)                     <br>
├── repository/      # akses database (JPA Repository)              <br>
├── service/         # business logic utama                         <br>
├── util/            # helper kecil (converter, time helper)        <br>
└── exception/       # custom error & handler                       <br>

---

## 2) Aturan Penamaan File
Semua file Java wajib pakai prefix:                                 <br> &nbsp;&nbsp;&nbsp;&nbsp;
    Kontra_

Contoh:                                                             <br> &nbsp;&nbsp;&nbsp;&nbsp;
    Kontra_User.java

Ini wajib supaya konsisten dan mudah dicari (Biar keren 🥶☠️).

---

## 3) Maksimal 200 Baris per File
Setiap file usahakan maksimal 200 baris.                            <br>
Kalau lewat:                                                        <br> &nbsp;&nbsp;&nbsp;&nbsp;
    pecah jadi file baru atau pindahkan logika ke service/ / util/

Tujuan:                                                             <br> &nbsp;&nbsp;&nbsp;&nbsp;
    supaya gampang dibaca.

---

## 4) Aturan Git (Wajib)
Branch yang dipakai:                                                <br> &nbsp;&nbsp;&nbsp;&nbsp;
    main → versi final

Aturan branch:                                                      <br> &nbsp;&nbsp;&nbsp;&nbsp;
    nama-yang-ngerjain/nama-fitur → kerja masing-masing

Contoh:                                                             <br> &nbsp;&nbsp;&nbsp;&nbsp;
    doni-simamora/login-api