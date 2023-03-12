# Method expression body

Method expression body adalah cara singkat untuk mendefinisikan sebuah method pada Dart. Dalam method expression body, kita dapat langsung menuliskan implementasi dari method tersebut tanpa harus menggunakan blok kode.

</br>

Contoh definisi dari method expression body:

```Dart
class MyClass{
  int addNumbers(int x, int y) => x + y;
}
```

</br>

Pada contoh di atas, `addNumbers` adalah sebuah method yang menerima dua parameter bertipe integer `x` dan `y` dan mengembalikan hasil penjumlahan dari kedua parameter tersebut. Kita menggunakan tanda `=>` untuk menuliskan implementasi dari method tersebut.

</br>

Dengan menggunakan method expression body, kita dapat menghindari penulisan kode yang berlebihan dan membuat kode lbih mudah dibaca. Namun, perlu diingat bahwa method expression body hanya dapat digunakan pada method yang memiliki satu pernyataan saja. Jika method memiliki beberapa pernyataan atau kode yang kompleks, maka sebaiknya menggunakan blok kode yang biasa.