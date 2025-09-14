## Deskripsi
Ada Volation yang dilakukan oleh user di satu laptop, coba bantu forensic browsernya dong !!
(Filenya ada di pertanyaan pertama)
extension id dengan icon salah satu vpn yang diinstal V.. !
format flag : IDN_FLAG{Jawaban yang disoal}

#### Auhtor: Aditya Firman Nugroho

## solusi
Pada soal nomor 9, saya memperhatikan bahwa dalam deskripsi soal disebutkan bahwa yang diminta adalah “extension ID”. Berdasarkan petunjuk tersebut, saya menyimpulkan bahwa flag kemungkinan besar terkait dengan ekstensi (extension) yang terinstal di browser, dan fokus pencariannya harus diarahkan ke folder atau file yang menyimpan informasi tentang ekstensi tersebut

<img width="791" height="423" alt="image" src="https://github.com/user-attachments/assets/085b8f13-368a-4aef-83c7-0ce30c7e4f8c" />

Saya kemudian menelusuri struktur direktori browser, terutama pada folder yang biasanya digunakan untuk menyimpan ekstensi, yaitu folder Extensions. Saya membuka folder tersebut dan menemukan bahwa di dalamnya terdapat sejumlah subfolder yang masing-masing dinamai dengan ID unik — ID inilah yang biasanya mewakili masing-masing ekstensi yang diinstal oleh pengguna.

dan nama sub folder kedua itu lah flag nya

<img width="806" height="267" alt="image" src="https://github.com/user-attachments/assets/05d64949-d0c4-4aa5-b406-c4cf0b5afbde" />

## flag
IDN_FLAG{majdfhpaihoncoakbjgbdhglocklcgno}
