# ptube
# servicemap
![servicemap](servicemap.jpg)

# サービスの説明および機能

## kahocliantサービス
- 各ページのデザイン作成

## akane-apiサービス
- 各サービスにapi-serviceを生やす
- 各サービスでapiをたたけるようにする
- cliantと各サービス間がやり取りできるようにする

## akane-authサービス
- ユーザー登録できるようにする
- ログイン時にユーザー認証を行いcliantにユーザー情報を返す

## akane-postgres-authサービス
- ユーザー情報の保存する機能
- akane-authやstreamingに必要な情報を返す機能

## akane-streamingサービス
- 動画再生をできるようにする機能
- 動画のタイトル表示機能

## akane-usersサービス
- 動画投稿者のusernameをakane-postgres-authから取得
- streamingとakane-postgres-authのやり取りの中間役

## akane-postgres-streamingサービス
- ユーザーがあげた動画を保存する機能

## akane-convertサービス
- mp4ファイルをHSLm3u8+ts)形式に変換

## minioサービス
- 動画ファイルの保存する
