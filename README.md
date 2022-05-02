# webpack-crash-course
セクション4-12 sass-loader　ブランチはsass-loader
node-sassのバージョンが動画通りだとエラーになってしまい、
最新版@7.0...をインストールして
sassファイルを編集　→　index.jsを編集　import './style.scss'
→　ブラウザで確認時にエラーが出た
Uncaught Error: Module build failed (from ./node_modules/sass-loader/lib/loader.js):
Error: Node Sass version 7.0.1 is incompatible with ^4.0.0.

node-sassのバージョンを動画のバージョンではなく
4.0.0にしようとしたが、エラー

npmのサイトでnode-sassを確認　→　node.jsのバージョンが16の時は6.0だった
→　npm run start　→　またエラー
Error: Node Sass version 6.0.0 is incompatible with ^4.0.0.

どうやら4.0.0でないとダメみたい
ということはnode.jsのバージョンを14くらいに下げればよさそう
node.js14でもダメでした
