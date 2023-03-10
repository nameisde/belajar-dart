# For loop

For loop digunakan untuk melakukan perulangan pada suatu blok kode dengan jumlah perulangan yang telah ditentukan.

Memiliki sintaksis sebagai berikut:

```Dart
for (initialization; condition; increment/decrement) {
  // Blok kode yang akan diulang
}
```

- `initialization` nilai awal dari variabel loop, biasanya digunakan untuk inisialisasi variabel counter
- `condition` ekspresi boolean yang menentukan kapan loop akan berhenti
- `increment/decrement` perintah untuk menambah atau mengurangi nilai variabel counter pada setiap iterasi

</br>

Berikut adalah contoh penggunaan for loop pada Dart:

```Dart 
void main() {
  // for loop dengan counter
  for (int i = 0; i < 5; i++) {
    print('Iterasi ke-$i');
  }

  // for loop dengan iterable
  List<int> listAngka = [1, 2, 3, 4, 5];
  for (int angka in listAngka) {
    print(angka);
  }
}
```

Pada contoh di atas, for loop pertama menggunakan variabel counter `i` untuk melakukan perulangan sebanyak 5 kali, dengan menggunakan initial value `0`, condition `i < 5` dan increment `i++`.

Sedangkan pada for loop kedua, digunakan iterable `listAngka` yang berisi angka dari 1 sampai 5, dan loop akan berhenti setelah iterasi terakhir pada iterable.

For loop pada Dart juga dapat ditulis dalam bentuk singkatan yaitu `for-in loop`, seperti contoh kedua di atas. Dalam bentuk ini, kita tidak memerlukan variabel counter atau inisialiasi nilai awal, dan kita hanya perlu menentukan iterable yang akan diulang dan variabel untuk menyimpan nilai iterasi saat ini.

```Dart
void main() {
  List<int> listAngka = [1, 2, 3, 4, 5];

  // for-in loop
  for (int angka in listAngka) {
    print(angka);
  }
}
```

Dalam `for-in loop`, setiap nilai dari iterable akan disimpan dalam variabel `angka` pada setiap iterasi.