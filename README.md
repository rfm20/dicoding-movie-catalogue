# Latihan PWA movie-catalogue Dicoding

### Cara menjalankan aplikasi
- Lakukan install `devDependencies` dengan mengetikkan command berikut pada terminal code editor.
```
npm install @babel/core @babel/preset-env babel-loader copy-webpack-plugin css-loader eslint html-webpack-plugin style-loader webpack webpack-cli webpack-dev-server webpack-merge --save-dev
```
- Selanjutnya install `Dependencies` dengan mengetikkan command berikut pada terminal code editor.
```
npm install regenerator-runtime
```
- Dalam file package.json, pada bagian scripts `webpack-dev-server` diganti dengan `webpack serve`
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
- Kemudian untuk menjalankannya dapat dilakukan dengan command berikut! 
```
npm run start-dev
```
Untuk membuka project, bisa dilihat di http://localhost:8080/

---
### Preview
![alt text](___)
