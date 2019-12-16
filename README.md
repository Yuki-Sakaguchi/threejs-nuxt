# threejs-nuxt
## DEMO
https://5df79bab13b6c4b6065d1af3--clever-jones-12d6ec.netlify.com/

## 参考
https://qiita.com/misaki_mofu/items/145ac26d600b429a6f8a

### まとめ
1. three.jsはひとつひとつのオブジェクトが数珠つながりでかなり大きいのでvueのdata()には入れない
2. methodsに長ーいthree.jsコードを書こうとしない
3. three.jsのオブジェクトが大きいということは、壊したり作り直したりを避けてなるべく使いまわししたほうがいい
4. domとthree.jsのやりとりにはEventBusですると便利

### その他
- nuxtで作ってgithubにあげてnetlifyにデプロイするの簡単すぎてやばい
- githubのリポジトリとビルドコマンドを入れればSPAが簡単にデプロイできる
