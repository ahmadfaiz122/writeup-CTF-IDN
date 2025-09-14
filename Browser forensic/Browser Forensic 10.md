## deskripsi
Ada Volation yang dilakukan oleh user di satu laptop, coba bantu forensic browsernya dong !! (Filenya ada di pertanyaan pertama)
Version vpn V.. yang diinstal oleh user ?
format flag : IDN_FLAG{Jawaban yang disoal}

#### Auhtor: Aditya Firman Nugroho

## solusi
Pada soal nomor 10, proses pencarian flag terasa lebih mudah dibandingkan soal-soal sebelumnya, karena deskripsi soalnya sangat membantu dan memberikan petunjuk yang jelas.
Deskripsi soal menyebutkan bahwa yang diminta adalah "version VPN V", yang saya tafsirkan sebagai versi dari ekstensi VPN tertentu yang sebelumnya telah ditemukan.
Saya mengingat kembali bahwa pada soal nomor 9, saya telah menemukan extension ID dari sebuah ekstensi VPN dengan ikon yang dimulai dengan huruf V, dan folder itulah yang menjadi flag saat itu.
Berbekal informasi tersebut, saya langsung membuka kembali subfolder ekstensi yang menjadi jawaban di soal nomor 9, karena saya menduga versi VPN yang diminta pasti ada di dalam struktur folder ekstensi tersebut.

<img width="791" height="423" alt="image" src="https://github.com/user-attachments/assets/fbe9f0ed-dee8-4ea5-8536-642da9f24236" />

Benar saja, setelah saya telusuri isi folder tersebut, saya menemukan file yang berisi informasi mengenai versi dari ekstensi tersebut. Saya membaca metadata atau nama folder/versi yang digunakan, dan dari situ saya mendapatkan versi dari VPN ekstensi V tersebut, yang langsung saya sesuaikan dengan format flag seperti yang diminta.

<img width="823" height="473" alt="image" src="https://github.com/user-attachments/assets/64747323-a73f-4310-b494-e19eebc70fc8" />

Dengan begitu, saya berhasil menemukan flag untuk soal nomor 10, hanya dengan melanjutkan eksplorasi dari folder yang sudah ditemukan sebelumnya di soal 9.

## flag
IDN_FLAG{3.4.3_0}
