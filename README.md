# Halo Suzuki

## Framework7 CLI Options

Framework7 app created with following options:

```
{
  "cwd": "D:\\PROJECT\\MOBILE\\new_suzuki",
  "type": [
    "cordova"
  ],
  "name": "Halo Suzuki",
  "framework": "core",
  "template": "single-view",
  "bundler": "webpack",
  "cssPreProcessor": false,
  "theming": {
    "customColor": false,
    "color": "#007aff",
    "darkTheme": false,
    "iconFonts": true,
    "fillBars": false
  },
  "customBuild": false,
  "webpack": {
    "developmentSourceMap": true,
    "productionSourceMap": true,
    "hashAssets": false,
    "preserveAssetsPaths": false,
    "inlineAssets": true
  },
  "pkg": "com.nieve.hallosuzuki",
  "cordova": {
    "folder": "cordova",
    "platforms": [
      "android"
    ],
    "plugins": [
      "cordova-plugin-statusbar",
      "cordova-plugin-keyboard",
      "cordova-plugin-splashscreen",
      "cordova-plugin-wkwebview-file-xhr"
    ]
  }
}
```

## NPM Scripts

* 🔥 `start` - run development server
* 🔧 `dev` - run development server
* 🔧 `build-dev` - build web app using development mode (faster build without minification and optimization)
* 🔧 `build-prod` - build web app for production
* 📱 `build-dev-cordova` - build cordova app using development mode (faster build without minification and optimization)
* 📱 `build-prod-cordova` - build cordova app

## WebPack

There is a webpack bundler setup. It compiles and bundles all "front-end" resources. You should work only with files located in `/src` folder. Webpack config located in `build/webpack.config.js`.

Webpack has specific way of handling static assets (CSS files, images, audios). You can learn more about correct way of doing things on [official webpack documentation](https://webpack.js.org/guides/asset-management/).
## Cordova

Cordova project located in `cordova` folder. You shouldn't modify content of `cordova/www` folder. Its content will be correctly generated when you call `npm run cordova-build-prod`.



## Assets

Assets (icons, splash screens) source images located in `assets-src` folder. To generate your own icons and splash screen images, you will need to replace all assets in this directory with your own images (pay attention to image size and format), and run the following command in the project directory:

```
framework7 generate-assets
```

Or launch UI where you will be able to change icons and splash screens:

```
framework7 generate-assets --ui
```

## Documentation & Resources

* [Framework7 Core Documentation](https://framework7.io/docs/)



* [Framework7 Icons Reference](https://framework7.io/icons/)
* [Community Forum](https://forum.framework7.io)

## Support Framework7

Love Framework7? Support project by donating or pledging on patreon:
https://patreon.com/vladimirkharlampidi

## Additional information

Project ini berbasis hybrid application menggunakan Cordova dan Framework7.
Langkah pertama yang dibutuhkan sebagai berikut :

    1.	Pastikan sudah menginstall Node JS. [online dokumentasi (https://nodejs.dev/) tutorial , panduan , dan contoh].
    
    2.	Kemudian install Cordova [online dokumentasi (https://cordova.apache.org/docs/en/7.x/) tutorial , panduan , dan contoh]

Langkah kedua cara menjalankan kode program sebagai berikut :
    
    1.	Masuk ke dalam directory atau path dari aplikasi menggunakan Command Prompt. 
        
            Contoh => D:\DataCoding\HaloSuzuki\  
    
    2.	Setelah masuk ke dalam directory install node module terlebih dahulu dengan perintah berikut :
        
            npm install
    
    3.	Kemudian build aplikasi dengan perintah berikut :
        
            npm run build-prod-cordova android
        
    4.	Selanjutnya untuk jalankan aplikasi dapat menggunakan perintah berikut:
        
            Framework7 cordova run android
        
Note : Source Utama terdapat pada /root_diretory/src/. List page apa saja yang terdapat dalam aplikasi berada pada  /root_diretory/src/pages/. Lalu list asset terdapat pada /root_diretory/src/static. Kemudian Fucntion menggunakan javascript terdapat pada /root_diretory/src/js/app.js

Jika sudah berhasil menjalankan aplikasi , selanjutnya adalah cara mengatur config pada aplikasi :
    
    1.	Untuk mengatur configurasi environment (URL API, Version,dll) pada production , dev, dan pra-production dapat mengubah [var getData ] yang terdapat pada app.js.
    
    2.	Untuk mengatur root navigasi pada page dapat mengubahnya pada file routes.js.


