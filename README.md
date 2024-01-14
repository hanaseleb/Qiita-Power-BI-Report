# Qiita-Power-BI-Report

![image](https://github.com/hanaseleb/Qiita-Power-BI-Report/assets/8947320/721b5b8f-47ea-4c5e-aa0d-b937549aa1ec)

# 利用条件

利用する方は、以下のQiita記事にいいねをしてください😊

https://qiita.com/akihiro_suto/items/92a787c4b41d210bab57

# 使い方

## Qiita アクセストークンの取得

**設定→アプリケーション→個人用アクセストークン**

**新しくトークンを発行**

![image.png](https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/80467/813bc744-2c13-5bf0-b559-5ee391c7374f.png)

トークン名は任意です。管理しやすい名前をつけましょう。
今回はread権限だけあれば十分です。

![image.png](https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/80467/774298ee-31fe-18e5-2d31-799b10878150.png)

発行した後のトークンは、コピーして安全に保存しておいてください。トークンはこの画面に一度表示された後は、再度表示はできない仕様になっています。

![image.png](https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/80467/25099152-c0d9-bfc5-8c59-fced9b1cf3fe.png)

## Power BI テンプレートのDL

以下URLよりPower BI テンプレートをDLしてください。

**※利用条件 本記事に「いいね」すること😊**

https://github.com/hanaseleb/Qiita-Power-BI-Report/releases/latest

Power BI テンプレートをDLしたら、ダブルクリックして開きます。

開くと、パラメーターの入力画面になります。

 **page_num** には **1** を入力してください。

**your_token** には 先ほど取得したQiitaのトークンを貼り付けます。

![image.png](https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/80467/249767c3-2644-162e-e662-bdcca5919025.png)

入力をしたら、**読み込み** を押せば完成です。

プライバシーレベルを求められる場合、データソースがQiita APIのみなので今回は「Public」で問題ないでしょう。

プライバシーレベルについては以下ドキュメントを参考にしてください。

https://learn.microsoft.com/ja-jp/power-bi/enterprise/desktop-privacy-levels

## 完成

これだけの手順で完成です。順調にいけば3分くらい！
レポートのデザインやデータモデルはシンプルなものなので、あとはご自身で改良して使用してください。

![image.png](https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/80467/b97e8fd1-fba2-f666-6f8f-fcea598b4a92.png)

# Power BI Serviceへ発行

レポートを作成したら、Webに発行して自動更新したいですよね。

発行しても、すぐに自動更新を有効にはできません。

セマンティックモデルの設定画面から、データソースの資格情報を編集しましょう。

![image.png](https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/80467/2e7286d6-77cc-2ce0-c535-0c5d8ec7f900.png)

ここで、認証は**匿名**、プライバシーレベルは再度**Public**を選択します。

![image.png](https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/80467/6268a888-e4f9-acba-5a76-dda2436336b4.png)

ここまでやると、自動更新を設定することができますので、任意の時間に設定しましょう。

![image.png](https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/80467/7d12510d-c8db-099b-9db1-3572e7b7c315.png)

