# Function short expression

Function short expression atau disebut dengan arrow function adalah cara alternatif untuk mendefinisikan function dalam bahasa Dart. Dalam function short expression, sintaksisnya lebih singkat dan dapat diimplementasikan dalam satu baris kode.

</br>

Contoh sintaksis function short expression:

```Dart
int tambah(int a, int b) => a + b;
```

</br>

Pada contoh di atas, `tambah` adalah nama function yang menerima dua parameter bertipe `int` dan mengembalikan hasil penjumlahan keduanya. Perhatikan bahwa tanda `=>` digunakan untuk menggantikan kata kunci `return`, sehingga kode menjadi lebih singkat.

Function short expression juga dapat digunakan untuk function dengan optional parameter dan named parameter, sebagai berikut:

```Dart
// Optional parameter
int hitungLuas(int panjang, [int lebar = 1]) => panjang * lebar;

// Named parameter
String buatKontak({required String nama, required String nomor}) => '$nama: $nomor';
```

</br>

Perhatikan bahwa pada function hitungLuas, tanda kurung siku `[]` digunakan untuk menandakan parameter lebar bersifat opsional dengan nilai default `1`. Sedangkan pada function buatKontak, tanda kurung kurawal `{}` digunakan untuk menandakan kedua parameter (`nama` dan `nomor`) adalah named parameter yang wajib diisi dan ditandai dengan kata kunci required.

Dalam keseluruhan, penggunaan function short expression dapat mempercepat dan mempermudah penulisan function dalam bahasa Dart, terutama untuk function sederhana dengan implementasi yang singkat.