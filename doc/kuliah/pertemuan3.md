<h1 align ="justify">RETRIEVE PADA DATA GEOSPASIAL DAN MEMBUAT CLASS PADA PADA PYTHON</h1>

<p align="justify">Data Geospasial merupakan pengetahuan yang mepelajari tentang titik koordinat dari suatu peta atau juga dapat disebut dengan mempelajari tentang geografis yang ada bumi. Didalam geospasial itu sendiri ada untuk manipulasi data dan menghitung record pada file .shp, dan shp itu terdapat dalam shapefile dan didalam shapefile itu tidak hanya terdapat file shp namun ada juga file dbf. Untuk membaca shapefile kita dapat menggunakan python kita dapat memanggil langsung file shp nya atau juga bisa membuat class terlebih dahulu.</p>

<p align="justify">Retrieve data geospasial adalah merupakan suatu cara untuk melakukan select/view, data record dari file dbf dan geometri dari file shp.</p>

<p align="justify">SHP adalah salah satu file yang berada didalam shapefile yang menyimpan data geometri.
Didalam file shp terdapat beberapa data seperti:</p>

1.       Bbox adalah sebuah boundary box (koordinat 4 titik) atau koordinat batas view yang ada pada peta.</br>
2.       Point adalah titik suatu koordinat</br>
3.       Shapetype adalah jenis data geometri yang mempunyai standar nomor yang ditetapkan oleh ESRI seperti nomor 1 untuk poin, 2 untuk polygon, 3 untuk polyline, dll. 
Contoh ada pada link: shapefile.esri</br>

<p align="justify">DBF adalah sebuah file yang menyimpan file tabular yang menyimpan data attribut.

Membaca Jumlah data geometri dengan python:</p>
-          Membaca data shp 
>> import shapefile </br>
>> sf = shapefile.Reader(“namafile.shp”) </br>
>> sf.shapes() </br>
>> a = sf.shapes() </br>
>> len(a) </br>

-          Membaca data DBF </br>
>> import shapefile </br>
>> sf.records() </br>
>> sf.records(n) </br>
