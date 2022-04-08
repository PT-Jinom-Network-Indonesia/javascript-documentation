# Javascript documentation
Ini adalah starter template yang digunakan untuk dokumentasi program javascript

## Get started

Clone repository ini ke projek kamu

```
$ git clone https://github.com/PT-Jinom-Network-Indonesia/javascript-documentation.git supports
```

Lalu jalankan npm install untuk menginstall dependencies

```
$ cd supports && npm install
```

Selanjutnya sesuaikan kembali source project javascriptnya pada file `jsdoc.json` 

```json
{
  ...
  "source": {
    "include": [
      "../src" // source dimana tempat file javascript yang akan didokumentasikan
    ]
  }
  ...
}

```

Selanjutnya generate documentationnya dengan menjalankan perintah berikut

```
$ npm run docs
```


## Docblocks
Untuk Dokumentasi javascript kamu perlu menambahkan dockblock seperti berikut pada setiap file / module

```javascript
/**
 * Module helloworld
 * @module helloworld
 */

/**
 * Say hello
 * @param {string} name name
 * @memberof helloworld
 */
function say_hello(name = "") {
    console.log(`Hello, ${name}`);
}
```