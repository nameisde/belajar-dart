# For in

`for in` pada Dart adalah salah satu cara untuk melakukan iterasi pada objek yang dapat diulang, seperti `List`, `Set`, `Map`, atau `String`. `for in` secara sederhana berarti "untuk setiap elemen di dalam objek ini".

</br>

Contoh penggunaan `for in` pada `List` adalah sebagai berikut:

```Dart
List<int> numbers = [1, 2, 3, 4, 5];

for (int number in numbers) {
  print(number);
}
```
```sh
1
2
3
4
5
```

</br>

Perbedaan utama antara menggunakan `for in` dengan tidak menggunakan `for in` adalah kita dapat menulis kode yang lebih sederhana dan lebih mudah dibaca untuk melakukan iterasi pada objek. Kita juga dapat memastikan bahwa setiap elemen dalam objek dapat diakses tepat satu kali, karena variabel iterasi akan menampung nilai dari setiap elemen secara berurutan.