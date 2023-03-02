## String

String adalah tipe data yang digunakan untuk menyimpan teks. String dapat ditulis dengan tanda kutip tunggal ('') atau ganda (""). Berikut adalah contoh penggunaan string pada Dart:

```Dart
void main() {
  String name = "Fahfudin Farhan";
  print("Hello, " + name + "!");
}
```
```sh
Hello, Fahfudin Farhan
```

Pada contoh di atas, kita menggunakan tipe data string untuk menyimpan nama "Fahfudin Farhan". Kemudian, kita menggunakan operator `+` untuk menggabungkan string.

Selain itu, tipe data string pada Dart memiliki beberapa metode yang berguna untuk memanipulasi atau mengakses data string. Berikut adalah beberapa metode yang sering digunakan pada tipe data string:

- `length` untuk mengembalikan panjang string
- `toUpperCase()` untuk mengubah seluruh karakter dalam string menjadi huruf besar
- `toLowerCase()` untuk mengubah seluruh karakter dalam string menjadi huruf kecil
- `substring(int start, [int? end])` untuk mengambil sebagian dari string dari indeks `start` hingga `end` (jika tidak diberikan, maka akan mengambil sampai akhir string)
- `split(String pattern)` untuk memisahkan string menjadi array substrigng berdasarkan pola yang diberikan
- `replaceAll(String from, String to)` untuk mengganti semua kemunculan substring `from` dengan substring `to` dalam string
- `contains(String substring)` untuk memeriksa apakah suatu substring terdapat dalam string
- `indeksOf(String substring, [int start =0])` untuk mencari indeks pertama kemunculan substring dalam string, dimulai dari indeks `start

Berikut adalah contoh penggunaan beberapa metode tipe data string tersebut:

```Dart
void main() {
  String message = "Hello, world!";
  print(message.length); 
  print(message.toUpperCase()); 
  print(message.substring(0, 5)); 
  print(message.split(",")); 
  print(message.replaceAll("o", "0")); 
  print(message.contains("world")); 
  print(message.indexOf("world")); 
}
```
```sh
13
HELLO, WORLD!
Hello
[Hello,  world!]
Hell0, w0rld!
true
7
```

</br>

## String Interpolation

String Interpolation adalah cara untuk memasukkan nilai variable ke dalam string dengan mudah. Kita dapat menggunakan tanda kurung kurawal `{}` untuk memasukkan nilai variabel ke dalam string. Berikut adalah contoh penggunaan string interpolcation pada Dart:

```Dart
void main() {
  String name = "Fahfudin Farhan";
  print("Hello, $name!");
}
```
```sh
Hello, Fahfudin Farhan!
```

</br>

## Character Backslash

Character Backslash digunakan sebagai karakter escape sequence untuk menandai karakter khusus dalam string seperti `"\n"` (baris baru), `"\t"` (tab), atau `"""` (tanda kutip ganda). Ketika karakter backslash diikuti oleh karakter khusus seperti `"n"` atau `"t"`, maka Dart akan mengenali karakter tersebut sebagai karakter khusus dan melakukan aksi yang sesuai.

Beberapa karakter khusus yang dapat ditandai dengan backslash, antara lain:

- `\n` untuk karakter baris baru (newline)
- `\t` untuk karakter tab
- `\"` untuk menulis tanda kutip ganda di dalam string
- `\'` untuk menulis tanda kutip tunggal di dalam string
- `\\` untuk menulis tanda backslash di dalam string

Berikut adalah contoh penggunaan character backslash pada Dart:

```Dart
void main() {
  print("Hello, world!\nHow are you?");
  print("He said, \"Hello, world!\"");
}
```
```sh
Hello, world!
How are you?
He said, "Hello, world!"
```

</br>

## String Concatenation  

String concatenation adalah proses penggabungan dua atau lebih string menjadi satu string yang lebih panjang. Terdapat dua cara untuk melakukan string concatenation, yaitu dengan menggunakan operator `+` atau dengan menggunakan operator `${}`.

Operator `+` digunakan untuk menggabungkan dua atau lebih string. Contoh penggunaannya sebagai berikut:

```Dart
void main(){
  String firstName = "Fahfudin";
  String lastName = "Farhan";
  String fullName = firstName + " " + lastName;

  print(fullName);
}
```
```sh
Fahfudin Farhan
```

Operator `${}` digunakan untuk memasukkan nilai variabel atau ekspresi ke dalam string. Contoh penggunaannya sebagai berikit:

```Dart
void main(){
  String firstName = "Fahfudin";
  String lastName = "Farhan";
  String fullName = "$firstName $lastName";

  print(fullName);
}
```
```sh
Fahfudin Farhan
```

</br>

## Multiline String

Multiline string adalah tipe string yang dapat digunakan untuk menulis teks dalam beberapa baris tanpa harus menggunakan karakter escape seperti `\n\. Pada Dart, multiline string dapat ditulis dengan menggunakan tiga tanda petik (""") atau tiga tanda kutip tunggal (''') sebagai pembatas awal dan akhir dari string.

Contoh penggunaan multiline string dengan tiga tanda petik ("""):

```Dart
void main() {
  String message = """
  Hello, world!
  This is a multiline string.
  It can span multiple lines.
  """;

  print(message);
}
```
```sh
  Hello, world!
  This is a multiline string.
  It can span multiple lines.
```

Multiline string sangat berguna untuk menulis teks yang panjang seperti dokumen atau laporan, karena memungkinkan untuk menghindari penggunaan karakter escape seperti `\n\ dan membuat kode lebih mudah dibaca dan ditulis.