# Inner function

Inner function atau fungsi dalam fungsi adalah sebuah fungsi yang didefinisikan di dalam fungsi lain. Dalam bahasa Dart, inner function dikenal sebagai `nested function` atau `nested method`.

</br>

```Dart
void outerFunction() {
  print('Ini adalah fungsi luar');

  void innerFunction() {
    print('Ini adalah fungsi dalam');
  }

  innerFunction();
}

void main() {
  outerFunction();
}
```

</br>

Pada contoh di atas, `innerFunction()` adalah fungsi dalam dari `outerFunction()`. Ketika `outerFunction()` dipanggil, ia juga memanggil `innerFunction()`.

Inner function juga dapat mengakses variabel dan parameter yang didefinisikan di dalam fungsi yang memuatnya (`outerFunction()`). Namun, variabel dan parameter di dalam `innerFunction()` tidak dapat diakses di luar fungsi tersebut.

</br>

```Dart
void outerFunction() {
  int x = 5;

  void innerFunction() {
    print(x);
  }

  innerFunction();
}

void main() {
  outerFunction();
}
```

</br>

Dalam contoh di atas, `innerFunction()` memiliki akses ke variabel `x` yang didefinisikan di dalam outerFunction(). Tetapi `x` tidak dapat diakses di luar `outerFunction()` atau `innerFunction()`.