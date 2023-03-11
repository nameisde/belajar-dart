# Anonymous function

Anonymous function dalam bahasa Dart adalah sebuah fungsi yang tidak memiliki nama. Sebuah anonymous function dapat didefinisikan dan langsung dipanggil tanpa harus memiliki nama terlebih dahulu.

Dalam Dart, anonymous function dapat didefinisikan menggunakan syntax `() {}` atau `() => expression`. Yang pertama digunakan untuk menuliskan blok kode dan yang kedua digunakan untuk menuliskan sebuah ekspresi.

</br>

Berikut adalah contoh penggunaan anonymous function di Dart:

```Dart
void main() {
  // Contoh anonymous function dengan blok kode
  var funcA = () {
    print('Hello from anonymous function!');
  };

  funcA(); // Panggil anonymous function

  // Contoh anonymous function dengan ekspresi
  var funcB = () => 'Hello from anonymous function!';

  print(funcB()); // Panggil anonymous function
}
```

Dalam contoh di atas, kita mendefinisikan dua anonymous function, `funcA` dan `funcB`. Kedua fungsi tersebut kemudian dipanggil menggunakan operator `()`.

</br>

Anonymous function sangat berguna dalam situasi di mana kita hanya membutuhkan sebuah fungsi sederhana yang hanya digunakan satu kali, sehingga tidak perlu menuliskan fungsi dengan nama terlebih dahulu. Contoh penggunaan anonymous function adalah ketika kita ingin melakukan operasi pada setiap elemen di dalam sebuah list, seperti berikut:

```Dart
void main() {
  var numbers = [1, 2, 3, 4, 5];

  // Anonymous function untuk menghitung jumlah dari setiap elemen di dalam list
  var sum = numbers.fold(0, (acc, val) => acc + val);

  print(sum);
}
```
```sh
15
```

Dalam contoh di atas, kita menggunakan anonymous function untuk menghitung jumlah dari setiap elemen di dalam list menggunakan metode `fold`.