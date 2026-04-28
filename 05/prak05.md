Nama : Aulia Rachmi Liunsanda <br>
NIM : 235410009 <br>
Kelas : Informatika 1 <br>

Pembuatan Folder & Setup Project <br>
<img width="940" height="346" alt="image" src="https://github.com/user-attachments/assets/4554608f-c3b7-4656-9d4b-a388dd0694e3" /> <br>
Pada bagian ini dibuat folder kerja (misalnya workspace-05) yang berfungsi sebagai tempat penyimpanan project. <br>
 <br>
 Pembuatan Virtual Environment Python <br>
<img width="940" height="121" alt="image" src="https://github.com/user-attachments/assets/ab7f5f1d-b483-4023-868e-e4d104dabb86" /> <br>
Tahapan ini menunjukkan proses pembuatan virtual environment menggunakan Python <br>

Install Blacksheep dan Blacksheep-CLI <br>
<img width="940" height="1151" alt="image" src="https://github.com/user-attachments/assets/44781e2a-0434-4dd2-8ee3-bb12c043a33f" /> <br>
 <img width="940" height="934" alt="image" src="https://github.com/user-attachments/assets/094731bd-8a1e-4ded-b49c-35c69cf9f03d" /> <br>
Pada bagian ini dilakukan instalasi framework Blacksheep dan CLI-nya menggunakan pip. Framework ini digunakan untuk membuat aplikasi web berbasis ASGI. Hasil install menampilkan daftar package yang berhasil terpasang, yang menunjukkan bahwa environment sudah siap untuk membuat aplikasi. <br>
Pembuatan Project Blacksheep <br>
<img width="841" height="383" alt="image" src="https://github.com/user-attachments/assets/cea2ed32-0f0c-4d4b-a6bb-f1c97537eaf3" /> <br>
Screenshot ini menunjukkan proses pembuatan aplikasi menggunakan CLI Blacksheep. Aplikasi yang dibuat masih berupa template sederhana (default). Tujuannya adalah sebagai contoh untuk memahami konsep load balancing, bukan untuk pengembangan fitur kompleks. <br>

 Install Requirements.txt<br>
<img width="940" height="477" alt="image" src="https://github.com/user-attachments/assets/0ba88716-e33c-4235-8ea0-e2b640b9d0de" /> <br>
Pada tahap ini dilakukan instalasi dependensi tambahan dari file requirements.txt. File ini berisi daftar library yang dibutuhkan aplikasi agar dapat berjalan dengan baik. Di Windows biasanya menggunakan perintah: pip install -r requirements.txt

<img width="940" height="198" alt="image" src="https://github.com/user-attachments/assets/c1bfd669-dfbb-42b2-abcf-f9b71bceb73a" /> <br>
Aplikasi Berjalan (localhost:44777)
<img width="940" height="503" alt="image" src="https://github.com/user-attachments/assets/ba48a816-2f1d-4ad5-901a-945ad08a2673" /> <br>
Screenshot ini menunjukkan bahwa aplikasi berhasil dijalankan secara lokal menggunakan server bawaan (uvicorn). Akses dilakukan melalui browser ke http://localhost:44777. Jika halaman tampil, berarti aplikasi sudah berjalan dengan baik sebelum masuk ke tahap containerisasi.

Terminal Server Running
<img width="940" height="344" alt="image" src="https://github.com/user-attachments/assets/50046fed-ee16-41b9-b3c4-52b81b238799" /> <br>
Pada bagian ini terlihat log di terminal saat server berjalan. Log ini menunjukkan bahwa server aktif dan siap menerima request. Informasi seperti port, status running, dan request yang masuk dapat dilihat di sini. Ini penting untuk memastikan tidak ada error saat menjalankan aplikasi.

Dockerfile Blacksheep
<img width="940" height="604" alt="image" src="https://github.com/user-attachments/assets/af704ed8-0e9a-452e-a7a9-e1f20959f926" /> <br>

<img width="940" height="853" alt="image" src="https://github.com/user-attachments/assets/68cdb3d6-150e-4610-b55a-95e5aa8e3802" /> <br>
