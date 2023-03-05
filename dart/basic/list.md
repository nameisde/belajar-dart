## List

`List` pada bahasa pemrograman Dart merupakan struktur data yang digunakan untuk menyimpan kumpulan nilai yang sejenis. `List` dapat dianggap sebagai tipe data yang memungkinkan kita untuk menyimpan banyak nilai dalam satu variabel.

</br>

### Deklarasi List

Untuk membuat `List`, kita dapat mendeklarasikannya dengan menuliskan tipe data `List` diikuti dengan tanda kurung siku `[]` yang di dalamnya dapat diisi dengan nilai-nilai yang ingin disimpan.

```Dart
List<int> angka = [1, 2, 3];
```

</br>

### Akses elemen pada List

Untuk mengakses elemen pada `List`, kita dapat menggunakan `indeks` atau nomer urut elemen yang dimulai dari angka `0`.

```Dart
List<String> buah = ['apel', 'mangga', 'pisang'];
print(buah[0]);
```
```sh
apel
```

</br>

### Mengubah elemen pada List

Kita dapat mengubah nilai elemen pada `List` dengan cara mengakses elemen yang ingin diubah menggunakan `indeks` dan kemudian menetapkan nilai baru pada `indeks` tersebut.

```Dart
List<int> bilangan = [1, 2, 3, 4, 5];
bilangan[2] = 6;
print(bilangan);
```
```sh
[1, 2, 6, 4, 5];
```

</br>

### Menghapus elemen pada List

Kita dapat menghapus sebuah elemen pada `List` dengan cara menggunakan metode `removeAt()` yang menerima sebuah `indeks` sebagai `parameter`.

```Dart
List<String> buah ['apel', 'mangga', 'pisang'];
buah.removeAt(1);
print(buah);
```
```sh
['apel', 'pisang'];
```

</br>

### Menambahkan elemen pada List

Kita dapat menambahkan sebuah elemen baru pada `List` dengan cara menggunakan metode `add()` yang menerima sebuah nilai sebagai `parameter`.

```Dart
List<int> bilangan = [1, 2, 3, 4, 5];
bilangan.add(6);
print(bilangan);
```
```sh
[1, 2, 3, 4, 5, 6]
```