# Interface dan Class pada Typescript

## Interface

Kelebihan dari typescript adalah fokus pada pengecekan tipe data. Penggunaan Interface adalah sebagai kontrak tipe data input antara fungsi atau class dengan diluar dari kode.

```js
interface KonfigurasiPersegiPanjang {
  panjang?: number;
  lebar?: number;
}

function hitungPersegiPanjang(
  konfigurasi: KonfigurasiPersegiPanjang
): { luas: number, keliling: number } {
  let persegiPanjang = { luas: 0, keliling: 0 };
  if (konfigurasi.panjang && konfigurasi.lebar) {
    persegiPanjang.luas = konfigurasi.panjang * konfigurasi.lebar;
    persegiPanjang.keliling = (konfigurasi.panjang + konfigurasi.lebar) * 2;
  }
  return persegiPanjang;
}

let hitunganPersegiPanjang = hitungPersegiPanjang({ panjang: 10, lebar: 10 });
```

Dengan menggunakan `interface` maka untuk menggunakan fungsi `hitungPersegiPnajang` mesti memenuhi syarat tipe data pada `KonfigrasiPersegiPanjang`.

## Class

Class adalah bagian utama dari pemrograman berbasis objek. Jika javascript awalnya hanya menggunakan fungsi dan inhiritance berbasis prototype kini mulai ECMAScript 6 telah mendu
kung penggunaan Class.
Berikut contoh Class:

```js
class Salam {
  katasalam: string;
  constructor(pesan: string) {
    this.katasalam = pesan;
  }
  salam() {
    return "Hai, " + this.katasalam;
  }
}

let berisalam = new Salam("Agung!");
```

Pada baris terakhir kita membuat satu instanece `Salam` dengan pesan `"Agung!"`.
