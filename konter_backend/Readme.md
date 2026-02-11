# Backend - AstroSyncs (Java)
Dokumentasi struktur folder, aturan penamaan, dan aturan kerja tim untuk backend AstroSyncs.

---

## Struktur Folder Backend (Java)
Semua file Java wajib berada di:

```txt
src/com/konter/astrosyncs
```

---

## 1) Pembagian Folder
```txt
com.konter.astrosyncs  
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

Semua file Java wajib pakai prefix:                                 
    konter_

```txt
Contoh:                                                             
    konter_User.java
```

Ini wajib supaya konsisten dan mudah dicari (Biar keren 🥶☠️).

---

## 3) Maksimal 200 Baris per File
Setiap file usahakan maksimal 200 baris.     

```txt
Kalau lewat:                                                        
    pecah jadi file baru atau pindahkan logika ke service/ atua util/
```

```txt
Tujuan:                                                             
    supaya gampang dibaca.
```

---

## 4) Aturan Git (Wajib)

```txt
Branch yang dipakai:                                                
    main → versi final
```

```txt
Aturan branch:                                                      
    nama-yang-ngerjain/nama-fitur --> kerja masing-masing
```

```txt
Contoh:                                                             
    doni-simamora/login-api
```