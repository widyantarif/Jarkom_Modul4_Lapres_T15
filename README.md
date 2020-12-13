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

