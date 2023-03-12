# Method

Method pada Dart adalah sebuah blok kode yang terdiri dari satu atau beberapa pernyataan yang digunakan untuk melakukan tugas tertentu. Method biasanya didefinisikan di dalam suatu class dan dapat dipanggil atau digunakan oleh objek yang telah dibuat dari class tersebut.

</br>

Contoh sederhana dari definisi method di dalam sebuah class:

```Dart
class MyClass {
  void printMessage(){
    print('Hello World');
  }
}
```

</br>

Pada contoh di atas, `printMessage()` adalah sebuah method yang didefinisikan di dalam class `MyClass` dan bertugas mencetak pesan "Hello World".

</br>

Kemudian, kita dapat membuat objek dari class `MyClass` dan memanggil method `printMessage()` seperti ini:

```Dart
var myObject = MyClass();
myObject.printMessage();
```
```sh
Hello World
```

</br>

Dalam Dart, terdapat beberapa jenis method yang dapat didefinisikan di dalam suatu class, seperti constructor, getter, setter, dan method yang mengembalikan nilai (returning method).