Nama : Aulia Rachmi Liunsanda
NIM : 235410009
Kelas : INformatika 1

<img width="933" height="792" alt="image" src="https://github.com/user-attachments/assets/cf1b10b3-f7b5-431e-8ec9-edb0ae3fd3fc" />
Hash merupakan representasi unik dari suatu data yang digunakan untuk memastikan integritas informasi. Setiap perubahan pada data, bahkan hanya satu karakter saja, akan menghasilkan nilai hash yang berbeda secara signifikan. Dalam teknologi blockchain, hash berperan penting untuk menjaga keaslian dan konsistensi data sehingga setiap perubahan dapat terdeteksi dengan mudah. Salah satu algoritma hash yang banyak digunakan adalah SHA-256, yang menghasilkan nilai hash sepanjang 64 karakter heksadesimal.

CoreBlockchain.py 
<img width="785" height="670" alt="image" src="https://github.com/user-attachments/assets/0cffacda-172d-4d52-a0a1-bb4e19894022" />

UtdiBlockchain.py 
<img width="875" height="530" alt="image" src="https://github.com/user-attachments/assets/be2a3f4d-c6a3-462c-848e-40e052995b37" />

blockchain_demo_01.py
<img width="827" height="368" alt="image" src="https://github.com/user-attachments/assets/248c5b7c-3db3-44c4-bb11-003d8f928ec0" />

jalankan
<img width="935" height="516" alt="image" src="https://github.com/user-attachments/assets/09e3d626-61c3-4013-86a1-b1fd49b63f21" />

pembahasan:
CoreBlockchain.py merupakan kelas inti yang merepresentasikan sebuah blok dalam blockchain. Pada method __init__(), sistem akan membuat objek blok baru dengan menyimpan informasi penting seperti indeks blok, waktu pembuatan (timestamp), data transaksi, hash dari blok sebelumnya, nilai nonce, serta hash blok saat ini. Selain itu, method count_hash() digunakan untuk menghasilkan nilai hash blok menggunakan algoritma SHA-256 berdasarkan seluruh isi blok. Hash yang dihasilkan berfungsi sebagai identitas unik blok sekaligus mekanisme untuk menjaga integritas data agar setiap perubahan pada isi blok dapat terdeteksi.

UtdiBlockchain.py berfungsi sebagai pengelola rangkaian blockchain yang terdiri dari beberapa blok yang saling terhubung. Method init_genesis_block() digunakan untuk membuat Genesis Block, yaitu blok pertama dalam blockchain yang menjadi titik awal pembentukan rantai blok. Sementara itu, method `add_block()` digunakan untuk menambahkan blok baru ke dalam blockchain dengan cara menghubungkan hash blok sebelumnya ke blok yang akan ditambahkan. Mekanisme ini memastikan setiap blok memiliki keterkaitan yang kuat sehingga keamanan dan konsistensi data dalam blockchain dapat terjaga.

blockchain_demo_01.py merupakan program utama yang digunakan untuk mendemonstrasikan cara kerja blockchain secara sederhana. Program ini bertugas membuat objek blockchain, menambahkan beberapa data transaksi ke dalam blok baru, serta menampilkan seluruh isi blockchain yang telah terbentuk. Melalui program ini, pengguna dapat memahami proses pembentukan blok, hubungan antarblok melalui hash, dan bagaimana data disimpan secara berurutan dalam sebuah blockchain.


