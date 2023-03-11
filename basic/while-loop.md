# While loop

`While loop` pada Dart adalah salah satu jenis perulangan yang digunakan untuk mengulangi satu atau lebih pernyataan selama kondisi tertentu terpenuhi. Perulangan `while` akan terus dilakukan selama kondisi yang diberikan dalam blok `while` tetap benar `true`. Ketika kondisi menjadi salah `false`, maka perulangan `while` akan berhenti.

</br>

Berikut adalah sintaksis dari `while loop` pada Dart:

```Dart
while (kondisi) {
  // Pernyataan yang akan diulang
}
```

</br>

Di dalam blok while, Anda dapat menuliskan satu atau lebih pernyataan yang ingin diulang. Kondisi adalah ekspresi Boolean yang diperiksa sebelum setiap iterasi perulangan dimulai.

```Dart
void main() {
  int i = 0;

  while (i < 5) {
    print("Angka ke-$i");
    i++;
  }
}
```

</br>

Pada contoh di atas, perulangan while akan berlangsung selama variabel `i` kurang dari `5`. Di dalam blok while, akan dieksekusi pernyataan `print("Angka ke-$i")` dan nilai `i` akan ditambahkan `1` setiap kali perulangan dilakukan. Output yang dihasilkan sebagai berikut:

```Dart
Angka ke-0
Angka ke-1
Angka ke-2
Angka ke-3
Angka ke-4
```

</br>

Dalam contoh di atas, perulangan while akan berhenti ketika variabel i sama dengan 5, karena pada saat itu kondisi dalam blok while menjadi salah (false).
