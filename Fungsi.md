# Fungsi pada Typescript

Fungsi pada javascript biasa ada dua cara ditulis yaitu fungsi dengan nama dan fungsi anonim. Berikut contoh penulisan fungsi bernama dan fungsi anonim:

```js
// fungsi bernama
function tambah(x, y) {
  return x + y;
}

// fungsi anonim
let tambahkan = function(x, y) {
  return x + y;
};
```

Pada typescript kita menambahkan deklarasi tipe data pada saat penulisan fungsi. berikut cara penulisannya:

```js
// fungsi bernama
function tambah(x: number, y: number): number {
  return x + y;
}

// fungsi anonim
let tambahkan = function(x: number, y: number): number {
  return x + y;
};
```

Dalam contoh diatas pada fungsi `tambah` memiliki input `x` dan `y` dimana keduanya memiliki tipe data `Number`. Fungsi `tambah` juga memiliki tipe data yaitu `Number` dimana fungsi ini hanya akan mengeluarkan hasil berupa angka.
