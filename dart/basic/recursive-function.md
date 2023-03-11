# Recursive function

Recursive function adalah sebuah fungsi yang memanggil dirinya sendiri secara berulang untuk menyelesaikan tugas atau mencapai kondisi tertentu. Ketika sebuah fungsi memanggil dirinya sendiri, ia akan membentuk tumpukan panggilan atau "call stack" yang menampung semua pemanggilan fungsi yang belum selesai. Setelah kondisi yang diinginkan tercapai, fungsi akan mulai kembali ke pemanggilan sebelumnya dan mengembalikan nilai-nilai yang diperlukan.

Recursive function sangat berguna ketika kita perlu menyelesaikan tugas yang dapat dipecah menjadi beberapa sub-tugas yang serupa. Contoh umum penggunaan recursive function adalah dalam penghitungan bilangan faktorial atau pencarian jalur dalam struktur data seperti pohon.

</br>

Contoh implementasi recursive function pada Dart untuk menghitung bilangan faktorial adalah sebagai berikut:

```Dart
int factorial(int n) {
  if (n == 0 || n == 1) {
    return 1;
  } else {
    return n * factorial(n - 1);
  }
}

void main() {
  print(factorial(5)); // Output: 120
}
```

Dalam contoh di atas, kita memiliki fungsi `factorial` yang menerima satu parameter `n`. Jika `n` sama dengan 0 atau 1, fungsi akan mengembalikan nilai 1, karena faktorial dari 0 dan 1 adalah 1. Jika tidak, fungsi akan memanggil dirinya sendiri dengan argumen `n - 1` dan mengembalikan hasil perkalian antara `n` dan hasil panggilan rekursif dari fungsi `factorial` dengan argumen `n - 1`.

Pada akhirnya, kita memanggil fungsi `factorial` dengan parameter 5 dan mencetak hasilnya yang adalah 120, yang merupakan hasil faktorial dari 5.