# iOSコーディング能力テスト

Swiftを使います、次のテストを完了します。

### 1
**UITableView**または**UICollectionView**を使用してリスト画面を作成します。
リスト画面の構造は以下のイメジを参考して下さい。（同じことをする必要はありません）
リスト画面は複数の部分に分割する必要があり、各コンテンツには画像、テキストが必要です。
<p align="center"><img width="300" src="https://user-images.githubusercontent.com/92193175/150973935-dcea7351-20fa-4cfe-b6a8-b0809f0a2717.jpeg"></p>

### 2

今ログインAPIがあります。ログインAPI情報は以下を参考して下さい。

APIパース: https://devapi.scanat.app/auth/login

Request方法: POST

Content-Type: application/json

パラメータ:
以下のメールアドレスとパスウードは使うことができます。
```
{
	"email":"zyfoolboy@icloud.com",
	"password":"Aa123123111"
}
```
Response:
ログイン成功の場合：
```
{
    "code": 200,
    "message": "操作成功",
    "data": {
        "access_token": ".....",
        "token_type": "bearer",
        "refresh_token": ".....",
        "expires_in": 86399,
        "scope": "read",
        "jti": "...."
    }
}
```
ログイン失敗の場合：
```
{
    "code": 401,
    "message": "....",
    "data": null
}
```

#### 要求

ログイン画面を作ります。

ログイン画面の内容：

メールアドレス入力ボックス，パスウード入力ボックス、ログインボタンがあります。

ログインAPIを使う、メールアドレスとパスウードを入力し、メールアドレスとパスウードが正しい場合、ログインボタンを押す、**ログインしました**メッセージに画面を表示します、メールアドレスとパスウードが間違い場合、ログインボタンを押す、**ログイン失敗しました**メッセージに画面を表示します。

### 3
 **1**と**2**のソースはこのリポジトリで新しいブランチを格納します。

