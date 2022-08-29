# slack-api-file1

## NodeJSとSlack APIによるいまどきのネットワークプログラミング

### ファイルを操作する その1

Node.jsのファイル書き込み機能を用いて新型コロナウィルス感染者数の履歴データをCSVファイルとして保存するプログラムの動作を確認する。

[動作確認の手順]

1. コマンドプロンプトを開き、ダウンロードしたフォルダへ移動する
1. npm installコマンドでアプリに依存するパッケージをインストールする
1. .envファイルの環境変数SLACK_BOT_TOKEN、SLACK_APP_TOKEN、DB_URLが正しく設定されているか確認する
1. アプリを起動する
    $ node ./app.js
1. Slackアプリをインストールしたチャネルのメッセージ欄に「/covid19」と入力し、送信する
1. 選択メニューから適当な国を選ぶ
1. 感染状況の下に[CSV出力]ボタンが配置されていることを確認する
1. このボタンをクリックすると_tempフォルダにCSVファイルが作成される
1. テキストエディタでファイルを開き、内容を確認する
