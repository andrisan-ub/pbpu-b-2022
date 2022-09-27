# Pengembangan Beroritentasi Penggunaan Ulang

### Dosen Pengampu: Andri Santoso, S.kom., M.Sc.,

| Nama | NIM |
| --- | --- |
| Prasetya Naufal Rahmandita | 195150401111035 |
| Aditya Akhmad Jatnika | 195150401111025 |
| Mohammad Aditya Putra | 195150400111054 |
| Ronaldo Simatupang | 195150400111015 |
| Hendika Fashobiqul Galang F. | 195150400111024 |

### Kasus :
Buatlah sebuah UML Diagram mengenai alur kerja dari sistem antara e-commerce yang terintegrasi dengan ekspedisi dimana nantinya e-commerce dapat melihat tarif dan mengirim request untuk berbagai ekspedisi yang tersedia.

## Deklarasi Kelas

### eCommerece Class
Terdapat Beberapa atribut dari kelas ini yakni :

| Nama Field | Type | Visibility |
| --- | --- | -- |
| userName | String | private |
| address | String | private |
| packages | barang | private |

Terdapat juga method yang dipakai pada kelas ini, yakni :

| Nama Method | Parameter | Visibility |
| --- | --- | -- |
| delivery | barang : pemilihanKurir | public |

### JNE Class
Terdapat Beberapa atribut dari kelas ini yakni :

| Nama Field | Type | Visibility |
| --- | --- | -- |
| name | String | private |

Terdapat juga method yang dipakai pada kelas ini, yakni :

| Nama Method | Parameter | Visibility |
| --- | --- | -- |
| pengirimanYES | tarifPengiriman, requestPengiriman | public |
| pengirimanREG | tarifPengiriman, requestPengiriman | public |
| pengirimanOKE | tarifPengiriman, requestPengiriman | public |

### JNT Class
Terdapat Beberapa atribut dari kelas ini yakni :

| Nama Field | Type | Visibility |
| --- | --- | -- |
| name | String | private |

Terdapat juga method yang dipakai pada kelas ini, yakni :

| Nama Method | Parameter | Visibility |
| --- | --- | -- |
| pengirimanSuper | tarifPengiriman, requestPengiriman | public |
| pengirimanEZ | tarifPengiriman, requestPengiriman | public |
| pengirimanECO | tarifPengiriman, requestPengiriman | public |

### SiCepat Class
Terdapat Beberapa atribut dari kelas ini yakni :

| Nama Field | Type | Visibility |
| --- | --- | -- |
| name | String | private |

Terdapat juga method yang dipakai pada kelas ini, yakni :

| Nama Method | Parameter | Visibility |
| --- | --- | -- |
| pengirimanBEST | tarifPengiriman, requestPengiriman | public |
| pengirimanGOKIL | tarifPengiriman, requestPengiriman | public |
| pengirimanHALU | tarifPengiriman, requestPengiriman | public |

## Penjelasan 
Diagram UML yang telah dibuat mencerminkan alur kerja sistem E-Commerce yang terintegrasi dengan ekspedisi. Dalam kasus ini, Kelas E-Commerce memiliki ketergantungan terhadap interface pemilihanKurir. Hal ini terjadi karena Kelas E-Commerce dibatasi hanya akan berinteraksi dengan objek kurir yang mengimplementasikan interface pemilihanKurir. Artinya, setiap packages atau barang pada kelas E-Commerce harus bisa dikirimkan oleh objek Kurir dengan mengimplementasikan method tarifPengiriman() dan juga requestPengiriman().

## Sumber Pustaka
https://www.gleek.io/blog/class-diagram-arrows.html -> Relasi Kelas
http://www.cs.sjsu.edu/~pearce/modules/lectures/oop/basics/interfaces -> Inrterface Class

## Alur Relasi Kelas
Kelas eCommerece memlliki hubungan Directed association dengan Interface pemilihanKurir karena tanpa kelas eCommerece sangat bergantung pada Interface pemilihanKurir untuk melakukan transaksi. Interface pemilihanKurir memiliki 2 method (tarifPengiriman dan requestPengiriman) yang akan diimplementasikan oleh 3 kelas lainnya yang merupakan pilihan pada implementasi interface pemilihanKurir, yaitu jne, jnt, atau siCepat. Interface pemilihanKurir memiliki hubungan Realization/Implementation dengan ketiga kelas tersebut. Ketiga kelas tadi akan mengimplementasikan method dari pemilihanKurir dan akan digunakan kembali lebih lanjut dalam method mereka sendiri sebagai metode pengiriman yang diseiakan masing - masing pilihan kurir.

## Tanggal
13-09-2020

