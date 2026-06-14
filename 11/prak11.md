Nama : Aulia Rachmi Liunsanda <br>
NIM : 235410009<br>
Kelas : INformatika 1<br>

<img width="933" height="792" alt="image" src="https://github.com/user-attachments/assets/cf1b10b3-f7b5-431e-8ec9-edb0ae3fd3fc" /> <br>
Hash merupakan representasi unik dari suatu data yang digunakan untuk memastikan integritas informasi. Setiap perubahan pada data, bahkan hanya satu karakter saja, akan menghasilkan nilai hash yang berbeda secara signifikan. Dalam teknologi blockchain, hash berperan penting untuk menjaga keaslian dan konsistensi data sehingga setiap perubahan dapat terdeteksi dengan mudah. Salah satu algoritma hash yang banyak digunakan adalah SHA-256, yang menghasilkan nilai hash sepanjang 64 karakter heksadesimal.<br>

CoreBlockchain.py <br>
<img width="785" height="670" alt="image" src="https://github.com/user-attachments/assets/0cffacda-172d-4d52-a0a1-bb4e19894022" /><br>

UtdiBlockchain.py <br>
<img width="875" height="530" alt="image" src="https://github.com/user-attachments/assets/be2a3f4d-c6a3-462c-848e-40e052995b37" /><br>

blockchain_demo_01.py<br>
<img width="827" height="368" alt="image" src="https://github.com/user-attachments/assets/248c5b7c-3db3-44c4-bb11-003d8f928ec0" /><br>

jalankan<br>
<img width="935" height="516" alt="image" src="https://github.com/user-attachments/assets/09e3d626-61c3-4013-86a1-b1fd49b63f21" /><br>

pembahasan:<br>
CoreBlockchain.py merupakan kelas inti yang merepresentasikan sebuah blok dalam blockchain. Pada method __init__(), sistem akan membuat objek blok baru dengan menyimpan informasi penting seperti indeks blok, waktu pembuatan (timestamp), data transaksi, hash dari blok sebelumnya, nilai nonce, serta hash blok saat ini. Selain itu, method count_hash() digunakan untuk menghasilkan nilai hash blok menggunakan algoritma SHA-256 berdasarkan seluruh isi blok. Hash yang dihasilkan berfungsi sebagai identitas unik blok sekaligus mekanisme untuk menjaga integritas data agar setiap perubahan pada isi blok dapat terdeteksi.<br>

UtdiBlockchain.py berfungsi sebagai pengelola rangkaian blockchain yang terdiri dari beberapa blok yang saling terhubung. Method init_genesis_block() digunakan untuk membuat Genesis Block, yaitu blok pertama dalam blockchain yang menjadi titik awal pembentukan rantai blok. Sementara itu, method `add_block()` digunakan untuk menambahkan blok baru ke dalam blockchain dengan cara menghubungkan hash blok sebelumnya ke blok yang akan ditambahkan. Mekanisme ini memastikan setiap blok memiliki keterkaitan yang kuat sehingga keamanan dan konsistensi data dalam blockchain dapat terjaga.<br>

blockchain_demo_01.py merupakan program utama yang digunakan untuk mendemonstrasikan cara kerja blockchain secara sederhana. Program ini bertugas membuat objek blockchain, menambahkan beberapa data transaksi ke dalam blok baru, serta menampilkan seluruh isi blockchain yang telah terbentuk. Melalui program ini, pengguna dapat memahami proses pembentukan blok, hubungan antarblok melalui hash, dan bagaimana data disimpan secara berurutan dalam sebuah blockchain. <br>

<img width="1917" height="962" alt="image" src="https://github.com/user-attachments/assets/7d980670-81b0-4c9b-a5c0-d8e41faedcdc" /><br>

<img width="1918" height="967" alt="image" src="https://github.com/user-attachments/assets/c56160b3-efa2-4cab-b419-ed12d8cc2357" /><br>

<img width="1912" height="967" alt="image" src="https://github.com/user-attachments/assets/03a139d7-7e15-4dc2-b80b-3ae85e87d8ed" /><br>

<img width="1918" height="973" alt="image" src="https://github.com/user-attachments/assets/c7844ba1-8057-4c02-a56f-cce1364bbe51" /><br>

<img width="592" height="843" alt="image" src="https://github.com/user-attachments/assets/10c04018-614e-4d39-abcf-90b2982e53dc" /><br>

<img width="1918" height="961" alt="image" src="https://github.com/user-attachments/assets/6bb57b9f-9ee6-4b99-85d5-4827e3c6f198" /><br>

<img width="1007" height="737" alt="image" src="https://github.com/user-attachments/assets/c05383a5-1034-4ce7-8a21-05f22f24e8ce" /><br>

Tugas 3 <br>
1. Implementasi Blockchain pada Berbagai Bidang<br>
a. DApps (Decentralized Applications)<br>
DApps atau Decentralized Applications adalah aplikasi yang dibangun dan dijalankan di atas jaringan blockchain tanpa bergantung pada server pusat. Berbeda dengan aplikasi konvensional, DApps memanfaatkan smart contract untuk mengelola proses bisnis secara otomatis dan transparan. Karena data tersimpan secara terdistribusi pada banyak node, aplikasi menjadi lebih aman, transparan, dan sulit dimanipulasi oleh pihak tertentu. DApps banyak digunakan dalam bidang keuangan, permainan (gaming), media sosial, hingga sistem pemungutan suara digital.<br>

