# 再実施で間違えたところ
* Autoscalingは24時間で停止
* Data Pipelineはサービス間のデータ転送や変換処理に利用される。
* Auroraレプリカは複数AZに展開してプライマリDBの障害似空得られる
* Lambdaファンクションに付与するのはIAMロール
* スループットHDD
* DynamoDBのオンデマンドは前に到達したトラフィックっレベルまで拡張、縮小する.利用不可が予測できない時
* Amazon SNSはプッシュ通知をトリガにジョブを実行する。並列実施でスケーリングはできない
* DynamoDBトランザクション機能で書き込み時に機密データを削除できる
* DatahoseはDBには保存できない
* AWS Secrets Managerはサービスの認証情報を暗号化して保存、取得する仕組みを提供
* インスタンス間のトラフィック制御はセキュリティグループを使う。ルールにはグループIDを使う
* LambdaのHTTPアクセスは関数URLをパブリックにすることでも可能
* Amazon GuardDutyはDDosいがいの不正アクセスの自動検知
* S3はインターフェースエンドポイントに対応している
* 処理停止イベントは直接lambdaでうけとれない
* AmazonDLMにてEBSのスナップショットの定期取得スケジュールを行う
* 1つのクロスリージョンレプリケーションだけでは双方向のレプリケーションは実現できない
* Kinesis Data Analyticsは直接S3などに配信できるのでDatahoseはいらない
* VPCのDNS hostnamesオプションを有効にしないとインスタンスがDNS解決できない
* 時間トリガーでDatapipelineをうごかすなどできる
* NLBはL4LB
* ADを連携してAWSにログインするにはAWS Single-Signonをつかう
* APIGatewayはlambdaだけでなくKinesisとも連携できる
* Cloud Trailは主にコンプラ用。
* VPCフローログでトラフィックモニタリングできる
* 異なるAWSアカウントのリソースへのアクセスを委任するにはクロスアカウントアクセス許可とIAMロールを設定する
* DynamoDBストリームはあるがいべんとはない
* ECSはAWS独自Docker
* AWS OrganizationsはADとは関係ない
* S3パブリック・アクセスを有効化するという項目はない
* AWS WAFによりトラフィック制御、SQLインジェクションなど防げる
* LambdaからRDSのアクセスはSecuritGroupIngressによりセキュリティグループを許可する
* EFSは特定のAZにげんていせずにVPCに配置できる
* Kinesis Data Streamsは重複、到着順保証
* S3 OAIをわりあててそのOAIのみがアクセスできるようにできる。OACも同様だが違いはすべてのリージョン対応、暗号化、S３への動的リクエスト可能
* Kinesis Data Streamsはストリーム用。画像などの取り扱いは不向き
* Auroraは基本AZやGlobalに関する設定は不要
* アプリケーション層にLambdaは不向き
* RDSはAZ配置にしてもセカンダリをアクティブにできない
* CloudFormmationスタックセットは複数のAWSアカウント、リージョンにリソース展開できる
* IAMロールをADユーザに割り当てる
* RedshuftのWLMをクエリ処理に対して割り当ててリソースを指定する