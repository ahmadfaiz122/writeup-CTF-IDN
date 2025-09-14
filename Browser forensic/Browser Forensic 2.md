## Deskripsi

Ada Volation yang dilakukan oleh user di satu laptop, coba bantu forensic browsernya dong !!
(Filenya ada di pertanyaan pertama)
Website apa yang dicari oleh user berkaitan dengan Teknik Persistence, Privilage Escalation, DLL Injection etc ?
format flag : IDN_FLAG{Jawaban yang disoal}

#### Auhtor: Aditya Firman Nugroho

## solusi

Dalam proses pencarian flag ini, saya menggunakan tools yang sama seperti yang saya gunakan pada langkah pertama. Tools tersebut terbukti cukup efektif dan memberikan kemudahan dalam menavigasi serta menganalisis struktur data yang tersedia. Karena saya sudah familiar dengan cara kerja tools tersebut dari penggunaan sebelumnya, saya bisa langsung menggunakannya tanpa perlu penyesuaian ulang.
Tools ini memungkinkan saya untuk mengakses dan memeriksa berbagai komponen sistem secara mendalam, termasuk file, folder, serta database dan tabel-tabel yang ada di dalamnya. Dengan fitur-fiturnya, saya dapat membuka setiap tabel satu per satu, mengecek isi data di dalamnya, dan mencari pola atau informasi yang mencurigakan yang bisa mengarah pada flag.
Familiaritas saya terhadap tools ini sangat membantu mempercepat proses pencarian karena saya sudah tahu fitur-fitur mana yang perlu dimanfaatkan untuk menelusuri informasi secara lebih efisien dan mendalam.

<img width="940" height="38" alt="image" src="https://github.com/user-attachments/assets/2ecbd203-7f8b-4f5e-8676-eb966541a18b" />

Saat saya sedang memeriksa isi dari tabel bernama urls menggunakan tools yang sama seperti pada langkah sebelumnya, saya menemukan sebuah entri yang mencurigakan. Di dalam tabel tersebut terdapat sejumlah baris data yang berisi link-link website, dan saya menelusuri satu per satu untuk melihat apakah ada yang mengarah ke sesuatu yang mencurigakan atau tidak biasa.
Ketika saya sampai pada baris dengan id bernomor 28, saya merasa ada sesuatu yang tidak biasa. Link pada baris tersebut tampak berbeda dibandingkan dengan link-link lainnya—baik dari segi struktur maupun kontennya. Karena rasa penasaran dan kecurigaan saya cukup tinggi terhadap entri ini, saya pun memutuskan untuk menyelidikinya lebih dalam.
Setelah saya membuka dan menganalisis lebih lanjut isi dari kolom pada baris dengan id 28 tersebut, ternyata benar dugaan saya. Di sanalah flag yang saya cari disembunyikan. Flag tersebut disisipkan dengan rapi di dalam data pada kolom tersebut, dan tidak langsung terlihat mencolok. Penemuan ini menegaskan bahwa ketelitian dalam memeriksa setiap entri sangat penting, karena informasi penting seperti flag bisa saja disembunyikan di tempat yang tidak terduga

## flag
IDN_FLAG{https://lolbas-project.github.io}/}
