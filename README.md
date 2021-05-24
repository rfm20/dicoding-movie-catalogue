# Latihan PWA movie-catalogue Dicoding

API yang dipakai dari [TheMovieDB](https://www.themoviedb.org/).

Buka file config.js pada `movie-catalogue/src/scripts/globals/config.js` dan ganti `YOUR_API_KEY` dengan `API Key TheMovieDB anda` 

### Cara menjalankan aplikasi
- Lakukan install `npm` dengan mengetikkan command berikut pada terminal code editor.
```
npm install
```
- Kemudian untuk menjalankannya dapat dilakukan dengan command berikut! 
```
npm run start-dev
```
Untuk membuka project, bisa dilihat di http://localhost:8080/

---
### Preview
![alt text](https://i.ibb.co/rZhNHDh/dicoding-movie-catalogue.png)

---
*★ Note 01 ★*

Ikuti langkah ini jika `package.json` belum terinstall `devDependencies` dan `Dependencies`

- Lakukan install `devDependencies` dengan mengetikkan command berikut pada terminal code editor.
```
npm install @babel/core @babel/preset-env babel-loader copy-webpack-plugin css-loader eslint html-webpack-plugin style-loader webpack webpack-cli webpack-dev-server webpack-merge --save-dev
```
- Selanjutnya install `Dependencies` dengan mengetikkan command berikut pada terminal code editor.
```
npm install regenerator-runtime
``` 
```
npm install serviceworker-webpack-plugin
```

---
*★ Note 02★*

Ikuti langkah ini jika `npm run start-dev` tidak bisa dijalankan

- Dalam file `package.json`, pada bagian scripts `webpack-dev-server` diganti dengan `webpack serve`
```json
"scripts": {
    "start-dev": "webpack-dev-server --config webpack.dev.js",
    "build": "webpack --config webpack.prod.js"
  },
```
Diubah menjadi
```json
"scripts": {
    "start-dev": "webpack serve --config webpack.dev.js",
    "build": "webpack --config webpack.prod.js"
  },
```
