# Pengenalan Typescript

Typescript adalah bagian dari javascript. Jika kita menulis kode dengan typescript maka kode ini akan di compilasi menjadi kode javascript biasa.

Sebelum memulai kita mesti menginstall Typescript di machine kita dengan menjalankan perintah berikut di terminal:
`npm install -g typescript`

Lalu kita tulis kode dengan membuat file dengan ekstensi `.ts` contohnya `salam.ts`.

```js
// file salam.ts
function salam(nama) {
  return "Halo, " + nama;
}

let namasaya = "Agung";

document.body.textContent = salam(namasaya);
```

Setelah itu kita mencompile dengan menjalankan perintah berikut di terminal:
`tsc salam.ts`

Hasil dari kompilasi adalah file `.js` yang dapat kita jalankan.
