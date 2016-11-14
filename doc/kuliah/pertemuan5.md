<h1 align="justify">MEMEBUAT DATA GEOSPASIAL</h1>
<img src="../../img/gambar.png">
<p align="justify"> kode yang digunakan untuk membuat data geospasial dengan bahasa python yaitu:</p> </br>
import shapefile </br>
a = shapefile.Writer() </br>
</br>
<p align="justify"> file untuk membuat data geospasial ada 2 yaitu: </p></br>
1. shp </br>
contohnya:</br>
a.point(x,y)</br>
a.poly([x,y],[v,w])</br>
2. dbf </br>
contohnya: </br>
a.field('namafield','C','40')</br>
a.record('Bdg)</br>
<p align="justify"> file itu disimpan dengan method:</p></br>
a.save('file.shp')</br>
</br>

<h2 align="justify"><strong>Penjelasan method-method pada Writer</strong></h2>
<h4 align="justify"><strong>Point(x,y)</strong></p>
<p align="justify">menginputkan data berbentuk point/titik ke dalam file shp dan harus sesuai dengan format yang ditentukan ESRI </p>
<h4 align="justify"><strong>Poly([a,b],[c,d])</strong></h4>
<p align="justify"> menginputkan data geospasial yang berupa polygon(kembali ke titik awal), dan polyline(tidak kembali ke titik awal)</p>
<h4 align="justify"><strong>field('kota','C','40')</strong></h4>
<p align="justify">membuat atribut tabel bernama 'kota' dengan tipe varchar, dengan panjang 40 karakter, jika ingin menmbahkan
 field maka panggil kembali method field contoh: field('Budaya','C','40')</p>
 <h4 align="justify"><strong>Record(''Bandung')</strong></h4>
 <p align="justify">mengisi tabel yang hanya terdapat 1 field dengan value = 'Bandung', jika ada 2 field maka record('Bandung','Kota')</p>
 <h4 align="justify"><strong>save('namafile')</strong></h4>
 <p align="justify">digunakan menyimpan file berbentuk shapefile dikomputer</p>
 <h4 align="justify"><strong>Param Writer</strong></h4>
 <p align="justify"> shapefile     POLYGON</p>
 <p align="justify"> shapefile     POINT</p>
 <p align="justify"> shapefile     POLYLINE</p>
 <p align="justify">contoh: </p>
 <p align="justify"><strong>POINT</strong></p>
 a.point(10,12) </br>
 <p align="justify"><strong>POLYLINE</strong></p>
 a.poly(parts=[[[1,5],[5,5],[3,3]]], <br>
 shapetype = shapefile.POLYLINE)</br>
 <p align="justify"><strong>POLYGON</strong></p>
 a.poly(parts=[[[1,5],[5,5],[5,1]]])
 
 
 

 
 
 