b. NFT (Non-Fungible Token)<br>
NFT (Non-Fungible Token) merupakan aset digital unik yang kepemilikannya tercatat secara permanen di blockchain. Setiap NFT memiliki identitas dan metadata yang berbeda sehingga tidak dapat dipertukarkan secara setara seperti mata uang kripto biasa. Teknologi ini memungkinkan pembuktian kepemilikan dan keaslian aset digital secara transparan. Contoh penerapan NFT meliputi karya seni digital, item dalam permainan (game items), koleksi digital, tiket acara, dan sertifikat digital.<br>

c. DEX (Decentralized Exchange)<br>
DEX (Decentralized Exchange) adalah platform pertukaran aset kripto yang beroperasi secara terdesentralisasi tanpa memerlukan perantara seperti bank atau broker. Seluruh transaksi dilakukan melalui smart contract, sehingga pengguna tetap memiliki kendali penuh atas aset mereka. Keunggulan DEX meliputi keamanan yang lebih baik, privasi pengguna yang lebih terjaga, serta biaya operasional yang relatif rendah. Contoh platform DEX yang populer adalah Uniswap dan PancakeSwap.

d. Tokenization<br>
Tokenisasi (Tokenization) adalah proses mengubah kepemilikan suatu aset fisik maupun digital menjadi token yang tercatat di blockchain. Dengan tokenisasi, aset dapat diperdagangkan secara lebih mudah, transparan, dan efisien. Teknologi ini memungkinkan pembagian kepemilikan aset menjadi bagian-bagian kecil sehingga lebih mudah diakses oleh investor. Contoh aset yang dapat ditokenisasi antara lain tanah, rumah, saham perusahaan, obligasi, hingga karya seni bernilai tinggi.<br>

e. Stablecoin<br>
Stablecoin adalah jenis mata uang kripto yang dirancang untuk memiliki nilai yang stabil dengan cara dipatok pada aset tertentu, seperti mata uang fiat, emas, atau instrumen keuangan lainnya. Tujuan utama stablecoin adalah mengurangi volatilitas harga yang umum terjadi pada aset kripto. Stablecoin banyak digunakan sebagai alat transaksi, penyimpanan nilai, serta sarana transfer dana lintas negara. Contoh stablecoin yang paling populer adalah Tether (USDT) dan USD Coin (USDC).<br>

2. Peranti Pengembangan DApps pada Ethereum <br>
Dalam pengembangan DApps berbasis Ethereum, saya memilih beberapa peranti yang telah menjadi standar industri karena kemudahan penggunaan, kelengkapan fitur, dan dukungan komunitas yang luas.
1. Solidity<br>
Solidity merupakan bahasa pemrograman utama yang digunakan untuk mengembangkan smart contract pada blockchain Ethereum. Bahasa ini dirancang khusus untuk membuat logika bisnis yang dapat berjalan secara otomatis dan aman di jaringan blockchain.<br>
2. Remix IDE<br>
Remix IDE adalah lingkungan pengembangan berbasis web yang menyediakan berbagai fitur untuk menulis, mengompilasi, menguji, dan melakukan deployment smart contract. Remix sangat cocok digunakan oleh pemula karena tidak memerlukan proses instalasi yang rumit.<br>
3. MetaMask<br>
MetaMask berfungsi sebagai dompet digital (wallet) sekaligus penghubung antara aplikasi dengan jaringan Ethereum. Dengan MetaMask, pengguna dapat mengelola aset kripto, menandatangani transaksi, dan berinteraksi dengan DApps secara aman.
4. Hardhat<br>
Hardhat merupakan framework modern yang menyediakan berbagai fitur penting untuk pengembangan smart contract, seperti testing, debugging, simulasi jaringan lokal, serta otomatisasi proses deployment. Hardhat sangat membantu dalam membangun aplikasi blockchain yang lebih kompleks dan profesional.<br>
5. Node.js<br>
Node.js digunakan sebagai lingkungan eksekusi JavaScript yang mendukung berbagai tool pengembangan Ethereum. Banyak framework dan pustaka blockchain modern bergantung pada Node.js untuk menjalankan proses pengembangan dan pengujian aplikasi.<br>
Alasan Pemilihan Peranti<br>
Pemilihan kombinasi Solidity, Remix IDE, MetaMask, Hardhat, dan Node.js didasarkan pada beberapa pertimbangan utama, yaitu bersifat gratis dan open source, memiliki dokumentasi yang lengkap, didukung komunitas yang besar, serta banyak digunakan dalam industri blockchain. Selain itu, peranti-peranti tersebut memudahkan proses pengujian pada jaringan testnetseperti Sepolia dan mendukung deployment langsung ke jaringan Ethereum. Dengan kombinasi ini, proses pengembangan DApps menjadi lebih efisien, terstruktur, dan sesuai dengan praktik terbaik (best practices) dalam ekosistem Ethereum saat ini.<br>




<img width="1917" height="965" alt="image" src="https://github.com/user-attachments/assets/6b06a8dc-9625-44ce-86cd-36c0c8dc9ea5" />



