# Map

Map adalah salah satu struktur data pada bahasa pemrograman yang terdiri dari pasangan `key-value`. `Key` digunakan untuk mengidentifikasi value yang terkait dengannya. Map dapat digunakan untuk menyimpan data dengan format `key-value` yang bersifat dinamis dan dapat dimodifikasi.

</br>

Map, dapat dideklarasikan menggunakan *sintax* berikut:

```Dart
Map<String, int> mapHarga = {'apel': 5000, 'mangga': 8000,'pisang': 3000};
```

</br>

Berikut adalah beberapa cara manipulasi data yang dapat dilakukan pada map:

</br>

## 1\. Menambah pasangan `key-value` ke dalam map

Kita dapat menambah pasangan `key-value` ke dalam map dengan menggunakan metode `.put()` atau dengan langsung menambahkan pasangan `key-value` tersebut ke dalam map.

```Dart
Map<String, int> mapHarga = {'apel': 5000, 'mangga': 8000, 'pisang': 3000};

// Metode .put()
mapHarga.put('jeruk', 6000);

// Menambahkan pasangan key-value
mapHarga['durian'] = 15000;

print(mapHarga);
```
```sh
{'apel': 5000, 'mangga': 8000, 'pisang': 3000, 'jeruk': 6000, 'durian': 15000}
```

</br>

## 2\. Mengubah value pada pasangan `key-value` yang sudah ada

Kita dapat mengubah value pada pasangan `key-value` yang sudah ada dengan operator `[]`

```Dart
Map<String, int> mapHarga = {'apel': 5000, 'mangga': 8000, 'pisang': 3000};

mapHarga['mangga'] = 9000;

print(mapHarga);
```
```sh
{'apel': 5000, 'mangga': 9000, 'pisang': 3000}
```

</br>

## 3\. Menghapus pasangan `key-value` dari map

Kita dapat menghapus pasangan `key-value` dari map dengan menggunakan metode `.remove()`.

```Dart
Map<String, int> mapHarga = {'apel': 5000, 'mangga': 8000, 'pisang': 3000};

mapHarga.remove('mangga');

print(mapHarga);
```
```sh
{'apel': 5000, 'pisang': 3000}
```

</br>

## 4\. Mendapatkan jumlah pasangan `key-value` pada map

Kita dapat mendapatkan jumlah pasangan `key-value` pada map dengan menggunakan metode `.length`.

```Dart
Map<String, int> mapHarga = {'apel': 5000, 'mangga': 8000, 'pisang': 3000};

print(mapHarga.length);
```
```sh
3
```
