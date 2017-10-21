# Tipe Data Pada PHP
**1. Integer**

Tipe data integer digunakan untuk menyimpan bilangan bulat yang berisikan bilangan bulat negatif dan positif atau tanpa ada nilai pecahan. Atruran untuk tipe data integer :
1. Harus minimal 1 digit (0-9).
2. Harus mengandung koma atau tanda kurung.
3. Tidak menganadung titik desimal.
4. Bisa bilangan positif
5. Dispesifikasikan mennjadi 3 format : desimal (10-based), hexadecimal (16-based diawali dengan ()x) atau octal (8-based diawali dengan 0).

* Contoh penulisan tipe data integer :
```php
$x = 12;
var_dump($x);
echo "<br>";
// bilangan negatif
$x = -12; 
var_dump($x);
echo "<br>";
// bilangan hexadecimal
$x = 0x8c;
var_dump($x);
echo "<br>";
```
**2. Double Floating**

Tipe Double Floating biasa juga disebut dengan double, float atau real merupakan tipe data yang digunakan untuk menyimpan bilangan desimal.

* Contoh Penulisan tipe data Double Floating
```php
$x = 3.5;
```
**3. Boolean**

Tipe Data Bolean pada PHP merupakan tipe data yang paling sederhana yakni hanya berupa dua kondisi yaitu True atau False.   Cara menuliskannya pada variabel hanya dengan memberikan nilai true atau false pada variabel tersebut.
* contoh penulisan tipe data bolean pada PHP.

```php
$x = true;
$y = false;
```
Tipe Data tersebut memberikan nilai true atau false pada kondisi tertentu diantaranya Pada :

1. Variabel yang bertipe data integer = 0 (nol) mempunyai boolean false, selain itu true.
2. Variabel yang bertipe data float = 0.0 (nol) mempunyai boolean false, selain itu true.
3. Variabel yang bertipe data string yang kosong, dan string = “0” mempunyai boolean false, selain itu true.
4. Array yang tidak mempunyai element mempunyai boolean false, selain itu true.
5. Objek yang tidak mempunyai member mempunyai boolean false, selain itu true.
6. Tipe NULL dan Variabel yang belum terisi mempunyai boolean false.

**4. String**

Tipe data string merupakan sebuah tipe data yang terdiri dari kata, baik kata tunggal maupun kalimat. Penulisan string pada PHP harus diapit oleh tanda petik tunggal (‘ ‘) atau tanda petik ganda (” “).
* Contoh penulisan tipe data String pada PHP 
```php
$x = "Hello World";
echo 'tulisan dalam petik tunggal $x';
echo "tulisan dalam petik ganda $x";
```


**5. Tipe Data Null**
* Contoh Penulisan tipe data Null
```php

$x = "Hello World!";
$x = null;
var_dump($x);
```

**6. Array**
Array digunakan untuk menyimpan sekumpulan nilai yang bertipe data sama.
## Pada PHP ada 3 (tiga) jenis array, yaitu : 
1. Numeric Array

Contoh Numeric Array :
```php
$x[0] = "Hello";
$x[1] = "Tuliskode";
echo $x[0]." ".$x[1];
```
Ket : Pemanggilan data pada jenis numeric array menggunakan angka, angka merupakan nomor index dari data array yang dimulai dari 0 sampai jumlah data yang dimasukkan. 

2. Associative Array

Contoh Associative Array :
```php
$x= array("web=>tuliskode.com","email=>infotulisankode.com");
echo "kunjungi TulisKode, Website : $x[web], email = $x[email]";
```
Ket :  Pada associative array pemanggilan nilai array menggunakan string yang telah kita ditentukan saat mendeklarasi array.

3. Multidimensional Array.

Contoh Multidimensional Array :
```php
$x= array(
array("web=>tuliskode.com","email=>info@tuliskode.com"),
array("motto=>ikatlah ilmu dengan berbagi","alamat=>Banda Aceh"));
echo "kunjungi TulisKode, Website : $x[0][web], alamat = $x[1][alamat];
```

**7. Object**

* Inisialisasi Object
Untuk membuat objek baru, gunakan pernyataan baru untuk memberi contoh pada kelas:
```php
class foo
{
    function do_foo()
    {
        echo "Doing foo."; 
    }
}

$bar = new foo;
$bar->do_foo();
```
* Mengubah ke objek 

Jika sebuah objek dikonversi ke suatu objek, maka objek tersebut tidak dimodifikasi. Jika nilai dari tipe lain dikonversi ke sebuah objek, sebuah instance baru dari stdClass built-in class dibuat. Jika nilainya NULL, instance baru akan kosong. Sebuah array mengkonversi ke objek dengan properti yang diberi nama oleh kunci dan nilai yang sesuai, kecuali kunci numerik yang tidak dapat diakses kecuali diulang.
```php
$obj = (object) array('1' => 'foo');
var_dump(isset($obj->{'1'})); // outputs 'bool(false)'
var_dump(key($obj)); // outputs 'int(1)'
```
Untuk nilai lainnya, variabel anggota bernama skalar akan berisi nilainya.
```php
$obj = (object) 'ciao';
echo $obj->scalar;  // outputs 'ciao'
```



# Referensi
* [Modul PWD]
