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

Dengan demikian, ketika mengakses localhost:8888 di host, maka akan diteruskan ke localhost:3000 di guest (VM).
