# Function

Function adalah blok kode yang dapat digunakan untuk melakukan tugas tertentu. Function dapat mengambil input dalam bentuk parameter, melakukan beberapa operasi atau pemrosesan, dan mengembalikan output. Function digunakan untuk memecah kode menjadi bagian yang lebih kecil, lebih mudah dikelola, dan dapat digunakan kembali di beberapa tempat dalam program.

</br>

Pada Dart, sintaks untuk mendefinisikan function adalah sebagai berikut:

```Dart
returnType functionName(parameterA, parameterB, ...) {
   // Body of cuntion
   return value;
}
```

</br>

- `returnType` tipe data nilai kembalian dari function. Jika function tidak mengembalikan nilai, kita dapat menggunakan tipe data `void`
- `functionName` nama yang diberikan kepada function tersebut
- `parameterA`, `parameterB`, ... parameter yang diterima oleh function. Kita dapat menentukan tipe data parameter dengan menambahkan tipe data sebelum nama parameter

</br>

Contoh sederhana penggunaan function pada Dart:

```Dart
void greet(String name) {
  print('Hello, $name!');
}

void main() {
  greet('Alice'); // Hello, Alice
  greet('Bob'); // Hello, Bob
  greet('Charlie'); // Hello, Charlie
}
```

</br>

Pada contoh di atas, function `greet` didefinisikan dengan parameter `name` yang bertipe `String` dan bertujuan untuk mencetak pesan sapaan untuk setiap nama yang diberikan.