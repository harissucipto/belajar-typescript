# Pengenalan Tyepscript

Typescript adalah bahasa pemograman yang akan memberikan powerup ke javascript, kenapa powerup ? sesuai dengan namanya typescript akan memberikan salah satu fiturnya yaitu **type safety** ke pada javascript agar mencegah program melakukan hal yang salah.

contoh hal yang tidak kita inginkan atau salah menurut kita.

```js

3 + []
// string "3"

let obj = {}
obj.foo
// hasilnya undefined

function a(b) {
  return b/2
}
a("z")
// hasilnya Nan


```

dengan typescript hal tersebut akan di tangkap sebagai error, seperti dibawah ini.

```ts
3 + []
// Error TS2365: Operator '+' cannot be applied to types '3'

let obj = {}
obj.foo
// Error: You forgot to define the property "foo" on obj.

function a(b) {
  return b/2
}
a("z")
// Error: The function "a" expects a number,
// but you gave it a string.

```