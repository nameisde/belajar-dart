# Set

Set adalah struktur data yang memungkinkan untuk menyimpan sekumpulan nilai yang unik dan tidak terurut. Artinya, `set` tidak mengizinkan duplikat nilai yang sama di dalamnya dan elemen-elemennya tidak memiliki urutan tertentu.

</br>

Untuk mendeklarasikan `set`, kita dapat menggunakan kurung kurawal `{}` dan menyebutkan setiap elemen yang ingin kita masukkan ke dalamnya.

```Dart
Set<int> setAngka = {1, 2, 3, 4, 5};
```

Dalam contoh di atas, kita membuat `set` bernama `setAngka` yang berisi 5 nilai `integer`. Karena `set` hanya menyimpan nilai yang unik, maka jika kita mencoba menambahkan nilai yang sudah ada di dalam `set`, nilai tersebut tidak akan ditambahkan ke dalam `set`.

</br>

```Dart
Set<int> setAngka = {1, 2, 3, 4, 5, 5};
print(setAngka);
```
```sh
{1, 2, 3, 4, 5}
```

</br>

Dalam contoh di atas, meskipun kita mencoba untuk menambahkan nilai `5` ke dalam `set` `setAngka` dua kali, namun nilai tersebut hanya muncul satu kali saja di dalam `set`.

</br>

`Set` juga memiliki beberapa metode yang berguna untuk memanipulasi `set`, seperti:

</br>

- `.add()` untuk menambahkan sebuah elemen ke dalam set
- `.addAll()` untuk menambahkan beberapa elemen ke dalam set sekaligus
- `.remove()` untuk menghapuse sebuah elemen dari set
- `.clear()` untuk menghapus semua elemen dari set

</br>

```Dart
Set<String> setHewan = {'kucing', 'anjing', 'burung'};
setHewan.add('ikan');
print(setHewan);

setHewan.addAll({'gajah', 'kuda'});
print(setHewan);

setHewan.remove('burung');
print(setHewan);

setHewan.clear();
print(setHewan);
```
```sh
{'kucing', 'anjing', 'burung', 'ikan'}
{'kucing', 'anjing', 'burung', 'ikan', 'gajah', 'kuda'}
{'kucing', 'anjing', 'ikan', 'gajah', 'kuda'}
{}
```