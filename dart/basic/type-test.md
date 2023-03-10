# Type Test

Operator type test digunakan untuk melakukan pengecekan tipe data dan konversi tipe data pada variabel atau objek.

</br>

## 1\. Operator `as`

Mengkonversi suatu objek menjadi tipe data yang diinginkan atau subtype dari tipe tersebut. Jika konversi tidak berhasil, maka akan terjadi `runtime error``.

```Dart
var x = 'hello';
String y = x as String;
print(y);
```
```sh
hello
```

</br>

## 2\. Operator `is`

Memeriksa apakah sebuah nilai atau *instance* dari suatu tipe tertentu atau *subtype* dari tipe tersebut. Jika ya, maka hasilnya adalah nilai `boolean` `true`, dan `false` jika tidak.

```Dart
var x = 'hello';
if (x is String) {
  print('x adalah string');
} else {
  print('x bukan string');
}
```
```sh
x adalah string
```

</br>

## 3\. Operator `!is`

Memeriksa apakah sebuah nilai bukan *instance* dari suatu tipe tertentu atau bukan *subtype* dari tipe tersebut. Jika ya, maka hasilnya adalah nilai `boolean` `true`, dan `false` jika tidak.

```Dart
var y = 10;
if (y !is String){
  print('y bukan string');
} else {
  print('y adalah string');
}
```
```sh
y bukan string
```

Ketika operator ini dapat membantu dalam melakukan pengecekan tipe data dan konversi tipe data pada variabel atau objek dalam program.