# README

## 環境構築
```
$ bundle install --without=production
$ bin/rails db:setup
$ yarn install
$ bin/webpack
$ bin/rails s
```

## 事業をエンジニアリングしよう提案編の回答は以下に記述してください
## 選択した事業側の課題
サービス登録者数の内、男性60%に対して、女性は40%。一方で、サービス内のもくもく会に参加した人の比率は、男性90%：女性10%と大きな差が出ています。もっと女性が使いやすいようなサービス設計にする必要があるのではないか？

## 提案内容
男女別にもくもく会を開催できるように設定し、絞り込みができるようにする。
→もくもく会に参加した人の比率が男性90%という状況なので、女性にとっては男性が多い会に参加しずらく、選択肢が男性が多い会ばかりになってしまう。そのため、女性が参加しやすいように男女に分ける機能をつける。

## 実装方針
・ユーザー登録の際に、性別を選択できるようにセレクトボックスをつける。
・もくもく会作成ページの性別項目にセレクトボックスを作成し、男女別に設定できるようにする。
・もくもく会一覧画面にて、「女性専用イベント」という絞り込み機能をつける。