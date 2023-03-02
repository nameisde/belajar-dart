## Number

Number adalah tipe data angka yang memiliki dua jenis tipe, yaitu `int` dan `double.

- `int` adalah tipe data bilangan bulat
- `double` adalah tipe data bilangan desimal

Penulisan (,) koma pada `double` menggunakan (.) titik, bukan (,) koma. Jadi, kita akan ketika ingin mendefinisikan sebuah bilangan desimal (0,5) ditulis (0.5).

```Dart
void main() {
  int number1 = 10;
  double number2 = 10.5;

  print(number1);
  print(number2);
}
```
```sh
10
10.5
```

</br>

## Num

Jika kamu ingin menggunakan tipe data number yang bisa `int` ataupun `double`, gunakanlah tipe data `num`.

```Dart
void main() {
  num number = 10;
  print(number);

  number = 10.5;
  print(number);
}
```
```sh
10
10.5
```