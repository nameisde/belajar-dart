## Boolean

Tipe data boolean pada Dart adalah tipe data yang hanya memiliki dua nilai, yaitu true atau false. Tipe data boolean biasanya digunakan dalam logika dan pengambilan keputusan dalam program.

Contok deklarasi variable bertipe data boolean

```Dart
void main() {
  bool isTrue = true;
  bool isFalse = false;
}
```

Kita dapat melakukan operasi logika seperti AND, OR, dan NOT pada tipe data boolean. Berikut adalah contoh penggunaan operator logika pada tipe data boolean:

```Dart
void main() {
  // Operator AND
  bool resultA = isTrue && isFalse; //false
  bool resultB = isTrue && !isFalse; //true

  // Operator OR
  bool resultC = isTrue || isFalse; //true
  bool resultD = isTrue || !isFalse; //false 

  // Operator NOT
  bool resultA = !isTrue; //false
  bool resultB = !isFalse; //true
}
```