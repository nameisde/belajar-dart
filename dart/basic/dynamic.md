## Dynamic

Dynamic adalah tipe data yang dapat menampung nilai apapun. Ini berarti Anda dapat mengubah tipe data dynamic saat runtime, sesuai dengan nilai yang sedang disimpan.

Dynamic sering digunakan ketika tipe suatu data tidak diketahui secara pasti, atau ketika nilainya bisa berubah dari waktu ke waktu. Dynamic juga digunakan ketika kita ingin memanipulasi nilai dalam cara yang fleksibel dan dinamis, tanpa harus memperhatikan tipe data aslinua.

Contoh penggunaan dynamic, sebagai berikut:

```Dart
void main() {
  dynamic value = 42;
  print(value);

  value = "Hello, World!";
  print(value);
}
```
```sh
42
Hello, World!
```

Sebaiknya, dynamic digunakan dengan sangat hati-hati. Karena dapat menyebabkan kesalahan dan bug yang sulit dilacak. Pastikan selalu untuk mengetahui tipe data yang diharapkan, untuk menghindari penggunaan dynamic secara berlebihan pada kode program Anda.