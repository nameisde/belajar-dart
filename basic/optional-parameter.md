# Optional parameter

Optional parameter adalah parameter yang tidak diwajibkan saat memanggil sebuah function. Optional parameter dapat memberikan nilai default jika tidak diberikan nilai saat pemanggilan function. Dalam Dart, ada dua jenis optional parameter yaitu Positional parameter dan Named parameter.

</br>

## 1\. Positional parameter

Positional parameter adalah parameter yang diberikan secara posisi atau urutan saat memanggil function. Dalam Dart, positional parameter dibuat dengan menempatkan parameter di dalam kurung siku `[]` setelah parameter wajib pada definisi function. Jika tidak ada nilai yang diberikan saat memangigl function, maka nilai default dari positional parameter akan digunakan.

</br>

Contoh penggunaan positional parameter:
```Dart
void greet(String name, [String greeting = 'Hello']) {
  print('$greeting, $name!');
}

void main() {
  greet('Alice'); // Hello, Alice!
  greet('Bob', 'Hi'); // Hi, Bob!
  greet('Charlie', 'Hola'); // Hola, Charlie!
}
```

Pada contoh di atas, parameter `greeting` adalah positional parameter dan diatur sebagai parameter opsional dengan memberikan nilai default `'Hello'`. Saat function dipanggil, jika kita hanya memberikan nilai untuk parameter `name`, maka nilai default untuk `greeting` adalah `'Hello'`. Jika kita memberikan nilai untuk kedua parameter, maka nilai untuk `greeting` akan diganti dengan nilai yang diberikan.

</br>

## 2\. Named parameter

Named parameter adalah parameter yang diberikan dengan memberikan nama parameter saat memanggil function. Dalam Dart, named parameter dibuat dengan menempatkan parameter di dalam kurung kurawal `{}` setelah parameter wajib pada definisi sebuah function.

Saat memanggil function, kita dapat memberikan nama parameter dan nilai parameter secara bersamaan. Jika tidak ada nilai yang diberikan saat memanggil function, maka nilai default dari named parameter akan digunakan.

</br>

Contoh penggunaan named parameter:

```Dart
void greet(String name, {String greeting = 'Hello', String suffix = '!'}) {
  print('$greeting, $name$suffix');
}

void main() {
  greet('Alice'); // Hello, Alice!
  greet('Bob', greeting: 'Hi'); // Hi, Bob!
  greet('Charlie', greeting: 'Hola', suffix: ' amigos'); // Hola, Charlie amigos!
}
```

</br>

Pada contoh di atas, parameter greeting dan suffix adalah named parameter dan diatur sebagai parameter opsional dengan memberikan nilai default `'Hello'` dan `!`. 

Saat memanggil function, kita dapat memberikan nilai untuk kedua parameter dengan memberikan nama parameter bersama nilai yang diberikan. Jika kita hanya memberikan nilai untuk parameter name, maka nilai default untuk greeting dan suffix akan digunakan.