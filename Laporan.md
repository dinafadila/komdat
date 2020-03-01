<p align="center">
  <a href="">
    <img src="https://github.com/dinafadila/komdat/blob/master/agar.io.png" alt="Agar.io" width=72 height=72>
  </a>

  <h3 align="center">Agar.io</h3>

  <p align="center">
    adalah permainan multiplayer yang bertujuan untuk mendapatkan </br>
    lebih banyak massa sebanyak mungkin dengan menelan sel yang lebih kecil.
    <br>
  </p>
</p>

## Anggota Kelompok

1. Fathiya (G64170010)
2. Dina Fadila (G64170021)
3. Annisa Widia Astuti (G64170051)
4. Bella Anggita Safitri (G64170059)

## Yang dibutuhkan dalam instalasi

```text
1. Windows
2. Ubuntu server
3. Node.js
4. NPM
5. Socket.io
6. Express.io
```

## Langkah instalasi

### 1. Membuat VM Ubuntu Server
Dalam instalasi, digunakan Ubuntu Server 18.04. Kemudian, buat Virtual Machine baru pada VirtualBox dengan tipe "Ubuntu 64-bit".
- Jalankan VirtualBox lalu klik New. Berikan nama bebas, tapi pastikan version: Ubuntu (64-bit).
![Gambar Memotret](https://github.com/dinafadila/komdat/blob/master/1.png)
- Pilih Create a virtual hard disk now, lalu klik Create.
![Gambar Memotret](https://github.com/dinafadila/komdat/blob/master/2%20(2).png)

### 2. Setting Port-Forwarding
Port-forwarding berfungsi agar server dapat diakses dari luar melalui alamat host (IP host).
- Klik setting pada ubuntu server, klik Network, pilih Advance, lalu klik Port Forwarding.
![Gambar Memotret](https://github.com/dinafadila/komdat/blob/master/3.png)
- Tambah port dan atur seperti tabel dibawah ini:
![Gambar Memotret](https://github.com/dinafadila/komdat/blob/master/4.png)

Dengan demikian, ketika mengakses localhost:8888 di host, maka akan diteruskan ke localhost:3000 di guest (VM). Begitu juga dengan SSH, jika kita mengakses port 2200 di host, maka akan diteruskan ke port 22 di guest.

### 3. Update Paket Sistem dan Install ss
Update seluruh paket dalam sistem agar up-to-date. Serta, install ssh agar dapat diakses melalui terminal ubuntu.
```text
$ sudo apt update
$ sudo apt install ssh
```

### 4. Install Node.js dan NPM
```text
$ sudo apt-get install nodejs
$ sudo apt-get install npm
```

### 5. Install Socket.io dan Express.io
Pada command line instalasi socket.io dan express.io ditambahkan --save. Hal ini berfungsi untuk menyimpan hasil instalasi sehingga selanjutnya jika ingin menjalankan agar.io tidak perlu melakukan instalasi socket.io dan express.io lagi.
```text
npm install socket.io --save
npm install express.io --save
```

### 6. Download Agar.io
Setelah di download, kita masuk kedalam direktori agar.io-clone.
```text
$ git clone https://github.com/huytd/agar.io-clone.git
$ cd agar.io-clone
```

### 7. Install Agar.io
Saat melakukan instalasi agar.io, pastikan anda masih berada pada direktori 
```text
agar.io-clone
npm install
```

### 8. Menjalankan Agar.io
Saat menjalankan agar.io, pastikan anda masih berada pada direktori 
```text
agar.io-clone
npm start
```
![Gambar Memotret](https://github.com/dinafadila/komdat/blob/master/5.png)

Buka port localhost:8888, maka akan muncul tampilan sebagai berikut
![Gambar Memotret](https://github.com/dinafadila/komdat/blob/master/6.png)

## Cara Pemakaian
### a. Langkah pemakaian
1. Masukkan nama pengguna pada kolom Nick sebagai identitas bakteri pengguna.
2. Pengguna menekan tombol Play dan memulai permainan.
3. Gerakkan mouse ke segala arah pada layar untuk menggerakan karakternya. Pengguna cukup memakan sel-sel bakteri berukuran kecil yang ada disekitarnya dan menghindari sel bakteri berukuran besar agar tidak dimakan oleh sel bakteri besar tersebut sehingga pengguna dapat bertahan hidup.
4. Tekan tombol space untuk membelah diri.
5. Permainan berakhir saat karakter dimakan oleh lawan yang berukuran lebih besar.
6. Objective: Cobalah untuk menjadi sebesar mungkin dengan memakan pemain yang lain.

### b. Rules 



## Pembahasan
### Kelebihan
```text
1. Tidak terpengaruh jaringan internet.
2. Sederhana ketika memulai permainan. Pengguna cukup mengisi nama pengguna pada kolom Nick dan menekan tombol Play.
3. Mudah dimengerti dan dimainkan oleh pengguna awam.
4. Setting yang mudah dimengerti.
```

### Kelemahan
```text
1. User Interface game terlalu simple.
2. Permainan hanya bisa dimainkan secara local.
3. Tidak ada tantangan pada game, karena tidak ada lawan dan tidak bisa mati.
```

## Referensi
- github.com/auriza
- https://github.com/huytd/agar.io-clone
