## Comparison

Operasi perbandingan pada bahasa Dart adalah operasi yang digunakan untuk membandingkan dua nilai atau variabel. Operasi ini mengembalikan nilai `boolean` (`true` atau `false`) yang menunjukkan hasil perbandingan.

Berikut adalah daftar operator perbandingan yang tersedia pada bahasa Dart:

</br>

### 1\. Sama dengan `==`

Operator ini digunakan untuk memeriksa apakah dua nilai atau variabel memiliki nilai yang sama

```Dart
int a = 5;
int b = 5;
bool result = (a == b);
```
```sh
true
```

</br>

### 2\. Tidak sama dengan `!=`

Operator ini digunakan untuk memeriksa apakah dua nilai atau variabel tidak memiliki nilai yang sama

```Dart
int a = 5;
int b = 10;
bool result = (a != b);
```
```sh
true
```

</br>

### 3\. Lebih besar dari `>`

Operator ini digunakan untuk memeriksa apakah nilai pertama lebih besar dari nilai kedua

```Dart
int a = 5;
int b = 2;
bool result = (a > b);
```
```sh
true
```

</br>

### 4\. Lebih kecil dari `<`

Operator ini digunakan untuk memeriksa apakah nilai pertama lebih kecil dari nilai kedua

```Dart
int a = 5;
int b = 2;
bool result = (a < b);
```
```sh
false
```


</br>

### 5\. Lebih besar atau sama dengan `>=`

Operator ini digunakan untuk memeriksa apakah nilai pertama lebih besar atau sama dengan nilai kedua

```Dart
int a = 5;
int b = 2;
bool resultA = (a >= b);
bool resultB = (a >= 5);
```
```sh
true
true
```

</br>

### 6\. Lebih kecil atau sama dengan `<=`

Operator ini digunakan untuk memeriksa apakah nilai pertama lebih kecil atau sama dengan nilai kedua

```Dart
int a = 5;
int b = 2;
bool resultA = (a <= b);
bool resultB = (a <=> 5);
```
```sh
false
true
```

</br>

Operator perbandingan digunakan untuk mengontrol alur program. Misalnya, operator perbandingan digunakan untuk membandingkan nilai-nilai dalam kondisi `if-else`, `loop`, dan `switch-case` untuk menentukan apakah program harus melakukan tindakan tertentu atau tidak.