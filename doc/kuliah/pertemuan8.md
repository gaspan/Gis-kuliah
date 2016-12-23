#Verview
Data producer  -> data provider -> platform
Shp   setelah UTS -> setelah UTS -> sebelum UTS

Data provider
Pada saat ini kita akan menyajikan data shapefile untuk dikonsumsi secara public melalui platform

Provider: Mapserver adalah sebuah executable file yang bias mengubah atau mentrasformasikan file vector shp ke dalam format gambar. Agar bias dilihat / dikonsumsi oleh platform.
Cara instalasi mapserver
1.	Mengunduh (untuk windows) dari ms4w dari halaman download
2.	Diinstall aplikasinya
3.	Dilanjut install mapproxy

Install mapproxy
Untuk melakukan cache pada peta agar petanya lebih cepat diakses.
Langkah
1.	Install python , unduh dihalaman download
2.	Install virtual env melalui “pip install virtualenv”
3.	Install mapproxy melalui “pip install mapproxy”
     4  .Buat konfigurasi default
Mapproxy-utill Create –t base-Config anu
Dimana anu adalah folder yang baru. Masuk ke anu
4.	Edit folder mapproxy.yaml disesuaikan 

