# Null

Sebuah nilai yang menunjukkan bahwa suatu variabel tidak memiliki nilai atau kosong. Jika suatu variabel dideklarasikan dengan tipe data *nullable*, maka variabel tersebut dapat menyimpan nilai `null`.

Tipe data *nullable* pada Dart ditandai dengan tanda tanya (`?`) di akhir tipe data. Misalya, tipe data `int?` adalah tipe data *nullable* dari `int`.

```Dart
void main() {
  int? nilai;
  print(nilai);

  String? teks = 'hello';
  teks = null;
  print(teks);

  List<int?> angka = [1, 2, 3];
  angka = null;
  print(angka);
}
```
```sh
null
null
null
```

Penggunaan `null` pada Dart sangat penting untuk menghindari terjadinya error atau pengecualian yang tidak diinginkan ketika suatu variabel tidak memiliki nilai atau kosong. Oleh karena itu, sebaiknya selalu gumakan tipe data *nullable* jika suatu variabel mungkin kosong atau tidak memiliki nilai.