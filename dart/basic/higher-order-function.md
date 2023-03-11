# Higher order function

Higher order function adalah fungsi yang dapat menerima satu atau lebih fungsi seabgai parameter atau mengembalikan sebuah fungsi. Dalam bahasa Dart, fungsi adalah first class object yang dapat diperlakukan seperti tipe data lainnya, sehingga memungkinkan kita untuk mengeksekusi dan memanipulasi fungsi dalam program

</br>

Contoh sederhana dari higher order function yang menerima sebuah fungsi sebagai parameter:

```Dart
void repeat(int times, Function action) {
  for (int i = 0; i < times; i++) {
    action();
  }
}

void main() {
  repeat(3, () => print('Hello, World!'));
}
```

Dalam contoh di atas, `repeat()` adalah higher order function yang menerima dua parameter: `times`, sebuah integer yang menentukan berapa kali fungsi `action` akan dijalankan, dan `action` sebuah fungsi tanpa parameter. Fungsi `repeat()` akan memanggil fungsi `action` sebanyak `times` kali.

Pada contoh di atas, kita memanggil higher order function `repeat()` dengan memberikan lambda expression sebagai argumen ke -2, yaitu `() => print('Hello, World!')`. Lamba expression ini adalah contoh dari fungsi tanpa nama yang diteruskan sebagai parameter ke higher order function.

</br>

Higher order function juga dapat mengembalikan sebuah fungsi. Contoh sederhana dari higher order function yang mengembalikan sebuah fungsi:

```Dart
Function multiplyBy(int factor) {
  return (int number) => number * factor;
}

void main() {
  final triple = multiplyBy(3);
  print(triple(2));
}
```
```sh
6
```

Dalam contoh di atas, `multiplyBy()` adalah higher order function yang menerima sebuah integer `factor` dan mengembalikan sebuah fungsi yang mengalikan bilangan integer dengan `factor`. Saat `multiplyBy()` dipanggil dengan argumen `3`, ia mengembalikan sebuah fungsi yang akan mengalikan sebuah bilangan dengan 3. Kita menyimpan hasil dari pamanggilan fungsi `multiplyBy(3)` ke dalam variabel `triple`. Selanjutnya kita memanggil `triple(2)`, yang akan mengembalikan hasil dari `2x3`, yaitu `6`.