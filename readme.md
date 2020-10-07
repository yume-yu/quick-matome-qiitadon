# Quick "Matome" For Qiitadon

## これはなに?
Qiitaが提供するマストドンインスタンス[Qiitadon](https://qiitadon.com)で、有志が作成したtootまとめ[mastogetter](https://github.com/Qithub-BOT/mastogetter)のまとめを簡単に作れるようにするTampermonkeyのユーザースクリプトです。

QiitadonのWebに画像の様なボタンが表示されるようになります。Web版のマルチカラム表示での利用を想定しています。

![スクリーンショット 2020-10-082 39 32](https://user-images.githubusercontent.com/30368684/95367269-85454180-090f-11eb-9875-d45d4279ba46.png)

## どうすれば使えるようになる?
1. まずはお使いのブラウザにブラウザ拡張 **Tampermonkey** をインストールしてください。インストール方法については公式ページ[tampermonkey.net](https://www.tampermonkey.net/)にブラウザごとに書いてあります。
2. [このリンク](https://github.com/yume-yu/quick-matome-qiitadon/raw/master/quick-matome-qiitadon.user.js)をクリックします。
3. Tampermonkeyのユーザースクリプトインストール画面が開くのでインストールを押してください。
4. Qiitadon.comを開いてみてください

## 使い方
1. まとめをつくりたいなと思ったら右下の"mt"ボタンを押します。"mt"ボタンが緑になっているときは、Toot記録モードです。
2. まとめに含めたいtootをクリックしましょう。クリックしたTootのidが裏で記録されていきます。
3. 必要なtootをクリックし終えたら、">"ボタンを押します。記録されていたTootを含んだmastogetterのリンクがコピーされています。
4. そのまま共有してもよし、[mastogetterの編集ページ](https://qithub-bot.github.io/mastogetter/)からインポートして編集するのもいいでしょう。

## ボタンの説明
* "mt" ボタン: 一番したのボタンです。クリックでモードが切り替わります。緑になっているときのみ、クリックしたtootのidを記録します。
* ">" ボタン: 真ん中の青いボタンです。クリックしたときに記録されていたidからmastogetterのリンクを作成します。もしブラウザがclipboardAPIに対応していないときは新しいタブでurlを開きます.
* 赤いボタン: 記録されているidをすべて消去します。連続してまとめを作るときは一度押すと良いかもしれません。

## 注意事項
1. このid記録にはlocalStorageを使っています。
2. Quick "Matome" For Qiitadon が作成するリンクは mastogetterが"互換性のために残している機能"を利用しています。そのため、mastogetterの変更に伴い機能しなくなることがあります。
3. 力技のtootid取得により、通知タブのtootのidが正常に取得できません。気が向いたら直します。
