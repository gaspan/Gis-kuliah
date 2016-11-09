
<img width="450cm" height="450cm" src="../../img/images.jpg">

<strong>LATAR BELAKANG MASALAH</strong></br>
     <p align="justify"> banyak aplikasi yang membutuhkan data-data geospasial, contohnya seperti google earth, maka dibuatlah blog ini untuk meretrive data geospasial yang berupa data vektor.</p>

Geometri suatu data pada titik koordinat yang bisa berwujud bangun 2 dimensi / 3 dimensi diantaranya:</br>
a. Polygon</br>
b. Garis Shape, type / Line (bukan sosmed ya :v)</br>
c. titik/ Point (tanpa Blank)</br>

Geometri menurut standar ESRI dibagi menjadi 3 bagian:</br>
1. point </br>
2. polyline </br>
3. Poligon</br>

operasi pada pemogramman Python </br>
Library pyshp adalah import shapefile penjelasan instansi (OOP maksudnya) kelas  shapefile pada suatu variabel</br> 

Sf = shapefile.Reader(‘Bts.shp’) </br>
Penjelasan :</br>
SF = Variable</br>
Shapfile = Sebuah class</br>
Reader = Method</br>
Bts,shp = Parameter file</br>
Method method pada data DBF dan SHP</br>
Method pada data DBF</br>
sf.fileds() adalah untuk melihat attribute table</br>
sf.records() adalah untuk mengambil semua record</br>
sf.record(n) adalah untuk isi record</br>
Method pada data SHP</br>
Sf.shapes() adalah untuk mengambil semua record geometri</br>
Sf.shape(n) adalah untuk mengambil 1 record pada baris n Cara untuk mengambil 1 record dengan parameter nilai atau Array</br>
sf.records(0) [8]</br>
sf.field(0) [8]</br>
Titik koordinat terdapat 4 titik</br>
BBOX</br>
POINT</br>
SHAPETYPE</br>
Contoh Code untuk menampilkan nama Negara memakai contruk .</br>
For a in sf.records():</br>
If a[8] = “Indonesia”</br>
Print a</br>
Atau bisa juga</br>
I = 0</br>
For a in sf.records():</br>
If a[8] ==”Zimbabwe”:</br>
Print a :</br>
I = i+1</br>
menampilkan jumlah record melalui terminal cmd</br>

<img width="450cm" height="450cm" src="../../img/1.png" ></br></br>
masukan koding Indicator.py </br></br>
<img width="450cm" height="450cm" src="../../img/2.png"></br></br>
membuat method select,  Where Negara Indonesia Output Data Record Negara Indonesia</br></br>
<img width="450cm" height="250cm" src="../../img/3.png"> </br></br>

<strong>kesimpulan</strong></br>
<p align="justify">Dengan membuat class di python yang sesuai dengan file.py akan membuat kita bisa melihat record data. Dengan perintah perintah yang sudah dipraktekan kita menjadi lebih tahu hal hal yang baru di Python.</br>
</br>
<strong>saran<strong></br> 

Pengembangan GIS untuk User dan bagaimana penerapannya dgn bahasa python harus dipraktekan.</br>
</br>
nama : gentur ariyadi siddiq permana yakti</br> 
npm : 1144025</br>
kelas : 3b</br>
prodi : D4 teknik informatika</br>
matakuliah: sistem informasi geografis</br>
