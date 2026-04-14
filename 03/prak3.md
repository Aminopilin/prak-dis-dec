Nama  : Aulia Rachmi Liunsanda <br>
NIM  : 235410009 <br>
Kelas  : Iinformatika 1 <br>

Sinkronisasi pada Sistem Terdistribusi <br>
3.1 Sinkronisasi Waktu <br>
<img width="969" height="606" alt="image" src="https://github.com/user-attachments/assets/103e292a-0d18-4d79-acf8-5df57a2d4492" /> <br>
Sinkronisasi waktu dilakukan dengan menghubungkan client ke server NTP untuk menyamakan waktu sistem. Chrony/NetTime akan mengirim request, menerima waktu server, lalu menghitung selisih (offset). Sistem kemudian menyesuaikan waktu secara bertahap agar tidak terjadi lonjakan.  <br>
3.2 Vector Clock <br>
<img width="703" height="972" alt="image" src="https://github.com/user-attachments/assets/a9ae29ae-4515-4ef4-b675-cc6214337264" />  <br>
<img width="630" height="815" alt="image" src="https://github.com/user-attachments/assets/61760d92-2b17-40a8-983f-71cb5d54a11e" />  <br>
output  <br>
<img width="1153" height="262" alt="image" src="https://github.com/user-attachments/assets/5a71c5e3-9c93-4e5f-a175-f3993b4c0648" />  <br>
Program ini menunjukkan bagaimana setiap proses memiliki vector clock untuk mencatat urutan event. Setiap event (internal, send, receive) akan mengupdate nilai clock sesuai aturan. Output memperlihatkan hubungan sebab-akibat (causality) antar event.<br>
<br>
vectorClock <br>
<img width="618" height="354" alt="image" src="https://github.com/user-attachments/assets/9486434e-b4a2-4195-b921-84939ed1bc4b" />  <br>
test vectorclock <br>
<img width="627" height="257" alt="image" src="https://github.com/user-attachments/assets/a47234f7-56a0-41a6-93b3-b32d3c159269" /> <br>
output <br>
<img width="1239" height="100" alt="image" src="https://github.com/user-attachments/assets/8b629ceb-462d-4973-9d32-df548a5428cd" /> <br>
Class VectorClock dibuat untuk membungkus logika vector clock agar bisa digunakan ulang. Modul ini menyediakan fungsi seperti increment, update, dan compare antar clock. Contoh penggunaan menunjukkan bagaimana beberapa proses dapat berkomunikasi dan memperbarui waktu logisnya. <br>
<br>
3.3 Problem Tanpa Sinkronisasi <br>
<img width="602" height="655" alt="image" src="https://github.com/user-attachments/assets/96a0a05a-e25b-4994-a1a9-1fba6b3b28ed" />  <br>
output <br>
<img width="1246" height="238" alt="image" src="https://github.com/user-attachments/assets/81301e58-94af-4380-8c8c-e7f91b0dd548" /> <br>
<img width="1246" height="159" alt="image" src="https://github.com/user-attachments/assets/3fdb620f-cc84-4dce-9e74-2b6364393375" /> <br>
Program ini menjalankan beberapa thread secara bersamaan tanpa sinkronisasi. Output bisa berbeda setiap kali dijalankan karena urutan eksekusi thread tidak deterministik. Hal ini terjadi karena CPU menjadwalkan thread secara acak.<br>
<br>
3.3.1 Data Race / Race Conditions <br>
<img width="640" height="363" alt="image" src="https://github.com/user-attachments/assets/13d3af36-d5c3-4542-89cf-3738e498c2e9" /> <br>
output <br>
<img width="1232" height="75" alt="image" src="https://github.com/user-attachments/assets/0caba45e-416e-447c-8c06-f24474ee34fd" /> <br>
Race condition terjadi ketika beberapa thread mengakses dan memodifikasi data yang sama secara bersamaan. Tanpa mekanisme penguncian, nilai data bisa tidak sesuai harapan. Output program sering berubah karena interleaving eksekusi thread. Ini menyebabkan inkonsistensi data.<br>

