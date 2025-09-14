## Deskripsi
Ada Volation yang dilakukan oleh user di satu laptop, coba bantu forensic browsernya dong !!
(Filenya ada di pertanyaan pertama)
Streaming Website yang ditonton oleh user ?
format flag : IDN_FLAG{Jawaban yang disoal}

## solusi

Pada soal nomor 3 ini, saya kembali menggunakan tools yang sama seperti yang telah saya gunakan pada soal sebelumnya. Tools tersebut terbukti sangat membantu dalam menelusuri struktur database secara menyeluruh dan efisien. Karena saya sudah terbiasa menggunakannya, saya dapat langsung fokus pada proses analisis tanpa harus menyesuaikan diri kembali dengan antarmuka atau cara kerja tools tersebut.
Menariknya, saat saya mulai menyelidiki isi database untuk soal ketiga ini, saya menemukan bahwa flag ternyata disimpan di tabel yang sama seperti pada soal nomor 2, yaitu tabel urls. Hal ini membuat saya langsung teringat untuk memeriksa tabel tersebut secara lebih teliti, karena kemungkinan besar pola penyembunyian flag masih serupa

<img width="940" height="438" alt="image" src="https://github.com/user-attachments/assets/0aeb6f28-0773-4371-8bcb-ee4ff7168b70" />

Saya pun mulai membuka dan menelusuri setiap baris dalam tabel urls, hingga akhirnya saya menemukan sebuah entri yang mencurigakan pada baris dengan id bernomor 7. Setelah saya analisis lebih lanjut, benar saja — di dalam kolom pada baris tersebut terdapat flag yang tersembunyi. Flag ini tidak langsung terlihat mencolok, namun dengan pendekatan yang sistematis dan ketelitian dalam memeriksa setiap entri, saya berhasil menemukannya

## flag
IDN_FLAG{https://www.netflix.com/}
