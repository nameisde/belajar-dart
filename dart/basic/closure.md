# Closure

Closure adalah sebuah konsep yang mengacu pada kemampuan sebuah fungsi untuk mengakses variabel yang ada di luar lingkup fungsi tersebut, meskipun variabel tersebut sudah tidak berada dalam ruang lingkup yang sama. Di dalam bahasa Dart, setiap fungsi adalah objek dan dapat mengembalikan fungsi sebagai nilai balik atau argumen. Oleh karena itu, Dart mendukung penggunaan closure secara alami.

Dalam closure, sebuah fungsi dapat mengakses variabel-variabel yang didefinisikan di luar fungsi tersebut, bahkan jika variabel-variabel tersebut tidak lagi berada dalam ruang lingkup di mana fungsi tersebut didefinisikan. Ini memungkinkan kita untuk membuat fungsi yang memiliki akses ke lingkungan di mana fungsi tersebut didefinisikan.

</br>

Contoh penggunaan closure dalam Bahasa Dart adalah sebagai berikut:

```Dart
Function outerFunction(int x) {
  int innerValue = 2;

  return () => print(x + innerValue);
}

void main() {
  Function innerFunction = outerFunction(3);
  innerFunction(); // Output: 5
}
```

Di dalam contoh di atas, kita memiliki sebuah fungsi `outerFunction` yang mengembalikan sebuah fungsi baru yang tidak memiliki parameter dan mencetak hasil penjumlahan dari parameter `x` dengan variabel `innerValue` yang didefinisikan di dalam fungsi `outerFunction`. Variabel `innerValue` berada di luar ruang lingkup fungsi `innerFunction`, tetapi karena penggunaan closure, fungsi `innerFunction` masih memiliki akses ke variabel tersebut.

Kemudian, hal tersebut membuat variabel `innerFunction` yang menampung hasil pemanggilan fungsi `outerFunction` dengan parameter `3`. Setelah itu, kita memanggil `innerFunction` yang pada gilirannya memanggil fungsi yang dihasilkan oleh `outerFunction` dengan parameter `3`. Akibatnya, hasilnya adalah 5, yang merupakan hasil penjumlahan antara 3 dan 2 (nilai variabel `innerValue`).
