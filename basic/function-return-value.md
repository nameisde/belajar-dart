# Function return value

Function return value pada Dart adalah nilai atau data yang dikembalikan oleh suatu function setelah melakukan operasi atau pemrosesan tertentu. Setiap function di Dart dapat mengembalikan satu nilai atau objek, atau dapat juga tidak mengembalikan nilai apapun dengan menggunakan kata kunci `void`.

</br>

Untuk mendefinisikan function dengan nilai pengembalian, Anda dapat menentukan tipe data pengembalian pada deklarasi function menggunakan sintaksis berikut:

```Dart
int tambah(int a, int b) {
  int hasil = a + b;
  return hasil;
}
```

</br>

Pada contoh di atas, function `tambah` mengambil dua parameter bertipe `int` dan mengembalikan hasil penjumlahan keduanya dalam bentuk `int`. Setelah melakukan operasi penjumlahan, function mengembalikan nilai `hasil` menggunakan kata kunci `return`.

</br>

Selain itu, Anda juga dapat menggunakan `function short expression` untuk mendefinisikan function dengan nilai pengembalian, seperti contoh berikut:

```Dart
int tambah(int a, int b) => a = b;
```