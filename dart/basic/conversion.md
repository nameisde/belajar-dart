# Conversion

Terdapat beberapa cara untuk melakukan konversi atau perubahan tipe data dari suatu nilai ke tipe data yang lain. Berikut adalah beberapa cara yang umum digunakan:

</br>

## 1\. Konversi secara eksplisit menggunakan operator `as`.

Operator `as` digunakan untuk mengkonversi tipe data secara eksplisit. Misalnya, untuk mengkonversi nilai dari tipe data `int` ke tipe data `double`, Anda dapat menggunakan operator `as double`.

```Dart
void main(){
  int nilaiInt = 10;
  double nilaiDouble = nilaiInt as double;

  print(nilaiDouble);
}
```
```sh
10
```

Namun, perlu diingat bahwa operator `as` hanya dapat digunakan jika tipe data yang akan dikonversi adalah subtype dari tipe data yang dituju.

</br>

## 2\. Konversi secara implisit 

Konversi secara implisit terjadi ketika kita mengubah atau memasukkan nilai dari suatu tipe data ke tipe data lainnya.

Contohnya, ketika kita menghitung nilai dengan tipe data `integer` dan `double` dalam satu operasi matematika, hasilnya secara otomatis dikonversi oleh Dart ke tipe data `double`.

```Dart
void main() {
  int nilaiInt = 10;
  double nilaiDouble = 3.14;
  double hasil = nilaiInt + nilaiDouble;

  print(hasil);
}
```
```sh
13.14
```

Pada contoh di atas, nilai integer `10` dan double `3.14` dijumlahkan, dan hasilnya secara otomatis dikonversi oleh Dart ke tipe data double, sehingga hasilnya menjadi `13.14`.


</br>

## 3\. Menggunakan metode konversi yang disediakan oleh tipe data

Tipe data pada Dart menyediakan beberapa metode dan fungsi untuk melakukan konversi nilai dari suatu tipe data ke tipe data lainnya. Berikut adalah beberapa konversi yang disediakan oleh tipe data pada Dart.

A\. Konversi antara tipe data `number`

- `toDouble()` untuk mengubah nilai `int` atau `float` ke dalam tipe data `double`
- `toInt()` untuk mengubah nilai `double` atau `float` ke dalam tipe data `int`

```Dart
void main() {
  double nilaiDouble = 3.14;
  int nilaiInt = nilaiDouble.toInt();
  print(nilaiInt);

  int nilaiIntX = 10;
  double nilaiDoubleX = nilaiIntX.toDouble();
  print(nilaiDoubleX); 
} 
}
```
```sh
3
10.0
```
</br>

B\. Konversi antara tipe data `string` dan `number`

`toString()` untuk mengubah nilai bilangan ke dalam bentuk string
`parse()` untuk mengubah nilai string ke dalam tipe data bilangan

```Dart
void main(){
  int nilaiInt = 10;
  String nilaiString = nilaiInt.toString();
  print(nilaiString);

  String nilaiStringX = "3.14";
  double nilaiDoubleX = double.parse(nilaiStringX);
  print(nilaiDoubleX);
}
```
```sh
10
3.14
```

</br>

C\. Konversi antara tipe data `boolean` dan `string`

- `toString()` mengubah nilai boolean ke dalam bentuk string
- `toLowerCase()` mengubah nilai string ke dalam bentuk lowercase
- `toUpperCase()` mengubah nilai string ke dalam bentuk uppercase

```Dart
void main() {
  bool isAktif = true;
  String isAktifString = isAktif.toString();
  print(isAktifString);

  String stringLower = "true";
  String stringToLower = stringLower.toUpperCase();
  print(stringToLower);
}
```
```sh
true
TRUE
```

</br>

D\. Konversi antara tipe data `list` dan `set`

- `toList()` mengubah nilai `set` ke dalam bentuk `list`
- `toSet()` mengubah nilai `list` ke dalam bentuk `set`

```Dart
void main() {
  List<int> list = [1, 2, 3];
  Set<int> toSet = list.toSet();
  print(toSet);

  Set<int> set = {1, 2, 3};
  List<int> toList = set.toList();
  print(toList);
}
```
```sh
{1, 2, 3}
[1, 2, 3]
```

</br>

E\. Konversi antara tipe data `map` dan `list`

- `keys.toList()` mengubah nilai `key` dari `map` ke dalam bentuk `list`
- `values.toList()` mengubah nilai value dari `map` ke dalam bentuk `list`
- `Map.fromEntries()` mengubah nilai `list of map entries` ke dalam bentuk `map`

```Dart
void main() {
  Map<String, int> map = {"apple": 1, "banana": 2, "orange": 3};
  print(map);

  List<String> keys = map.keys.toList();
  print(keys);

  List<int> values = map.values.toList();
  print(values);
}
```
```sh
{apple: 1, banana: 2, orange: 3}
[apple, banana, orange]
[1, 2, 3]
```