<img width="657" height="422" alt="image" src="https://github.com/user-attachments/assets/97523d98-c958-4419-9ebb-07c0ba45b4ff" /> <br>
output <br>
<img width="1233" height="54" alt="image" src="https://github.com/user-attachments/assets/36aa96aa-bf58-4491-8e85-91c103a4154d" /> <br>
Program ini menggunakan mekanisme lock untuk menghindari akses bersamaan ke data. Hanya satu thread yang bisa mengakses resource dalam satu waktu. Hal ini membuat hasil program menjadi konsisten. Race condition tidak terjadi karena ada kontrol sinkronisasi.<br>
<br>
3.3.2 Deadlock <br>
<img width="775" height="580" alt="image" src="https://github.com/user-attachments/assets/d843d0cb-b8e5-4466-9538-b0772ed8f179" /> <br>
output <br>
<img width="1166" height="63" alt="image" src="https://github.com/user-attachments/assets/0d3e90a6-13ee-4a15-b364-855c47f70060" /> <br>
Deadlock terjadi ketika dua atau lebih thread saling menunggu resource yang dikunci oleh thread lain. Akibatnya, semua thread berhenti dan tidak bisa melanjutkan eksekusi. Program tampak “hang” atau tidak selesai.<br>
<br>
<img width="625" height="880" alt="image" src="https://github.com/user-attachments/assets/93748b0f-cedc-4681-8c6f-111e6db06518" /> <br>
output <br>
<img width="1186" height="177" alt="image" src="https://github.com/user-attachments/assets/4a9ffad2-b89e-481e-a7c3-15cbc7e93dd3" /> <br>
Deadlock dihindari dengan mengatur urutan penguncian resource atau menggunakan strategi tertentu. Thread tidak saling menunggu secara melingkar. Program dapat berjalan sampai selesai tanpa berhenti.<br>
<br>
3.4 Algoritma Raft <br>
<img width="743" height="945" alt="image" src="https://github.com/user-attachments/assets/743f9408-af3a-4179-90eb-73f22c5860fb" /> <br>
<img width="698" height="860" alt="image" src="https://github.com/user-attachments/assets/bfe787f9-8ee1-4433-b40f-9319ef291db5" /> <br>
<img width="950" height="238" alt="image" src="https://github.com/user-attachments/assets/e7900020-1bcb-469b-8d34-691d59fc6138" /> <br>
output <br>
<img width="417" height="839" alt="image" src="https://github.com/user-attachments/assets/bcc39ece-a50f-4080-90f5-f52c94bd7634" /> <br>
<img width="324" height="973" alt="image" src="https://github.com/user-attachments/assets/a8ed7ba4-6517-4490-8c64-5b44779cb23c" /> <br>
<img width="394" height="95" alt="image" src="https://github.com/user-attachments/assets/11c89580-9b50-4491-9eaf-618f4cacf417" /> <br>

Program ini mensimulasikan algoritma Raft untuk memilih leader dalam sistem terdistribusi. Node akan melakukan election dengan mengirim vote ke node lain. Node dengan suara terbanyak menjadi leader. Output menunjukkan proses pemilihan dan pergantian leader secara sederhana.

<img width="310" height="166" alt="image" src="https://github.com/user-attachments/assets/01545848-936c-4144-b1d7-eedc8f8a2164" /> <br>
<img width="376" height="208" alt="image" src="https://github.com/user-attachments/assets/fd23dfc3-1e36-4893-bd41-cacbc3d02557" /> <br>
output
<img width="1175" height="88" alt="image" src="https://github.com/user-attachments/assets/1e192188-6f29-4614-ba77-78301b5596e7" /> <br>
Program diubah menjadi modul agar bisa digunakan ulang dalam simulasi lain. Modul menyediakan fungsi untuk node, voting, dan leader election. Contoh simulasi menunjukkan bagaimana beberapa node berinteraksi.<br>



