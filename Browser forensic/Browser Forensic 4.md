## Deskripsi

Ada Volation yang dilakukan oleh user di satu laptop, coba bantu forensic browsernya dong !!
(Filenya ada di pertanyaan pertama)
Vpn apa saja yang diinstal oleh user ?
format flag : IDN_FLAG{VPN_1-VPN_2} example : IDN_FLAG{IPSEC_SECURITY-L2TP_SECURITY}

#### Auhtor: Aditya Firman Nugroho

## solusi
Pada soal nomor 4 ini, saya tetap menggunakan tools yang sama seperti yang telah saya gunakan pada soal-soal sebelumnya, yaitu soal 1, 2, dan 3. Tools ini sudah terbukti sangat membantu dalam proses pencarian dan analisis data, baik dalam bentuk file sistem maupun database. Karena saya sudah cukup familiar dengan fungsionalitas dan antarmuka tools tersebut, saya dapat langsung melanjutkan proses investigasi tanpa harus melakukan penyesuaian ulang.
Konsistensi dalam penggunaan tools yang sama memberikan keuntungan tersendiri, terutama dalam hal efisiensi dan efektivitas. Saya tidak hanya bisa menelusuri struktur folder dan file dengan cepat, tetapi juga dapat melakukan eksplorasi mendalam ke dalam database, termasuk membuka tabel, melihat isi kolom, dan mengamati setiap baris data dengan lebih mudah.
Pada tahap ini, saya kembali menerapkan metode yang sama seperti sebelumnya, yaitu memeriksa setiap bagian data secara teliti. Dengan tools yang sama, saya merasa lebih percaya diri dalam menavigasi sistem dan lebih fokus untuk mencari pola-pola yang mencurigakan atau tidak biasa—yang sering kali menjadi petunjuk keberadaan flag.

<img width="940" height="121" alt="image" src="https://github.com/user-attachments/assets/22184c64-0cdd-4b5a-aab7-69aa82289e3f" />

<img width="940" height="113" alt="image" src="https://github.com/user-attachments/assets/4ef0be3d-9644-4761-9958-bf46d1aceca6" />

Pada soal nomor 4, saya masih menggunakan tools yang sama seperti pada soal-soal sebelumnya karena tools tersebut telah terbukti sangat efektif dalam proses pencarian flag. Dengan tools ini, saya bisa menjelajahi database, membuka tabel-tabel yang relevan, dan memeriksa isinya dengan mudah dan sistematis.
Saya kemudian menelusuri salah satu tabel dan mulai menganalisis setiap baris data yang ada. Dalam proses ini, saya menemukan dua entri yang mencurigakan, yaitu pada baris dengan id 2 dan id 23. Kedua entri tersebut mengarah pada layanan VPN, dan dari konteksnya terlihat bahwa itu merupakan jenis VPN yang sedang dicari oleh user dalam soal.

Setelah mencocokkannya dengan format flag yang diminta, yaitu:
IDN_FLAG{IPSEC_SECURITY-L2TP_SECURITY}

## flag
IDN_FLAG{BROWSEC_VPN-VPN_PROXY_VEEPN}
