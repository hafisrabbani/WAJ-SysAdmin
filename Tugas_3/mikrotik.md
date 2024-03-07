<div align="center">
  <h1 style="text-align: center;font-weight: bold">Praktikum 3<br>Mikrotik</h1>
  <h4 style="text-align: center;">Dosen Pengampu : Dr. Ferry Astika Saputra, S.T., M.Sc.</h4>
</div>
<br />
<div align="center">
  <img src="https://upload.wikimedia.org/wikipedia/id/4/44/Logo_PENS.png" alt="Logo PENS">
  <h3 style="text-align: center;">Disusun Oleh : <br>Kelompok 3</h3>
  <p style="text-align: center;">
    <strong>Ade Hafis Rabbani (3122500001)</strong><br>
    <strong>Nadila Aulya Salsabila Mirdianti (3122500002)</strong><br>
    <strong>Gandi Rukmaning Ayu (3122500016)</strong>
  </p>
  
  <h3 style="text-align: center;line-height: 1.5">Politeknik Elektronika Negeri Surabaya<br>Departemen Teknik Informatika Dan Komputer<br>Program Studi Teknik Informatika<br>2023/2024</h3>
  <hr>
</div>

## Daftar Isi

- [Daftar Isi](#daftar-isi)
  - [1. Apa itu Mikrotik?](#1-apa-itu-mikrotik)
  - [2. Penjelasan](#2-penjelasan)


### 1. Apa itu Mikrotik?
**Pengertian Mikrotik**

![Gambar mikrotik](images/mikrotik.png)

Mikrotik merupakan sebuah sistem operasi berbasis perangkat lunak (software) yang digunakan untuk mengubah komputer menjadi sebuah router dalam suatu jaringan. Menggunakan sistem operasi yang berbasis Linux dan menjadi dasar bagi router jaringan. Sistem operasi ini sangat ideal untuk mengelola administrasi jaringan komputer dengan berbagai skala, mulai dari kecil hingga besar.

Namun, masih banyak orang yang memiliki kesalahpahaman mengenai konsep Mikrotik dan router. Jika Mikrotik adalah suatu sistem operasi yang termasuk dalam kategori open source, maka router adalah perangkat keras yang berfungsi sebagai penghubung antara dua jaringan atau lebih. Jadi, perbedaan mendasar antara keduanya adalah bahwa Mikrotik adalah perangkat lunak (software) sedangkan router berperan sebagai perangkat keras (hardware).


### 2. Penjelasan
1. Buka aplikasi **Mikrotik**.

2. Step 2

   ![](images/3.jpg)
   
   ![](images/1.jpg)


   Membuat IP Address untuk interface ether1 (192.168.88.3/24)
3. Step 3
   ![](images/4.jpg)
   ![](images/6.jpg)
   ![](images/7.jpg)
   ![](images/9.jpg)
   Membuat bridge untuk menghubungkan ether2-5 dengan ether1 untuk menjadikan sebagai switch
4. Step 4
   ![](images/5.jpg)
   lakukan pengujian apakah bisa terhubung dengan gateway

5. Step 5

   ![](images/8.jpg)

6.  Step 6

    ![](images/10.jpg)
    ![](images/11.jpg)

    Tambahkan IP address untuk ether 2
7.  Step 7

    ![](images/12.jpg)
    ![](images/14.jpg)
    agar bisa terhubung ke internet kita mengatur route agar semua interface nantinya akan di 

8.  Step 8
   
    ![](images/15.jpg)
    ![](images/16.jpg)
    ![](images/17.jpg)
    ![](images/18.jpg)
    ![](images/19.jpg)
    ![](images/20.jpg)
    ![](images/21.jpg)
    Membuat DHCP server untuk client yang akan terhubung pada interface bridge yang sudah dibuat tadi dengan range IP 200-254 dan menggunakan DNS dari PENS
    

9.  Step 9
    ![](images/22.jpg)
    ![](images/23.jpg)
    ![](images/24.jpg)
    Membuat NAT agar client bisa terhubung ke internet, dengan mengatur General, masukkan interface yang akan di NAT, dan masukkan IP address yang akan di NAT dan masukkan action masquerade

10. Step 10
    ![](images/25.jpg)
    Hubungkan kabel dari ether 2 ke laptop dan cek apakah sudah bisa terhubung ke internet
    jika sudah maka akan muncul lease yang diberikan oleh DHCP server