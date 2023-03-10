# Logical

Operator logika atau *logical operators* digunakan untuk membandingkan dua nilai `boolean` (`true` atau `false`) dan menghasilkan nilai `boolean` baru sebagai hasil perbandingannya. Dalam Dart, operator logika terdiri dari operator `AND`, `OR`, dan `NOT`.

</br>

Berikut adalah daftar operator logika beserta contoh pengunaannya:

</br>

### 1\. Operator `AND` (`&&`)

Membandingkan dua nilai `boolean` dan menghasilkan nilai `boolean` `true` hanya jika kedua nilai tersebut bernilai `true`. Jika salah satu atau keduanya bernilai `false`, maka hasilnya akan bernilai `false`.

```Dart
bool a = true;
bool b = false;
bool c = true;
bool d = a && c;
bool e = b && c;
```
```sh
true
false
```

</br>

### 2\. Operator `OR` (`||`)

Membandingkan dua nilai `boolean` dan menghasilkan `boolean` `true` jika salah satu atau kedua nilai tersebut bernilai `true`. Jika kedua nilai tersebut `false`, maka hasilnya akan bernilai `false`

```Dart
bool a = true;
bool b = false;
bool c = true;
bool d = a || c;
bool e = b || c;
```
```sh
true
true
```

</br>

### 3\. Operator `NOT` (`!`)

Membalikkan nilai `boolean` menjadi nilai yang berlawanan. Jika nilai awalnya adalah `true`, maka hasilnya menjadi `false` dan sebaliknya.

```Dart
bool a = true;
bool c = !a;
bool c = !b;
```
```sh
false
true
```

</br>

Operator logika atau *logical operators* digunakan untuk menguji kondisi atau membuat keputusan berdasarkan hasil perbandingan dua nilai `boolean`. Contoh penggunaan operator logika dapat ditemukan pada struktur percabangan `if-else` dan `loop`.
