# Break dan continue

Break dan continue adalah dua statement yang digunakan dalam pengendalian alur program pada Dart.

</br>

## Break 

Perintah yang digunakan untuk menghentikan perulangan (loop) atau `switch statement` yang sedang berjalan. Ketika `break` dieksekusi, maka program akan keluar dari blok perulangan atau `switch statement` dan melanjutkan eksekusi perintah selanjutnya di luar blok tersebut.

Break biasanya digunakan ketika kita ingin menghentikan sebuah perulangan berdasarkan kondisi tertentu. Contohnya, ketika kita menghentikan perulangan saat sudah mencapai nilai tertentu.

Berikut adalah contoh `break` pada Dart:

```Dart
void main() {
  for (int i = 0; i < 10; i++) {
    if (i == 5) {
      break;
    }
    print("Angka ke-$i");
  }
}
```

</br>

Pada contoh di atas, perulangan `for` akan berhenti ketika variabel `i` sama dengan `5`, karena pada saat itu `break` dieksekusi.

Output yang dihasilkan, sebagai berikut:

```sh
Angka ke-0
Angka ke-1
Angka ke-2
Angka ke-3
Angka ke-4
```

</br>

## Continue

Perintah yang digunakan untuk melompati satu iterasi perulangan (loop) yang sedang berjalan. Ketika `continue` dieksekusi, maka program akan melompati satu iterasi perulangan dan langsung melanjutkan ke iterasi berikutnya. `Continue` biasanya digunakan ketika ingin melompati iterasi tertentu dan melanjutkan perulangan dengan iterasi berikutnya.

Berikut adalah contoh penggunaan `continue` pada Dart:

```Dart
void main() {
  for (int i = 0; i < 10; i++) {
    if (i % 2 == 0) {
      continue;
    }
    print("Angka ke-$i");
  }
}
```

</br>

Pada contoh di atas, perulangan `for` akan melompati setiap iterasi dengan nilai genap, karena pada saat itu `continue` dieksekusi. 

Output dari program ini adalah sebagai berikut:

```Dart
Angka ke-1
Angka ke-3
Angka ke-5
Angka ke-7
Angka ke-9
```

</br>

Dalam contoh di atas, perulangan akan menampilkan nilai dari variabel `i` hanya jika nilai tersebut adalah bilangan ganjil. Iterasi dengan nilai genap akan dilewati.
