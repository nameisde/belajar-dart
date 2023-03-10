## Null safety

Null safety digunakan untuk memastikan bahwa nilai `null` hanya diberikan ke variabel atau objek yang dinyatakan `nullable` secara eksplisit. Hal ini dapat mencegah bug runtime yang disebabkan oleh akses atau operasi pada variabel `null`.

Fitur null safety pada Dart memungkinkan untuk menandai variabel yang bernilai null atau tidak dapat bernilai null pada saat kompilasi. Ini dilakukan dengan menambahkan tanda tanya (`?`) setelah tipe data variabel. Tanda tanya menandakan bahwa variabel dapat bernilai null, sedangkan ketiadaan tanda tanya menandakan bahwa variabel tidak bernilai null.

</br>

Sebagai contoh, pada Dart sebelum fitur null safety, sebuah variabel dapat bernilai null atau tidak dapat bernilai null seperti berikut:

```Dart
int? nullableInt = null; // Variabel dapat bernilai null
int nonNullableInt = 42; // Variabel tidak dapat bernilai null
```

</br>

Pada Dart dengan fitur null safety, tipe data nullable ditandai dengan `?` di akhir tipe data, dan tipe data yang tidak nullable ditulis tanpa tanda tanya:

```Dart
int? nullableInt = null; // Variabel dapat bernilai null
int nonNullableInt = 42; // Variabel tidak dapat bernilai null

int? nullableInt2 = nonNullableInt; // Tidak error karena nullableInt2 dapat bernilai null
int nonNullableInt2 = nullableInt; // Error karena nullableInt dapat bernilai null
```

</br>

Dengan fitur null safety, Dart juga menambahkan operator null-aware, seperti operator `?`, `??`, dan `?.` untuk membantu mengakses atau memanipulasi nilai null dengan aman. Operator-operator ini memungkinkan untuk melakukan operasi hanya jika nilai variabel tidak null atau memberikan nilai default ketika variabel bernilai null.

Dengan null safety, Dart menjadi lebih aman dan dapat membantu programmer menghindari bug runtime yang disebabkan oleh nilai null yang tidak terduga.