## Deskripsi
Ada Volation yang dilakukan oleh user di satu laptop, coba bantu forensic browsernya dong !!
Tools apa yang di cari oleh user ?
format flag : IDN_FLAG{Jawaban yang disoal}

#### Auhtor: Aditya Firman Nugroho

## Solusi
Saya memulai pencarian flag ini dengan membuka setiap folder dan file yang tersedia satu per satu secara teliti. Awalnya, saya tidak mengetahui dengan pasti di mana flag tersebut disimpan, sehingga saya memutuskan untuk memeriksa seluruh struktur direktori tanpa melewatkan satu pun folder maupun file. Proses ini saya lakukan secara sistematis, mulai dari folder yang paling atas hingga ke subfolder-subfolder yang ada di dalamnya.
Setelah membuka dan memeriksa banyak folder dan file, akhirnya saya menemukan sebuah folder yang bernama default. Nama folder ini menarik perhatian saya karena bisa jadi merupakan direktori tempat penyimpanan pengaturan atau data awal yang bersifat penting. Ketika saya masuk ke dalam folder default, saya menemukan sebuah file dengan nama history.

<img width="401" height="384" alt="image" src="https://github.com/user-attachments/assets/8ac96b49-d6e1-420d-9b32-329c853a6ae9" />

Karena nama file tersebut mengindikasikan bahwa ia mungkin menyimpan catatan aktivitas sebelumnya, saya pun membukanya dan memeriksa isinya dengan menggunakan tools  https://inloop.github.io/sqlite-viewer/.

<img width="940" height="315" alt="image" src="https://github.com/user-attachments/assets/c10c9a6c-5603-4c68-89dc-b6be9f60a0b1" />

Dengan menggunakan tools tersebut, saya dapat melihat struktur tabel, isi datanya, serta melakukan query untuk mendapatkan informasi yang lebih spesifik. Saya memastikan untuk tidak melewatkan satu tabel pun dalam proses ini, karena setiap tabel berpotensi menyimpan informasi penting yang tersembunyi.
Akhirnya, setelah memeriksa cukup banyak tabel, saya menemukan sebuah entri yang mencurigakan dan setelah saya selidiki lebih lanjut, entri tersebut mengandung flag yang saya cari. Proses ini membutuhkan ketelitian dan kesabaran, namun dengan pendekatan yang sistematis dan penggunaan tools yang tepat, saya berhasil menemukan flag tersebut.

<img width="940" height="102" alt="image" src="https://github.com/user-attachments/assets/64f6116a-5518-433a-9ddd-4eeecb8a4ed5" />

saya curiga di dua column dengan id 23 dan 24 terlihat ada 2 link github yang merujuk kepada tools hacking pertama saya coba cari di google link github tersebut dan benar kedua nya adalah tools hacking.

saya coba input terlebih dahulu nama tools nya yaitu mimikatz dan ternyata benar itu flag nya

## flag:
IDN_FLAG{mimikatz}
