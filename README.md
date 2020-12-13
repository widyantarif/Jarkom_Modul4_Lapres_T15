# Jarkom_Modul4_Lapres_T15

Nama Anggota: 
  - Widyantari Febiyanti 05311840000030
  - Nabella Desyawulansari 05311840000039

## Soal

1. Melakukan perhitungan subnetting VLSM dan CIDR.
2. Mengimplementasikannya ke Cisco Packet Tracer(CPT) dan UML.
3. Ilustrasinya adalah sebagai berikut ini:

![1](https://github.com/widyantarif/Jarkom_Modul4_Lapres_T15/blob/main/gambar%20modul%204/Soal%20Shift%20Modul%204.png)

## Jawaban

1. Buat topologi sama seperti soal di Cisco Packet Tracker

![2](https://github.com/widyantarif/Jarkom_Modul4_Lapres_T15/blob/main/gambar%20modul%204/topologi%20yak.png)

2. Selanjutnya tambahkan port NM-2FE2W pada semua router terlebih dahulu. khusus untuk router __SURABAYA__ tambahkan port NM-4E.
3. Sambungkan kabel antara sesama router atau dengan switch.
4. Lalu kelompokkan router dan switch yang ada seperti gambar dibawah: 

![3](https://github.com/widyantarif/Jarkom_Modul4_Lapres_T15/blob/main/gambar%20modul%204/topologi.jpg)

5. Setelah dikelompokkan, dapat dihitung subnetnya ada berapa dan menentukan penggunaan netmask sesuai dengan prefix setiap subnet. Perhitungan seperti dibawah: 

![4](https://github.com/widyantarif/Jarkom_Modul4_Lapres_T15/blob/main/gambar%20modul%204/perhitungan%20IP.jpg)

6. Atur IP untuk masing-masing interface yang ada di setiap device sesuai dengan pembagian subnet pada __VLSM__. Interface dapat diatur pada menu ```Config -> Interface > “nama interface” (contoh: FastEthernet0/0)```. Kemudian, isi alamat IP dan subnet mask dari subnet interface tersebut. Berikut contoh untuk mengatur IP pada subnet A1.
Atur IP pada interface __SURABAYA__ yang mengarah ke client __SAMPANG__ dengan 192.168.4.0.

![5](https://github.com/widyantarif/Jarkom_Modul4_Lapres_T15/blob/main/gambar%20modul%204/atur%20ip%20router.png)

7. Lalu atur IP di __SAMPANG__ yang mengarah ke __SURABAYA__. 

![6](https://github.com/widyantarif/Jarkom_Modul4_Lapres_T15/blob/main/gambar%20modul%204/atur%20ip%20client.png)

8. Ulangi langkah di atas untuk setiap router, dan juga client lain yang ada.
9. Melakukan routing di setiap router yang ada. Routing dapat dilakukan pada menu ```Config > Routing > Static``` pada device Router. Lalu, isilah static routes seperti gambar dibawah pada __SURABAYA__ dan tekan tombol 'Add':

![7](https://github.com/widyantarif/Jarkom_Modul4_Lapres_T15/blob/main/gambar%20modul%204/2020-12-13%20(2).png)

10. Semua routing untuk per router adalah: 

- __SURABAYA__

```
192.168.16.0/22 via 192.168.0.14
192.168.0.128/25 via 192.168.0.14
192.168.2.0/23 via 192.168.0.6
192.168.0.16/28 via 192.168.0.6
192.168.12.0/22 via 192.168.0.6
10.151.77.176/29 via 192.168.0.6
192.168.1.0/24 via 192.168.0.6
192.168.8.0/22 via 192.168.0.6
192.168.24.0/21 via 192.168.0.14
192.168.0.0/30 via 192.168.0.6
192.168.0.4/30 via 192.168.0.6
192.168.0.8/30 via 192.168.0.14
```

- __PASURUAN__

```
192.168.0.128/25 via 192.168.0.10
192.168.24.0/21 via 192.168.0.10
0.0.0.0/0 via 192.168.0.13
192.168.16.0/22 via 192.168.0.13
```

- __PROBOLINGGO__

```
0.0.0.0/0 via 192.168.0.5
0.0.0.0/0 via 192.168.0.9
```

- __BATU__

```
0.0.0.0/0 via 192.168.0.5
192.168.0.16/28 via 192.168.2.3
192.168.12.0/22 via 192.168.0.5
10.151.77.176/29 via 192.168.0.2
192.168.1.0/24 via 192.168.0.2
192.168.8.0/22 via 192.168.0.2
```

- __MADIUN__

```
0.0.0.0/0 via 192.168.2.1
```

- __KEDIRI__

```
0.0.0.0/0 via 192.168.0.1
192.168.8.0/22 via 192.168.1.3
```

- __BLITAR__

```
0.0.0.0/0 via 192.168.1.1
```




