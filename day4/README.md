'''''''''''''''''''''''''''''''''''''

1. Jelaskan apa itu teks editor (docs shortcut" nya apa) 
- Suatu software yang digunakan untuk mengolah teks dengan keterbatasan tertentu (tidak seperti word) yang memiliki fungsi-fungsi dasar agar membantu dalam pengolahan teks ringan serta namun powerfull untuk digunakan dalam pemrograman khususnya



nano <namafile>

![Screenshot from 2023-12-01 00-02-10](https://github.com/Subzero16/TUGAS/assets/69718826/d7ee7aa9-a7e2-40e2-9979-1b728642d31f)

nano <ctrl +x> simpan file lalu tutup otomatis

![Screenshot from 2023-12-01 01-45-46](https://github.com/Subzero16/TUGAS/assets/69718826/07711791-e069-4a54-ab60-404b5f6cd772)

nano <ctrl +o> simpan file tetap dalam editor

![Screenshot from 2023-12-01 01-46-22](https://github.com/Subzero16/TUGAS/assets/69718826/b35fc428-7886-4a7e-aa63-366aa4b39520)

nano <ctrl +w> mencari kata

![Screenshot from 2023-12-01 01-47-55](https://github.com/Subzero16/TUGAS/assets/69718826/40f0bcf6-92a6-42b4-bb30-cb8384ab9ae0)

nano <alt +a> menandai kursos untuk blok

![Screenshot from 2023-12-01 01-48-59](https://github.com/Subzero16/TUGAS/assets/69718826/e4b24cd2-30dc-4de1-8835-c7eb8277567a)

nano <ctrl +n> enable line by number

![Screenshot from 2023-12-01 02-07-47](https://github.com/Subzero16/TUGAS/assets/69718826/951b6131-5517-41f7-a1d0-f67a4a2e124c)

nano <ctrl +/> menuju line by number

![Screenshot from 2023-12-01 02-08-14](https://github.com/Subzero16/TUGAS/assets/69718826/943ed288-d2aa-46f4-b6de-8c0b32520845)

2. manipulation teks (docs manipulation teks)

cat / concatenate / pada umumnya digunakan untuk menggabungkan teks pada excel (rumus)tetapi pada linux adalah sebuah perintah yang digunakan untuk menampilkan isi file tanpa harus membuka pada aplikasi bantu lainnya (quick view)

cat <file1 + file2 = file3> menggabungkan 2 file atau lebih dan menghasilkan file baru

<img width="503" alt="Screenshot 2023-12-01 at 06 50 42" src="https://github.com/Subzero16/TUGAS/assets/69718826/5067f4fd-af1b-48f3-9aa1-b44fab92cf7a">

cat <namafile> quick view

<img width="396" alt="Screenshot 2023-12-01 at 06 51 17" src="https://github.com/Subzero16/TUGAS/assets/69718826/842a543d-ea42-455e-9692-b2d0e091a529">

cat <merubah isi file >

<img width="402" alt="Screenshot 2023-12-01 at 06 52 57" src="https://github.com/Subzero16/TUGAS/assets/69718826/baf83b52-d619-4a24-8935-e845d09c00ab">

cat <menambah isi file pada line baru>

<img width="448" alt="Screenshot 2023-12-01 at 06 53 41" src="https://github.com/Subzero16/TUGAS/assets/69718826/2041ca62-7774-46e7-bbeb-2cac0ea84238">

--------------------------

sed (stream editor)

<img width="583" alt="Screenshot 2023-12-01 at 06 54 35" src="https://github.com/Subzero16/TUGAS/assets/69718826/7abb0eea-9e0f-43e6-bdfc-f88198281e92">

grep (mencari file)

<img width="442" alt="Screenshot 2023-12-01 at 06 55 52" src="https://github.com/Subzero16/TUGAS/assets/69718826/43ff21b0-30b4-4c12-bd0f-750e66c0121c">

grep -c (menghitung kata dari atau pada file

<img width="498" alt="Screenshot 2023-12-01 at 06 56 26" src="https://github.com/Subzero16/TUGAS/assets/69718826/76cc70ab-0b31-4ee9-af96-4804012076eb">

grep * (mencari kata pada file yang tidak diketahui namanya)

<img width="438" alt="Screenshot 2023-12-01 at 06 57 05" src="https://github.com/Subzero16/TUGAS/assets/69718826/0a798317-e0fb-4538-a839-140836f55f3a">

grep + history 

<img width="570" alt="Screenshot 2023-12-01 at 06 57 40" src="https://github.com/Subzero16/TUGAS/assets/69718826/22c5d6e8-e205-461e-817e-26c7f737e546">

sort -r (reverse)

<img width="475" alt="Screenshot 2023-12-01 at 06 58 13" src="https://github.com/Subzero16/TUGAS/assets/69718826/842a375e-cae0-493e-8f99-f109c1899760">

sort (berurutan)

<img width="445" alt="Screenshot 2023-12-01 at 06 58 43" src="https://github.com/Subzero16/TUGAS/assets/69718826/a7e25306-4118-4beb-894e-c2cd721c62ca">

echo (mirip dengan cat)

<img width="467" alt="Screenshot 2023-12-01 at 06 59 03" src="https://github.com/Subzero16/TUGAS/assets/69718826/76df3659-3b5e-41fe-a694-224e870c9544">

echo .sh (running file)

<img width="522" alt="Screenshot 2023-12-01 at 06 59 58" src="https://github.com/Subzero16/TUGAS/assets/69718826/91664f70-d18b-4c5f-8748-b73dc775f6e3">

3. Penjelasan apa itu firewall, fungsi firewall, di gunakan untuk apa (docs ufw , ex allow, deny )
Mekanisme teknis maupun konfigurasi yang bertujuan untuk menyaring lalu lintas data yang masuk maupun keluar


Hardware Firewall

>Juniper/Bitdefender Box/Fortinet/Sophos

![51oB6FBEWeL](https://github.com/Subzero16/TUGAS/assets/69718826/292a9a6b-c320-4480-af27-31566d290e93)


Software Firewall
Sebuah konfigurasi yang bertujuan untuk filter komunikasi data yang akan masuk dan keluar kedalam sistem yang kita miliki (server maupun desktop)

<img width="291" alt="Screenshot 2023-12-01 at 07 03 07" src="https://github.com/Subzero16/TUGAS/assets/69718826/0e05541b-1ac4-4820-bc27-711bf710d6e1">


Proxy Firewall

> Setting konfigurasi Firewall melalui server lain atau forwarding (3rd-party ip) jadi komunikasi tidak langsung kepada IP yang kita miliki

<img width="597" alt="Screenshot 2023-12-01 at 07 03 44" src="https://github.com/Subzero16/TUGAS/assets/69718826/0ee5d56b-c504-4cde-9252-1ceb20a14494">

Cloud Firewall
> Mirip dengan Proxy Firewall tetapi lebih mudah karena kita tidak perlu menyediakan on premis server sebagai server tumbal karena traffic sudah dihandle oleh perusahaan yang lebih powerfull dalam sisi INFRASTRUKTUR SERVER (IaaS / FaaS)

![1_LTykvnM6hpJkYg7m2zkwWQ](https://github.com/Subzero16/TUGAS/assets/69718826/bb12a76f-656c-4d28-a246-9c1124401a32)


Fungsi Firewall
> Content Filtering
> Port Configuration
> Anti Spam
> > File protection


'''''''''''''''''''''''''''''''''''''
