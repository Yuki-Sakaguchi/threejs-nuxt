# threejs-nuxt

> My supreme Nuxt.js project

## Build Setup

``` bash
# install dependencies
$ npm run install

# serve with hot reload at localhost:3000
$ npm run dev

# build for production and launch server
$ npm run build
$ npm run start

# generate static project
$ npm run generate
```

For detailed explanation on how things work, check out [Nuxt.js docs](https://nuxtjs.org).


## 参考
https://qiita.com/misaki_mofu/items/145ac26d600b429a6f8a

### まとめ
1. three.jsはひとつひとつのオブジェクトが数珠つながりでかなり大きいのでvueのdata()には入れない！
2. methodsに長ーいthree.jsコードを書こうとしない！
3. three.jsのオブジェクトが大きいということは、壊したり作り直したりを避けてなるべく使いまわししたほうがいい！
4. domとthree.jsのやりとりにはEventBusですると便利！
