# Function parameter

Function parameter digunakan untuk memberikan input ke dalam function. Parameter dapat berupa tipe data apapun, seperti `String`, `int`, `double`, `bool`, atau bahkan objek kelas yang telah dibuat. Function juga dapat memiliki parameter opsional yang dapat diberikan nilai default jika tidak diberikan nilai pada saat pemanggilan.

</br>

Contoh penggunaan parameter pada function:

```Dart
int sum(int a, int b) {
  return a + b;
}

void main() {
  int result = sum(5, 10);
  print(result);
}
```

</br>

Pada contoh di atas, function `sum` memiliki dua parameter bertipe `int` yaitu `a` dan `b`. Saat function dipanggil dengan argumen `5` dan `10`, maka nilai dari `a` adalah `5` dan nilai dari `b` adalah `10`. Function kemudian mengembalikan hasil penjumlahan dari kedua parameter tersebut dan disimpan dalam variabel `result`. Variabel `result` kemudian dicetak menggunakan function `print`.