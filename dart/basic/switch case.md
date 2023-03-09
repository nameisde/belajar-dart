## Switch case

Struktur kontrol untuk memeriksa nilai suatu variabel dan melakukan aksi yang sesuai dengan nilai tersebut.

```Dart
switch (variabel) {
  case nilaiA:
    // Blok kode jika variabel sama dengan nilaiA
    break;
  case nilaiB:
    // Blok kode jika variabel sama dengan nilaiB
    break;
  default:
    // Blok kode jika variabel tidak sama dengan semua nilai yang diberikan
}
```

</br>

Penjelasan mengenai struktur `switch case`:

- `switch` keyword untuk memulai struktur `switch case`
- `variabel` variabel yang akan diperiksa nilainya
- `case` keyword untuk menentukan nilai-nilai yang akan dibandingkan dengan variabel
- `nilaiA` nilai yang akan dibandingkan dengan variabel
- `break` keyword untuk menentukan `switch case` jika salah satu nilai tersebut terpenuhi
- `default` keyword untuk menentukan aksi yang akan dilakukan jika variabel tidak sama dengan nilai yang diberikan