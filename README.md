# ヨブトヤル

ユーザー同士でビデオ通話を繋げて、リアルタイムに一緒に黙々と作業会や勉強をするためのアプリです。

## :question: なぜ作ったのか

家で一人で勉強や作業をしていて、なかなか集中が出来なかったり、やる気が沸かない日ってどうしてもありますよね。
そんな時はカフェや図書館に行ったり、あるいは友人と動画を繋げて一緒に作業会をしたりしていました。
しかし、コロナの影響で外出が出来なくなり、また毎回友人に付き合ってもらうのもいたたまれなく、同じ悩みを持つ者同士で集まって、交流するわけでもなく黙々と一緒に作業ができたらいいのに…！と思い、このアプリを作成しました。

## :globe_with_meridians: URL
https://taskwith.herokuapp.com/

## :eyes: DEMO
〜gifが画像載せる〜

## :wrench: 使用技術(開発環境)
# フロントエンド
* Haml
* Sass
* JavaScript

# バックエンド
* Ruby 2.5.1
* Rails 5.2.4.3

# Web API
* SkyWay API
* webRTC

# インフラストラクチャー
* Mysql
* Heroku

## 工夫したポイント
ユーザーがビデオ通話にjoinするとSkyWayからユーザーを識別するためのにPeer IDというIDが与えられます。接続の度に新規に発行されてしまうのですが、このIDをアプリケーションのユーザー情報と紐付けて保存し、管理出来るようにしました。
そうすることで各ユーザーのjoin時間を測定することができ、累計時間をDBで保存出来るようにした点。

## 課題や今後実装したい機能

