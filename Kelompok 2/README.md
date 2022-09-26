# Pengembangan Beroritentasi Penggunaan Ulang

Penjelasan UML

Pada UML Diagram diatas, kami mendefinisikan 4 Class dan 1 Interface Class. Pada Class yang pertama yaitu ECommerce, memiliki beberapa atribut bersifat publik yang diantaranya adalah beratProduk, kecamatanAsal, kecamatanTujuan dan method bersifat publik yang berupa proses. Class selanjutnya berupa Interface dengan nama EkspedisiAPI yang berisi atribut tarif dengan parameter jarak, dan beratProduk dengan atribut selanjutnya berupa reqPengiriman yang memiliki parameter kecamatanAsal dan kecamatanTujuan. Selanjutnya terdapat Class SiCepat, JNE, dan JNT yang mengimplementasikan dari Class Interface EkspedisiAPI, sehingga pada masing-masing Class memiliki atribut tarifPengiriman dengan parameter jarak dan beratProduk serta reqPengiriman dengan parameter kecamatanAsal dan kecamatanTujuan.
