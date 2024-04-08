
# Cara Bikin NPM untuk tea.xyz

Hal-hal yang diperlukan :

1. ChatGPT | https://chat.openai.com/
2. Akun NPMJS | https://www.npmjs.com/
3. Akun Github | https://github.com/
4. Code Editor (VSCode, Codespaces, Gitpod, dll)

## Bikin NPM Package

1. Buka https://chat.openai.com/
2. Kirim prompt :
```bash
Buatkan saya program sederhana javascript menggunakan dependecies untuk membuat npm package dari awal hinggal publish
```
3. Nanti akan muncul, bagaimana cara membuatnya yang perlu diperhatikan oleh kita adalah agar ada dependecies, dependent dan saat pengisian npm init. (jangan sampai salah)
4. Kita buka Codespaces, agar mudah saja
5. Masukan perintah ini (rubah nama paket sesuai dengan keinginan) :
```bash
mkdir nama-paket ; cd nama-paket; npm init
```
6. Nanti akan muncul, semacam promt untuk diisi
7. Usahakan nama package tidak sama dengan project orang lain
8. Untuk yang lainnya isi default aja (pencet enter-enter)
9. Pas bagian github, isi dengan alamat repo Github, contoh:
```bash
https://github.com/shidiqmuh0/npm-tea.git
```
10. Ketika sudah selesai, lanjut untuk menginstall npm package
11. Install package apa aja yag kita Masukan, Contoh :
```bash
npm i axios
```
12. Setelah itu kita buat index.js untuk isi dari npm package, isi saja sesuai dari generate ChatGPT :
```bash 
// double.js

function doubleNumber(num) {
  return num * 2;
}

module.exports = doubleNumber;
```
13. Setelah itu, kirim perintah di terminal
```bash
npm login
```

14. Tinggal publish
```bash
npm publish
```

## Untuk menambah dependent

1. Kita buat ulang seperti diatas, pas langkah ke 11, kita install nama package kita
```bash
npm nama-paket-yang-sudah-di-buat
```
2. Lanjutkan hingga publish

3. Setelah itu cek di npmjs apakah ada dependecies dan dependent

## Catatan
Kalo binggung, cobalah minta bantua ke ChatGPT, Gemini, dsb
