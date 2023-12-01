1. Jelaskan apa itu web server dan jelaskan bagaimana cara kerjanya

> Merupakan layanan yang menerima permintaan data HTTP atau HTTPS dari client (browser) lalu merespon dengan menampilan konten yang tersedia atau respon lain jika gagal akses (Response Code 50*/40*/30*/20*)

CLIENT REQUEST > WEB SERVER > SERVER APP1 / SERVER APP2 > SERVER DATABASE 1/ SERVER DATABASE 2

2. buatlah reverse proxy sederhana menggunakan nginx, lalu untuk application nya kalian bisa clone application di link berikut Dumbsound App (https://github.com/RizqyAlvindra/dumbsound) 

git clone 

![Screenshot from 2023-12-01 04-51-02](https://github.com/Subzero16/TUGAS/assets/69718826/d3c8d112-c6f0-49be-aaa3-a65938f1a636)

npm install dumbsound

![Screenshot from 2023-12-01 04-51-05](https://github.com/Subzero16/TUGAS/assets/69718826/b3e839b4-b61d-40d2-bfd6-dc8c5e7a3611)

buka webserver localhost:3000

<img width="1412" alt="Screenshot 2023-12-01 at 07 27 49" src="https://github.com/Subzero16/TUGAS/assets/69718826/4b9853c0-9fd5-42ee-b811-9a48870eb097">

REVERSE IP PROXY

<img width="554" alt="Screenshot 2023-12-01 at 07 28 45" src="https://github.com/Subzero16/TUGAS/assets/69718826/683545aa-de80-4ec0-8a7b-d45b9c80e8e1">

SETTING nginx.conf

![Screenshot from 2023-12-01 06-08-04](https://github.com/Subzero16/TUGAS/assets/69718826/6c4996c7-a0b5-49dc-84f7-eed023ffd682)

TESTING NGINX & Error Check

<img width="535" alt="Screenshot 2023-12-01 at 07 29 44" src="https://github.com/Subzero16/TUGAS/assets/69718826/4e75091a-b2fa-46c5-b71f-692856445401">

WEBSERVER GO LIVE

![Screenshot from 2023-12-01 06-12-04](https://github.com/Subzero16/TUGAS/assets/69718826/f092b359-7a31-48b7-8a58-5efaa677893a)


3. buatlah -+ 2 atau 3 buah vm (1 nginx, 2 aplikasi) untuk mengimplementasikan loadbalancing applikasi yang ada di nomer 2

Membuat 3 VM menggunakan multipass
webserver >>> hagi2
appserver >>> hagi3 & hagi4

<img width="609" alt="Screenshot 2023-12-01 at 07 34 40" src="https://github.com/Subzero16/TUGAS/assets/69718826/06be0cee-a52c-4634-a144-101775b57a77">

INSTALL WEBSERVER pada hagi2, lalu setting Nginx.conf serta restart

<img width="739" alt="Screenshot 2023-12-01 at 07 36 06" src="https://github.com/Subzero16/TUGAS/assets/69718826/5c7c5a5c-61b3-45ab-98df-3c081ecd0a79">

Cek system alive pada 10.54.176.162:3000

![Screenshot from 2023-12-01 06-12-04](https://github.com/Subzero16/TUGAS/assets/69718826/90642bfc-a889-4041-8a59-c95c4a28b66d)

lalu pada server hagi3 install kembali 

![Screenshot from 2023-12-01 06-24-37](https://github.com/Subzero16/TUGAS/assets/69718826/b015db36-ec74-446e-a52a-eece6a2922ff)


SERVER hagi3 GO LIVE

![Screenshot from 2023-12-01 06-25-41](https://github.com/Subzero16/TUGAS/assets/69718826/5b0ee96f-f4ca-4d56-b216-7ddc8ee71714)

Konfigurasi Upstream pada server hagi2

<img width="273" alt="Screenshot 2023-12-01 at 07 44 20" src="https://github.com/Subzero16/TUGAS/assets/69718826/5f5c46e9-5856-4753-8fc1-cad6e7dd5f1d">

buat konfigurasi DNS pada local kita (alternatif domain)

<img width="503" alt="Screenshot 2023-12-01 at 07 43 37" src="https://github.com/Subzero16/TUGAS/assets/69718826/4b479dfd-8007-4620-a59c-569153af653f">


MATIKAN SERVER hagi3 dan hanya menyalakan server hagi2

![Screenshot from 2023-12-01 06-32-44](https://github.com/Subzero16/TUGAS/assets/69718826/e4474c49-ba19-4a9a-abf9-259f6fcdd45c)


MATIKAN SERVER hagi2 dan hanya menyalakan server hagi3

![Screenshot from 2023-12-01 06-32-44](https://github.com/Subzero16/TUGAS/assets/69718826/6626ee8e-228c-462b-94fa-8813960e3bd0)


============ done =============
