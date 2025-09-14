## Deskripsi
Ada Volation yang dilakukan oleh user di satu laptop, coba bantu forensic browsernya dong !! (Filenya ada di pertanyaan pertama)
Email yang digunakan pada browser ?
format flag : IDN_FLAG{Jawaban yang disoal}

## solusi
Pada soal nomor 6 ini, saya memutuskan untuk menggunakan teknik yang berbeda dibanding soal-soal sebelumnya. Alih-alih langsung mengakses database atau tabel seperti yang saya lakukan pada soal 1–5, kali ini saya fokus menelusuri struktur file secara manual.
Saya memulai dengan membuka folder User Data, karena folder ini biasanya menyimpan berbagai konfigurasi dan aktivitas pengguna. Setelah itu, saya membuka file-file yang terdapat di dalam folder tersebut satu per satu, dengan tujuan untuk menemukan data sensitif atau jejak aktivitas yang bisa mengarah pada flag.
Untuk mempercepat pencarian, saya menggunakan command-line tool find dengan perintah berbasis string, yaitu:

<img width="940" height="452" alt="image" src="https://github.com/user-attachments/assets/4b492c41-afa9-4ded-b661-4b0f8241a965" />

dan ketemulah flag nya:

## flag
IDN_FLAG{ghxyssforunfun@gmail.com}
