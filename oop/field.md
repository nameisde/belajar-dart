# Field

Fied adalah variabel atau properti yang terdapat pada suatu objek. Field dapat berupa variabel, objek, fungsi, atau bahkan class yang dapat diakses dari dalam objek. 

Field Biasanya didefinisikan di dalam class dan dapat diakses melalui objek yang telah di buat dari class tersebut.

</br>

Contohnya, jika kita memiliki class `Person`, kita dapat menambahkan field seperti `name`, `age`, dan `gender`.

```Dart
class Person {
  String name;
  int age;
  String gender;
}
```

</br>

Kemudian kita dapat membuat objek dari class `Person` dan mengakses field yang telah didefinisikan seperti berikut:

```Dart
var person = Person();
person.name = 'John';
person.age = 24;
person.gender = 'Male';

print('Name: ${person.name}, Age: ${person.age}, Gender: ${person.gender}')
```

</br>

Output dari program tersebut adalah sebagai berikut:

```sh
Name: John, Age: 24, Gender: Male
```