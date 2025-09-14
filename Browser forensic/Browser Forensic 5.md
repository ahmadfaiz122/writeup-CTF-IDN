## Deskripsi
Ada Volation yang dilakukan oleh user di satu laptop, coba bantu forensic browsernya dong !!
(Filenya ada di pertanyaan pertama)
Visit Duration di Website yang berkaitan dengan Persistence, Privilage Escalation, DLL Injection ?
format flag : IDN_FLAG{Jawaban yang disoal} example : XX:XX:XX.XXX

## solusi 
Pada soal nomor 5, saya tetap konsisten menggunakan tools yang sama seperti yang saya gunakan pada soal-soal sebelumnya (soal 1 hingga 4). Tools ini telah terbukti sangat membantu dalam proses investigasi, baik dalam menjelajahi struktur file maupun mengakses dan menganalisis database. Karena sudah familiar, saya dapat langsung fokus ke proses pencarian tanpa perlu membuang waktu untuk beradaptasi ulang.
Seperti biasa, saya memulai dengan menyisir data yang tersedia melalui tools tersebut. Saya menelusuri struktur direktori, membuka setiap file atau tabel yang relevan, dan memeriksa isinya satu per satu secara sistematis. Proses ini sudah menjadi pola kerja yang saya terapkan sejak soal pertama dan terus saya gunakan karena terbukti efektif dalam menemukan flag.
Penggunaan tools yang sama secara konsisten memudahkan saya untuk mengidentifikasi pola-pola soal dan mempercepat proses pencarian informasi penting seperti flag. Pada soal kelima ini pun, saya kembali mengandalkan keakuratan tools tersebut untuk mengakses data yang diperlukan dan menyelesaikan tantangan dengan baik.

<img width="940" height="450" alt="image" src="https://github.com/user-attachments/assets/ea97d90c-327f-430c-838c-3c86a1393685" />

Langkah pertama saya adalah membuka dan memeriksa tabel-tabel yang tersedia dalam database. Saat itu saya menemukan sebuah tabel bernama visits, yang di dalamnya terdapat kolom visit_duration. Awalnya saya cukup bingung karena terdapat banyak nilai pada kolom tersebut, dan saya tidak yakin data mana yang berkaitan langsung dengan flag atau informasi penting yang diminta.
Namun, saya tidak berhenti di situ. Saya melanjutkan pencarian dan menemukan tabel lain yang bernama clusters_and_visits. Tabel ini menarik perhatian saya karena tampaknya memiliki relasi dengan tabel visits, dan berpotensi menyimpan informasi tambahan yang lebih spesifik.

<img width="940" height="421" alt="image" src="https://github.com/user-attachments/assets/a3794d40-dd00-401b-a8a3-27017840afd3" />

Saya pun mulai menganalisis isi tabel tersebut dan menemukan adanya kolom visit_id, yang menunjukkan keterkaitan dengan data di tabel visits. Dari sinilah saya mulai mencari visit_id yang merujuk pada aktivitas mencurigakan atau yang terkait dengan teknik hacking tertentu.
Berdasarkan pengetahuan saya, saya mengenali bahwa salah satu website yang biasa digunakan untuk teknik living off the land binaries (LOLbins) adalah lolbas. Saya kemudian mencocokkan URL yang mengarah ke website tersebut di dalam data, dan setelah saya telusuri, saya menemukan bahwa URL tersebut berada pada visit_id dengan nilai 28.
Dari penemuan ini, saya menyimpulkan bahwa flag atau informasi penting pada soal nomor 5 berhubungan erat dengan visit_id 28, yang mengarah ke website teknik hacking lolbas.

<img width="940" height="56" alt="image" src="https://github.com/user-attachments/assets/0527fcbc-9293-43fc-b229-12fc0b8179ae" />

Berdasarkan informasi tersebut, saya langsung membuka entri pada tabel visits dengan id 28, dan saya menemukan nilai visit_duration yang ada di sana. Saya menyalin nilainya, lalu mulai menyesuaikan dengan format flag yang diminta, yaitu:
XX:XX:XX.XXX

Dari sini saya menyadari bahwa visit_duration hanya menyatakan nilai dalam detik (misalnya: 32.509). Maka saya pahami bahwa:
●	Bagian pertama (00) menunjukkan jam

●	Bagian kedua (00) menunjukkan menit

●	Bagian ketiga (32.509) menunjukkan detik dan milidetik

Sehingga saya konversi durasi tersebut ke dalam format yang sesuai, yaitu:

## flag
IDN_FLAG{00:00:32.509}
