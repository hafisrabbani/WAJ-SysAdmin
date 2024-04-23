
## 1. Mengubah Interface
Ubah interface jaringan VM menjadi ```Bridge Adapter```

![thunderbird](./img/4.jpg)

## 2. Menambahkan DNS
Untuk pengaturan IPv4 method pilih Manual, kemudian pada bagian DNS ubah menjadi ```10.10.10.1```
![thunderbird](./img/5.jpg)

## 3. Forwarder dan Allow-query
Menambahkan forwarder dan merubah allow-query  dan allow-recursion menjadi ```any``` pada file named.conf.options
```sudo nano /etc/bind/named.conf.options```.
![thunderbird](./img/6.jpg)

## 4. Merubah DNS
Merubah DNS Servers di mikrotik menjadi ```10.10.10.1```

![thunderbird](./img/8.jpg)

## 5. Testing
- Pengujian Web Server melalui client.
  ![thunderbird](./img/10.jpg)

- Mencoba mengirim email ke alamat email lain.
  ![thunderbird](./img/7.jpg)

- Melakukan pengecekan apakah dapat menerima email dari alamat lain.
  ![thunderbird](./img/9.jpg)