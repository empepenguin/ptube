# ptube
# servicemap
<img src="blob:https://whimsical.co/626e5153-bf82-4661-8d8e-d1695401b791" alt="エビフライトライアングル" title="サンプル">

# サービスの説明および機能

## kahocliantサービス
- 各ページのデザイン作成
- ホーム画面

## akane-apiサービス
- 各サービスにapi-serviceを生やす

## akane-authサービス
- ユーザー登録
- ユーザー認証

## akane-postgres-authサービス
- ユーザー情報の保存

## akane-streamingサービス
- 動画再生

## akane-usersサービス
- 動画投稿者のusernameをakane-postgres-authから取得
- streamingとakane-postgres-authのやり取りの中間役

## akane-postgres-streamingサービス
- 動画の保存

## akane-convertサービス
- mp4ファイルをHSLm3u8+ts)形式に変換

## minioサービス
- 動画ファイルの保存する
