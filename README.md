# ptube
# servicemap
![servicemap](https://github.com/empepenguin/ptube/blob/images/service-map.png)

# サービスの説明および機能

## kahocliantサービス
ここでは静的ファイルの配信を行っている.
ユーザが一番最初にアクセスする場所がここになる.

## akane-apiサービス
ほとんどのリクエストはakane-apiに来る.
そのリクエストを他のサービスに流す役割をもっている.

## akane-authサービス
akane-apiからユーザに関するリクエストが流れてきたら処理をする.
登録や認証などを担当するサービス.

## akane-postgres-auth
akane-authで処理されたデータを格納するDB

## akane-streamingサービス
akane-apiから動画に関するリクエストが流れきたら処理する.


## akane-postgres-streaming
ユーザーがあげた動画の情報を処理するサービス

## akane-convertサービス
mp4ファイルをHSLm3u8+ts形式に変換

## minioサービス
動画ファイルの保存する
