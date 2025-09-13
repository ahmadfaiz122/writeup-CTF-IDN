# 📝 Writeup CTF Seleksi Bootcamp ID.Networkers

Repositori ini berisi dokumentasi writeup dari **CTF Seleksi Bootcamp Gratis ID.Networkers**.  
CTF ini menjadi tahap seleksi bagi peserta yang ingin mengikuti bootcamp dengan fokus pada bidang **Keamanan Siber**.  

---

## 📂 Daftar Isi
- [Web Exploit](#-web-exploit)
- [Web 303](#-web-303)
- [Log Analysis](#-log-analysis)
- [Forensic](#-forensic)

---

## 🌐 Web Exploit
### Deskripsi
Kategori ini berisi challenge eksploitasi web dengan fokus pada analisis request/response, parameter injection, dan bypass mekanisme autentikasi/validasi.  

### Writeup
- **Challenge:** `Web Exploit 1`  
  **Solusi:**  
  - Analisis endpoint menggunakan `Burp Suite`.  
  - Parameter `id` rentan terhadap **SQL Injection**.  
  - Payload yang digunakan:  
    ```sql
    ' OR '1'='1' --
    ```
  - Flag berhasil diperoleh dari response database.  

---

## 🔄 Web 303
### Deskripsi
Kategori ini menguji pemahaman terhadap **HTTP status code 3xx**, khususnya **redirect handling** dan teknik manipulasi header.

### Writeup
- **Challenge:** `Web 303 Redirect`  
  **Solusi:**  
  - Aplikasi melakukan redirect berantai (status 302 → 303).  
  - Setelah memodifikasi header `Location`, akses diarahkan ke endpoint tersembunyi `/flag`.  
  - Flag berhasil didapatkan setelah mengikuti seluruh chain redirect.  

---

## 📑 Log Analysis
### Deskripsi
Kategori ini berisi analisis log sistem untuk menemukan jejak serangan, payload berbahaya, dan pola anomali.  

### Writeup
- **Challenge:** `Log Hunt`  
  **Solusi:**  
  - File log dianalisis dengan `grep` & `awk`.  
  - Terdapat request mencurigakan pada `/upload.php` dengan payload encoded.  
  - Setelah decode, ditemukan backdoor PHP yang mengarah ke `flag.txt`.  
  - Flag ditemukan di dalam log access setelah payload berhasil dieksekusi.  

---

## 🕵️ Forensic
### Deskripsi
Kategori ini berfokus pada investigasi file dump, memory image, dan analisis artefak untuk menemukan informasi tersembunyi.  

### Writeup
- **Challenge:** `Disk Dump Investigation`  
  **Solusi:**  
  - Ekstrak file menggunakan `binwalk`.  
  - Ditemukan file ZIP tersembunyi di dalam dump.  
  - Setelah di-unzip, terdapat gambar `.png`.  
  - Menggunakan `strings` pada file gambar ditemukan hidden flag.  

---

## 🎯 Tujuan Repositori
- Menyimpan arsip hasil pengerjaan CTF seleksi bootcamp ID.Networkers.  
- Berbagi pengetahuan dan solusi agar peserta lain dapat belajar.  
- Menjadi referensi bagi siapa saja yang ingin mengasah skill CTF & cybersecurity.  

---

## ⚠️ Catatan
Writeup ini dibuat untuk tujuan **pembelajaran**.  
Gunakan informasi di sini secara bijak dan **jangan disalahgunakan**.  
