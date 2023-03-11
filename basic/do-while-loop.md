# Do while loop

`Do while loop` pada Dart adalah jenis perulangan yang hampir sama dengan `while loop`. Namun, perbedaan terletak pada urutan eksekusi kondisi dan pernyataan dalam blok perulangan. Dalam `do while loop`, pernyataan dalam blok perulangan akan dieksekusi setidaknya satu kali sebelum kondisi dievaluasi. Setelah itu, blok perulangan akan diulang selama kondisi masih terpenuhi `true`.


</br>

Berikut adalah sintaksis dari `do while loop` pada Dart:

```Dart
do {

} while (kondisi);
```

</br>

Sama seperti `while loop`, di dalam blok `do while`, Anda dapat menuliskan satu atau lebih pernyataan yang ingin diulang. Kondisi adalah ekspresi `boolean` yang dievaluasi setelah setiap iterasi perulangan selesai.

Berikut adalah contoh penggunaan `do while loop` pada Dart:

```Dart
void main() {
  int i = 0;

  do {
    print("Angka ke-$i");
    i++;
  } while (i < 5);
}
```

</br>

Pada contoh di atas, blok perulangan do-while akan dijalankan setidaknya satu kali, karena kondisi belum dievaluasi ketika blok perulangan pertama kali dijalankan. Kemudian, setelah blok perulangan dieksekusi, kondisi akan dievaluasi. Jika kondisi masih benar (true), maka blok perulangan akan diulang. Jika kondisi salah (false), maka blok perulangan akan berhenti.

Output yang dihasilkan:

```Dart
Angka ke-0
Angka ke-1
Angka ke-2
Angka ke-3
Angka ke-4
```

</br>

Dalam contoh di atas, perulangan do-while akan berhenti ketika variabel i sama dengan 5, karena pada saat itu kondisi dalam blok do-while menjadi salah (false).