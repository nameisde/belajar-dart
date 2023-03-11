# Scope

Scope dalam bahasa Dart mengacu pada wilayah di dalam program di mana variabel dan fungsi dapat diakses. Ada dua jenis scope dalam bahasa Dart:

- Global scope
- Local scope

</br>

## Global scope

Ruang lingkup di mana variabel dan fungsi dapat diakses dari seluruh bagian program. Variabel yang dideklarasikan di luar fungsi atau blok kode memiliki global scope. Untuk membuat variabel dengan global scope, kita dapat mendeklarasikannya di luar fungsi atau blok kode. Contohnya adalah sebagai berikut:

```Dart
var globalVariable = 'Hello, World!';

void main() {
  print(globalVariabel);
}
```
```sh
Hello, World!
```

</br>

## Local scope

Ruang lingkup di mana variabel dan fungsi hanya dapat diakses dari bagian tertentu di dalam program, seperti fungsi atau blok kode tertentu. Variabel yang dideklarasikan di dalam fungsi atau blok kode memiliki local scope dan hanya dapat diakses dari dalam fungsi atau blok kode tersebut. Berikut adalah contohnya:

```Dart
void main() {
  var localVariable = 'Hello, Dart!';

  print(localVariable); // Output: Hello, Dart!

  function1();
}

void function1() {
  var localVariable = 'Hello, Function!';

  print(localVariable); // Output: Hello, Function!
}
```

Di dalam contoh di atas, variabel `localVariable` yang dideklarasikan di dalam fungsi `main` hanya dapat diakses dari dalam fungsi `main` itu sendiri. Variabel `localVariable` yang dideklarasikan di dalam fungsi `function1` hanya dapat diakses dari dalam fungsi `function1` itu sendiri.