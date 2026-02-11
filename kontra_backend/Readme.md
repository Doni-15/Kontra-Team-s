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

```txt
com.kontra.astrosyncs  
│                                                              
├── config/          # konfigurasi (CORS, scheduler, security) 
├── controller/      # endpoint REST API                       
├── dto/             # request/response object                 
│   ├── request/                                               
│   └── response/                                              
├── entity/          # class model (tabel database)            
├── enums/           # enum (Role, Status, dll)                
├── repository/      # akses database (JPA Repository)         
├── service/         # business logic utama                    
├── util/            # helper kecil (converter, time helper)   
└── exception/       # custom error & handler                  
```

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