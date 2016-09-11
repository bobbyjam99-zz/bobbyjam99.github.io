# Serverless Architecture

## Serverless Architectureとは

AWS Lambda
GCPのCloud Functions
Azure Functions
ユースケース
素早く届ける
即時処理
バックエンド構築
エコシステム
いくつかのユースケースが紹介されました。

ユースケース1 : データ処理

S3 のバケットトリガーとか DynamoDB のストリームをイベントトリガにする
膨大なスケールで実行されるが、Lambda 使うと気にしなくて良い
S3 のドキュメントのインデックスを作ったりするようなことはすぐできる
ユースケース2 : スケーラブルなバックエンド

AWS Mobile SDK を使ったモバイルアプリ、または IoT デバイス
Lambda のブループリントから作り始める (バックエンド用のブループリントがある)
データストレージは DynamoDB (RDS とかでもOK)
ユースケース3 : サーバーレスウェブアプリ

静的コンテンツは S3
動的コンテンツは Lambda
HTTP アクセスは APIGatway
データストレージは DynamoDB
CloudFront をオプションで使うと CDN もできる
ユースケース4 : 新しいアプリケーションエコシステム

Alexa Skill + Slack = サーバーレスボット！
音声を聞き、Slack のチャンネルにメッセージを送ることが可能

## 参考資料

* [レポート] サーバーレスで構築する、マイクロサービスの未来形 AWSSummit http://dev.classmethod.jp/cloud/aws/aws-summit-tokyo-2016-devcon-ha1420/
