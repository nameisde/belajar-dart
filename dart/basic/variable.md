## Variable

Variable merupakan tempat untuk menyimpan sebuah data dan dapat digunakan berulang kali. Variable memiliki tipe data dan nama variable.

</br>

## Membuat variable

Untuk membuat sebuah variable dapat menggunakan format `TipeData namaVariable`; dan penamaan variable diusakan menggunakan `camelCase` seperti `firstName`, `lastName`.

```dart
void main() {
    String name;
    name = 'Fahfudin Farhan';
}
```
```sh
Fahfudin Farhan
```

</br>

## Deklarasi langsung variable

Kamu juga bisa langsung mendeklarasikan nilai dari sebuah variable dengan cara menuliskan perintah `TipeData namaVariable = isi variable;`

```dart
void main() {
    String name = 'Fahfudin Farhan';
}
```
```sh
Fahfudin Farhan
```

</br>

## Var

Saat membuat variable secara langsung, kita bisa menggunakan `var` sebagai pengganti dari `TipeData`-nya. `TipeData` akan dibaca secara otomatis oleh Dart, sehingga kita tidak perlu menentukan secara manual `TipeData` yang dimaksud.

Var dapat dituliskan dengan perintah `var namaVariable = value;`

```dart
void main() {
    var name = 'Fahfudin Farhan';
}
```
```sh
Fahfudin Farhan
```

</br>

## Final

Variable pada bahasa pemrograman Dart dapat dideklarasikan secara ulang. Semisalnya kita membuat sebuah variable `nama` dengan `value` "Fahfudin", kita dapat mengubah nilai `value` dari `nama` dengan nilai lainnya.

Tetapi, ada situasi dimana kita tidak menginginkan sebuah variable dapat dideklarasikan secara ulang. Maka, kamu dapat menggunakan `final`.

```Dart
final tipeData namaVariable = value;
final namaVariable = value;
```

```Dart
void main() {
    var firstName = 'Fahfudin';
    final lastName = 'Farhan';

    firstName = 'Faiz';
    lastName = 'Ananta';

    print(firstName);
    print(lastName);
}
```

```sh
Error cant assign to the final variable 'lastName'
```

</br>

## Const

Const digunakan untuk menjadikan sebuah variable dan nilainya menjadi `immutable` (tidak bisa diubah sama sekali).

```Dart
final arrayA = [1, 2, 3];
const arrayB = [1, 2, 3];

arrayA[0] = 5;
arrayB[0] = 5;

print(arrayA);
print(arrayB);
```

</br>

## Late

Pada Dart, variable akan dideklarasikan nilainya ketika variable tersebut dibuat, tetapi kamu juga bisa mendeklarasikan variable tersebut nanti. 

Untuk melakukan hal tersebut kamu dapat menggunakan `late` pada awal mendeklarasikan sebuah variable.

```Dart
void main() {
   late var value = getValue();
   print('Display value');
   print(value);
}

String getValue() {
   print('getValue dipanggil');
   return 'Fahfudin Farhan';
}
```
```sh
Display value
getValue() dipanggil
Fahfudin Farhan
```