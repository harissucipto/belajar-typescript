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
