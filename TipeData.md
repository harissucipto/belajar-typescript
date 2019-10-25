# Tipe Data pada Typescript

Bila pada javascript biasa kita dapat meng-assign data ke variabel dengan bebas maka pada typescript tidak bisa. Pada typescript kita hanya boleh/bisa meng-assign value ke variabel dengan tipe data yang telah di tentukan saat inisialisasi variabel.

## Tipe data dasar

Tipe data dasar pada typescript terdiri dari tipe primitif seperti `Boolean`, `Number`, `String` lalu terdapat tipe yang bisa di enumerasi seperti `Array`, `Tuple` lalu ada `Enum`, `Any`, `Object` dan yang jarang digunakan seperti `Void`, `Undefined`, `Null` dan `Never`.

### Boolean

Tipe data yang paling dasar adalah `boolean` yaitu berupa `true`/`false`

```js
let sudahKaya: boolean = false;
```

### Number

Pada typescript untuk menginisialisasi variabel berisi angka kita perlu menentukan type `number`. Seperti pada javascript biasa di typescript angka disimpan dalam bentuk floating point.Selain dari angka desimal biasa kita juga dapat menggunakan hexadesimal,biner dan oktal.

```js
let desimal: number = 6;
let hexadesimal: number = 0xf00d;
let biner: number = 0b1010;
let oktal: number = 0o744;
```

### String

Untuk variabel berisi teks kita menggukanak tipe data `string`. Seperti biasa kita bisa menggunakan tanda petik `'`, petik dobel `"` atau ` backtick untuk membuat teks.

```js
let color: string = "blue";
color = "red";
```

Typescript juga mendukung _template string_.

```js
let nama: string = `Code Mode`;
let anggota: number = 2;
let perkenalan: string = `Halo, kami dari ${nama}, kami memiliki ${anggota} anggota.`;

// Halo, kami dari Code Mode, kami memiliki 2 anggota.
```
