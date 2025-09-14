## Deskripsi
Ada Volation yang dilakukan oleh user di satu laptop, coba bantu forensic browsernya dong !!
(Filenya ada di pertanyaan pertama)
url favicon, di website yang dicari oleh user ? ( tidak berkaitan dengan hacker !!! )
format flag : IDN_FLAG{Jawaban yang disoal}

#### Auhtor: Aditya Firman Nugroho

## solusi
Pada soal nomor 8, saya kembali melakukan eksplorasi dengan teliti terhadap semua folder dan file yang tersedia dalam sistem. Setelah mencoba beberapa pendekatan, saya menemukan bahwa flag untuk soal ini tidak berada di file atau tabel yang sama seperti soal-soal sebelumnya, melainkan tersembunyi di file yang berbeda, yang awalnya tidak saya duga.
Saya mulai menyisir folder Default, yang merupakan salah satu direktori penting dalam struktur data browser, karena biasanya menyimpan berbagai informasi terkait aktivitas pengguna. Di dalam folder ini, saya menemukan sebuah file yang menarik perhatian saya, yaitu Favicons.

<img width="940" height="340" alt="image" src="https://github.com/user-attachments/assets/157b9891-4239-4dd1-959e-669f244bf4fd" />

Dari hasil penelusuran saya terhadap tabel-tabel di dalam file ini, saya menemukan sebuah URL pada entri dengan ID 3, dan setelah saya cermati, URL tersebut merujuk langsung ke file favicon dari sebuah situs web.
Karena ini adalah soal CTF, saya mencurigai bahwa URL ini bukan hanya sebuah ikon biasa, melainkan kemungkinan besar telah dimodifikasi untuk menyisipkan flag. Saya menyalin (copy) URL tersebut, lalu saya menyesuaikannya dengan format flag yang ditentukan dalam soal.
Setelah penyesuaian dan pengecekan ulang, ternyata benar — URL tersebut adalah flag-nya.

## flag
IDN_FLAG{https://www.muslima.com/lp/paid-search/terra-assets/images/favicon-8b7d9ccfa1-3.ico}
