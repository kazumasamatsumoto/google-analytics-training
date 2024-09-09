# google-analytics-training

参考動画
https://www.youtube.com/watch?v=cpZMDkZ2mGA

タグマネージャーを使用

![image](https://github.com/user-attachments/assets/5992d07b-4b2c-4851-b22b-d688fe410448)

適当なログインが必要なページを用意

![image](https://github.com/user-attachments/assets/b9f9d767-bd30-46ab-8f82-4a2a4811b997)

ユーザーは一意のIDを保持していると仮定して、そのIDをGoogle　Analytiscに送信します。

コンソール画面でのサンプルコード（開発機能でのコンソール画面ではJavascriptが使用できます。

![image](https://github.com/user-attachments/assets/750ef445-03a4-4b5e-a8f5-fdc3369e89ae)

実際に送信されているかどうかはタグマネージャのプレビューの画面に移動します。

![image](https://github.com/user-attachments/assets/da98d57d-f494-4d31-bddc-aec08f0d7a0a)

そのあとにURLを貼り付けます。これは開発環境や本番環境などタグの設定が有効になっているか確認するページになります。

![image](https://github.com/user-attachments/assets/1a0833e4-8acb-4dce-b1b3-ea8de008eb1b)

ログインの挙動（つまりデータレイヤーの送信が完了したとき）

写真のようにサマリーとなってアクセスの流れが確認できます。

![image](https://github.com/user-attachments/assets/f3c26b18-9b7c-496c-ad5f-523a680065a9)

この動画ではloginの処理に対してAPIがCallされdataLayerがpushされている状態が判明できます

![image](https://github.com/user-attachments/assets/d1165ec9-95b5-47ee-87cb-ba0261407553)

注意点としてはタグにはメールアドレスやマイナンバーや社会保障番号などのような情報は秘匿するように作られています。

またuserIdはどのような形で宣言したとしてもuserIdという変数で受け取るためこの値をGA4で読み取れるように変換しなければいけません。

タグマネージャーではuserIdを呼び出しますが、その呼び出す定義はuserIdではなく違うものに区別できないといけません。

![image](https://github.com/user-attachments/assets/006da5a0-0503-4087-8d4b-739a6b57ebf4)

実際にuser_idとフィールドに設定して確認するととれます。

![image](https://github.com/user-attachments/assets/cf74136d-d2d0-40ed-b9f8-0acba1171d80)

デバックビューでも確認ができます。これがGA4に確実に送信されている状態になります。

![image](https://github.com/user-attachments/assets/5a6b2c9c-f292-468b-8d87-59f47c8f2b30)

ほかに分析などで使用する場合はカスタムディメンションを作成する必要がありますがユーザープロパティにuser_idなどは予約語として機能しているためべつの用語を定義する必要があります

![image](https://github.com/user-attachments/assets/8490205f-4cc1-4285-8f3a-cca063bf001b)

あとは24時間後
