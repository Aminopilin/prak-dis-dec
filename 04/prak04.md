Nama  : Aulia Rachmi Liunsanda <br>
NIM  : 235410009 <br>
Kelas  : Informatika 1 <br>

Konsistensi dan Replikasi pada Sistem Terdistribusi  <br>
4.1 Streaming Replication Menggunakan PostgreSQL <br>
4.1.1 Prasyarat <br>
<img width="543" height="129" alt="image" src="https://github.com/user-attachments/assets/45e2c58e-ec72-461a-8ba6-9859ce81f811" />
 <br>
<img width="1895" height="1017" alt="image" src="https://github.com/user-attachments/assets/93dd4434-275c-4728-a861-115a6a0b8b91" /> <br>


4.1.2 Struktur Direktori dan FIle <br>
<img width="769" height="335" alt="image" src="https://github.com/user-attachments/assets/27bb0253-a7b7-4d38-9b38-b658ba6f7ffe" />
Struktur folder ini berisi file utama yang digunakan untuk konfigurasi replikasi PostgreSQL. File SQL digunakan untuk inisialisasi database, docker-compose untuk menjalankan container, dan env.sh untuk shortcut command.

00_init.sql
<img width="877" height="120" alt="image" src="https://github.com/user-attachments/assets/47b680d2-35f9-4be9-b551-364785b65062" /> <br>
File ini berfungsi untuk membuat user khusus replikasi bernama “replicator”. Selain itu, dibuat juga replication slot untuk menjaga sinkronisasi data antara primary dan replica. Slot ini memastikan data tidak hilang saat proses replikasi berlangsung.

docker-compose.yaml <br>
<img width="960" height="968" alt="image" src="https://github.com/user-attachments/assets/df981c19-b1ae-416c-9720-6e355727fefc" /> <br>
<img width="1183" height="342" alt="image" src="https://github.com/user-attachments/assets/db81f8f2-5d9b-4063-b2ac-3afc47894e05" /> <br>
File ini adalah inti dari konfigurasi sistem, berisi dua service yaitu primary dan replica. Primary bertugas menerima read-write, sedangkan replica hanya read. Konfigurasi seperti wal_level dan hot_standby mengaktifkan fitur replikasi PostgreSQL.

env.sh
<img width="551" height="197" alt="image" src="https://github.com/user-attachments/assets/11f98584-9997-44b3-9602-88fb77f726a1" /> <br>
File ini berisi alias untuk mempermudah penggunaan perintah Docker. Dengan alias, pengguna tidak perlu mengetik command panjang berulang kali. 



4.1.3 Menjalankan docker-compose <br>
<img width="947" height="151" alt="image" src="https://github.com/user-attachments/assets/789bd11f-f6b7-437e-8f27-7391e30a3d95" />
 <br>
Saat pertama kali dijalankan, Docker akan melakukan pull image PostgreSQL dari Docker Hub. Proses ini menunjukkan container sedang dipersiapkan.

<img width="936" height="236" alt="image" src="https://github.com/user-attachments/assets/752f2597-5ce6-4ee2-80c9-d1e0138f6834" />
 <br>
Screenshot ini menunjukkan bahwa terdapat dua container aktif: primary dan replica. Status “healthy” menandakan bahwa PostgreSQL berjalan dengan baik.

4.1.4 Pengujian <br>
<img width="444" height="206" alt="image" src="https://github.com/user-attachments/assets/f83121d9-039e-4081-b166-c37a7e88ad1f" />

<img width="461" height="122" alt="image" src="https://github.com/user-attachments/assets/01ea4b05-3a81-4a1d-939c-4ab85923eddb" />

<img width="928" height="122" alt="image" src="https://github.com/user-attachments/assets/8817e20f-31be-4d4b-bb04-cbfcd819e803" />

<img width="926" height="143" alt="image" src="https://github.com/user-attachments/assets/fed65a32-fe54-4f9b-8b02-7fec065bc058" />

<img width="929" height="303" alt="image" src="https://github.com/user-attachments/assets/352c00dd-912f-4532-bf17-16af32647582" />


4.1.5 High-Availability<br>

4.2 Replikasi Master-Master Menggunakan Apache Ignite <br>
4.2.1 Prasyarat<br>
4.2.2. Struktur direktori dan file<br>
4.2.3 Menjalankan docker-compose <br>
4.2.4 Inisialisasi cluster<br>
4.2.5 Eksekusi perintah-perintah SQL <br>
