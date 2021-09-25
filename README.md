# Jarkom-Modul-1-C01-2021

# Anggota Kelompok
- **Muhammad Arifiansyah** (05111940000027)
- **Melanchthon Bonifacio Butarbutar** (05111940000097)
- **Muhammad Valda Rizky Nur Firdaus** (05111940000115)

# Pembahasan Soal
## Soal 1
Sebutkan webserver yang digunakan pada "ichimarumaru.tech"! <br>
**Filter**: ```http.host == "ichimarumaru.tech"``` <br>
**Cara pengerjaan**: Setelah memasukkan filter di atas pada display filter, pilih salah satu packet dan follow TCP Stream. <br>
**Screenshot**: <br>
![alt text](https://github.com/Kyu-u/Jarkom-Modul-1-C01-2021/blob/main/images/soal1.png) <br>
## Soal 2
Temukan paket dari web-web yang menggunakan basic authentication method! <br>
**Filter**: ```http.authbasic``` <br>
**Cara pengerjaan**: Masukkan display filter di atas <br>
**Screenshot**: <br>
![alt text](https://github.com/Kyu-u/Jarkom-Modul-1-C01-2021/blob/main/images/soal2.png) <br>
## Soal 3
 Ikuti perintah di basic.ichimarumaru.tech! Username dan password bisa didapatkan dari file .pcapng! <br>
**Filter**: ```http.host == “basic.ichimarumaru.host”``` <br>
**Cara pengerjaan**: Masukkan display filter di atas kemudian username dan password akan ditampilkan di bagian credentials. <br>
**Screenshot**: <br>
![alt text](https://github.com/Kyu-u/Jarkom-Modul-1-C01-2021/blob/main/images/soal3a.png) <br>
![alt text](https://github.com/Kyu-u/Jarkom-Modul-1-C01-2021/blob/main/images/soal3b.png) <br>
## Soal 4
 Temukan paket mysql yang mengandung perintah query select! <br>
**Filter**: ```mysql.query matches select``` <br>
**Cara pengerjaan**: Masukkan display filter di atas dan paket yang sesuai akan ditampilkan. <br>
**Screenshot**: <br>
![alt text](https://github.com/Kyu-u/Jarkom-Modul-1-C01-2021/blob/main/images/soal4.png) <br>
## Soal 5
Login ke portal.ichimarumaru.tech kemudian ikuti perintahnya! <br>
Username dan password bisa didapat dari query insert pada table users dari file .pcap! <br>
**Filter**: ```mysql.query matches insert``` <br>
**Cara pengerjaan**: Masukkan display filter di atas dan username berserta password akan terlihat pada query. <br>
**Screenshot**: <br>
![alt text](https://github.com/Kyu-u/Jarkom-Modul-1-C01-2021/blob/main/images/soal5a.png) <br>
![alt text](https://github.com/Kyu-u/Jarkom-Modul-1-C01-2021/blob/main/images/soal5b.png) <br>
## Soal 6
Cari username dan password ketika melakukan login ke FTP Server <br>
**Filter**: ```ftp.request.command == USER``` <br>
**Cara pengerjaan**: Masukkan display filter di atas kemudian Follow TCP Stream pada salah satu paket. <br>
**Screenshot**: <br>
![alt text](https://github.com/Kyu-u/Jarkom-Modul-1-C01-2021/blob/main/images/soal6.png) <br>
## Soal 7
Ada 500 file zip yang disimpan ke FTP Server dengan nama 0.zip, 1.zip, 2.zip, ..., 499.zip. Simpan dan Buka file pdf tersebut. (Hint = nama pdf-nya "Real.pdf") <br>
**Filter**: ```ftp-data && frame contains "Real.pdf"``` <br>
**Cara pengerjaan**: Masukkan display filter di atas kemudian Follow TCP Stream dan ganti show data as “raw” dan save data sebagai zip. <br>
**Screenshot**: <br>
![alt text](https://github.com/Kyu-u/Jarkom-Modul-1-C01-2021/blob/main/images/soal7.jpg) <br>
## Soal 8
**Filter**:  <br>
**Cara pengerjaan**: <br>
**Screenshot**: <br>
## Soal 9
Dari paket-paket yang menuju FTP terdapat inidkasi penyimpanan beberapa file. Salah satunya adalah sebuah file berisi data rahasia dengan nama "secret.zip". Simpan dan buka file tersebut! <br>
**Filter**: ```ftp-data.command contains "secret.zip"``` <br>
**Cara pengerjaan**: Masukkan display filter di atas kemudian Follow TCP Stream dan ganti show data as “raw” dan save data sebagai zip. <br>
**Screenshot**: <br>
![alt text](https://github.com/Kyu-u/Jarkom-Modul-1-C01-2021/blob/main/images/soal9a.png) <br>
![alt text](https://github.com/Kyu-u/Jarkom-Modul-1-C01-2021/blob/main/images/soal9b.png) <br>
## Soal 10
Selain itu terdapat "history.txt" yang kemungkinan berisi history bash server tersebut! Gunakan isi dari "history.txt" untuk menemukan password untuk membuka file rahasia yang ada di "secret.zip"! <br>
**Filter**: ```ftp-data.command contains "history.txt"``` <br>
**Cara pengerjaan**:
- Masukkan display filter di atas kemudian Follow TCP Stream.
- Kemudian filter lagi menggunakan ```ftp-data.command contains "bukanapaapa.txt" ``` dan follow TCP Stream.
- Masukkan password
**Screenshot**: <br>
![alt text](https://github.com/Kyu-u/Jarkom-Modul-1-C01-2021/blob/main/images/soal10a.png) <br>
![alt text](https://github.com/Kyu-u/Jarkom-Modul-1-C01-2021/blob/main/images/soal10b.png) <br>
![alt text](https://github.com/Kyu-u/Jarkom-Modul-1-C01-2021/blob/main/images/soal10c.png) <br>








