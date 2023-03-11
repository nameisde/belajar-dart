# Main function

Main function adalah fungsi khusus dalam bahasa Dart yang merupakan titik masuk atau entry point dari program Dart. Setiap program Dart harus memiliki satu dan hanya satu `main function`.

</br>

Contoh sederhana dari `main function`:

```Dart
void main() {
  print('Hello, World!');
}
```

Dalam contoh di atas, `main function` adalah `main()` yang mencetak string "Hello, World!".

</br>

Main function juga dapat menerima argumen dari baris perintah saat menjalankan program. Argumen ini dapat diakses melalui parameter opsional `List<String>`.

```Dart
void main(List<String> arguments) {
  print('Jumlah argumen: ${arguments.length}');
  print('Argumen pertama: ${arguments.isNotEmpty ? arguments[0] : "tidak ada"}');
}
```

Dalam contoh di atas, `arguments adalah daftar argumen yang diberikan saat menjalankan program. Program mencetak jumlah argumen yang diberikan dan argumen pertama (jika ada).

</br>

Main function biasanya digunakan untuk memanggil fungsi lain atau menjalankan program secara keseluruhan. Selain itu, main function juga dapat digunakan untuk menangani exception dan menampilkan pesan kesalahan jika terjadi masalah saat menjalankan program.