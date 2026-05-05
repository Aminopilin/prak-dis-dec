<h4> Nama : Aulia Rachmi Liunsanda <br>
NIM : 235410009  <br>
Kelas : Informatika 1  <br> <h4>
 <br>
<H1>Distributed File System-HDFS</H1>
 <br>
<b>install JDK  <br>
<img width="1082" height="110" alt="image" src="https://github.com/user-attachments/assets/52ead82a-232b-427c-bd3b-eafd1020efb5" />  <br>

 Install hadoop  <br>
<img width="472" height="38" alt="image" src="https://github.com/user-attachments/assets/fb150371-513c-4743-a5e4-3480c8b3aa60" />  <br>
<img width="595" height="912" alt="image" src="https://github.com/user-attachments/assets/f1871e30-d9da-4262-99ba-58f00298b897" />  <br>

Set Environment variable  <br>
<img width="436" height="27" alt="image" src="https://github.com/user-attachments/assets/6b284292-026f-4dd1-b7a6-e5012645b1f8" />  <br>
<img width="825" height="70" alt="image" src="https://github.com/user-attachments/assets/c628f1ed-1649-4574-84cd-5819ae740936" />  <br>
<img width="465" height="25" alt="image" src="https://github.com/user-attachments/assets/e77a2bfc-43d6-4bbf-a0b9-e0d672040c78" />  <br>

 <br> konfigurasi SSH
<img width="739" height="508" alt="image" src="https://github.com/user-attachments/assets/36d074c9-6ede-41fa-a095-235262026e8f" />  <br>
test  <br>
<img width="931" height="367" alt="image" src="https://github.com/user-attachments/assets/281c7108-d0cb-4f21-a2ab-1ae1d8ef08e3" />  <br>

Konfigurasi apache hadoop  <br>
hdfs-site.xml
<img width="951" height="645" alt="image" src="https://github.com/user-attachments/assets/42fb48f9-41c0-47ab-912a-3ae470adf537" />  <br>
core-site.xml 
<img width="941" height="861" alt="image" src="https://github.com/user-attachments/assets/c2bd8abf-9324-4a38-975c-f7a57aebdee8" />  <br>
mapred-site.xml 
<img width="949" height="763" alt="image" src="https://github.com/user-attachments/assets/9647338d-398f-450a-a341-4f06d8f070a8" />  <br>
yarn-site.xml 
<img width="940" height="937" alt="image" src="https://github.com/user-attachments/assets/08b63d84-b7af-4be3-8c80-02dda9ff4429" />  <br>

Set java hadoop  <br>
<img width="866" height="255" alt="image" src="https://github.com/user-attachments/assets/5167b978-09b7-4109-ae20-a4edf1a79b94" />  <br>

Format NameNode  <br>
<img width="951" height="278" alt="image" src="https://github.com/user-attachments/assets/d831d07b-6ef8-44bf-90ec-6e383aa59efb" />  <br>
<img width="1919" height="922" alt="image" src="https://github.com/user-attachments/assets/a1797c06-99ec-4399-aa3b-828d922bfdde" />  <br>

Jalankan hadoop  <br>
<img width="570" height="185" alt="image" src="https://github.com/user-attachments/assets/90f5ba83-d3fb-40c5-afe0-3f1c0d58ac8d" />  <br>
cek browser  <br>
http://localhost:9870
<img width="1917" height="973" alt="image" src="https://github.com/user-attachments/assets/b79eadfb-c30c-4481-a9da-9e6570dd5156" />  <br>

TUGAS  <br>
buat direktori baru
<img width="941" height="145" alt="image" src="https://github.com/user-attachments/assets/9429a04e-b149-4579-8160-8c5bd9fd55e2" />  <br>
Cari 3 file .csv di Internet dan kemudian copykan 3 file tersebut ke direktori yang baru 
saja anda buat pada tugas 1 di atas. <br>
<img width="1365" height="479" alt="image" src="https://github.com/user-attachments/assets/663ff0f9-b2a6-4668-a9ee-ae3aa576e58a" />  
<img width="1855" height="237" alt="image" src="https://github.com/user-attachments/assets/fbab4033-9bc9-40b0-a2cf-54dcac4d9c5d" />  <br>

mematikan HDFS <br>
<img width="486" height="112" alt="image" src="https://github.com/user-attachments/assets/918f8c61-da2c-410f-b4e2-fe8a229b892a" />  
<img width="314" height="89" alt="image" src="https://github.com/user-attachments/assets/04d0bb4c-51b3-40f3-b8dc-8b9e01192c60" />  <br> </b>

<b> pembahasan </b> <br>
Pada praktikum kali ini dilakukan implementasi sistem penyimpanan terdistribusi menggunakan Apache Hadoop dengan memanfaatkan HDFS (Hadoop Distributed File System). Praktikum diawali dengan menyiapkan lingkungan sistem seperti instalasi JDK, Hadoop, serta konfigurasi SSH agar proses komunikasi dapat berjalan dengan lancar. Selanjutnya dilakukan konfigurasi pada beberapa file penting seperti *core-site.xml* dan *hdfs-site.xml* untuk menentukan alamat NameNode dan pengaturan replikasi data. Setelah itu dilakukan proses formatting NameNode sebagai tahap inisialisasi, kemudian menjalankan daemon HDFS agar sistem dapat digunakan. Pada tahap akhir, dilakukan pengujian dengan membuat direktori dan mengunggah file dataset ke dalam HDFS, sehingga dapat disimpulkan bahwa sistem ini mampu mengelola penyimpanan data secara terdistribusi, efisien, dan mendukung kebutuhan pengolahan data skala besar .
