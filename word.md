# 知らない単語

* AWS Elemental MediaConvert
  * 画像動画音楽を変換する？
* AWS Data Pipeline
  * AWSサービス間のデータ転送や変換に使われる
  * データ駆動形のタスクを作成できる
* Amazon Kinesis Data Streams
  * ストリームデータの処理に利用する
* Kinesis Data Firehose
  * ストリームデータを変換したり、ストレージなどに配信するサービス
* RedShift Spectrum
  * S3バケットに対して直接データ解析を実行可能
AWS CodePipeline
  * CodeDeploy,ECSなどをパイプラインとして設定して開発からデプロイを自動化する
* Amazon ECR
  * DockerImageリポジトリ
* 
NLB
* CloudFront

* EFS
  * Amazon Elastic File System
  * NFSみたいなやつ
* ChangeMessageVisibility API
  * SQSの可視性タイムアウトを設定して重複処理をなくす
AddPermissionAPI
CreateQueueAPI
ReceiveMessageAPI
Amazon Data Lifecycle Manager
Amazon DLM
* AWS ストレージゲートウェイ
  * iSCSI
AWS Organizations
* Glacier Deep Archive
  * めったにアクセスされない用

* Glacier Instant Retrieval
  * データ取得時は数分でアクセス可能
  * 4半期に1回程度の頻度を想定
* AWS STS
  * ユーザに一時的なアクセス許可を与える
AWS Config
* AWS Shield Advanced
  * DDos攻撃によって生じた可能性のある請求を保護する
Amazon GuardDuty
* AWS Shield Standard
  * DDOS攻撃の防御
Amazon SQSキュー
Amazon Kinesis Data Firehose
* AWS Secrets Manager
  * データベースやその他サービスの認証情報を安全に暗号化してシークレットとして保存、取得する
* AWS Systems Manager OpsCenter
  * AWSで利用しているインフラの可視化、制御 
* AWS Secrets Manager Parameter Store
  * 存在しない
* Snowball edge
  * セキュリティを考慮されたペタバイト規模のデータ転送手段
  * 物理的に搬送する
  * Computeで40TB
  * Storageで80TB
* Direct Connect
  * 物理的な専用線が必要
AWS Certificate Manager（ACM）
* Amazon EventBridge
  * サービスを自動化して、アプリケーションの可用化の問題やリソースの変更のシステムイベントに応答する機能
* Amazon SNS
  * プッシュ型のメッセジングサービス
* Amazon SES
  * Eメール機能,メール通知
Amazon StepFunctins
Amazon Glacier Flexible Retrieval
* ALB
  * Application Load Balancer
* CloudFormation
  * テンプレートに基づきAWSインフラ構成をデプロイする
* Amason SNS
  * プッシュ型のメッセージングサービス
* Amazon Cognito
CloudHSM
Lustreクライアント
Amazon FSx for Lustre
* Amazon DLM
  * Amazon Data Lifecycle Manager EBSのデータを定期的にバックアップする
* Amazon EMR
  * マネージド型Hadoopフレームワーク
* DynamoDB Accelerator(DAX)
  * キャッシュを利用した特定のデータへの処理が高い場合、中長期的な性能向上が見込める
  * 需要変動に応じたパフォーマンス向上には不適切
* Route Origin Authorization(ROA)
  * RIRを介して作成されるドキュメント。これでパブリックにルーティング可能なIPのアドレス範囲をAWSアカウントに移行できる
CloudTrail Insight
* AWS Transit Gateway
  * マルチキャストに対応
* Amazon Athena
  * S3内のデータを直接かんたんに分析できるクエリサービス
* Amazon Kinesis Data Analytics
  * IoTストリーミングデータのリアルタイム分析可能なアプリを構築
* NLB
  * Network Load Balancer
* Amazon EKS
  * Amazon Elastic Kubernetes Service
RekognitionAPI
Amazon Inspector
* AWS AppSync
  * DynamoDBのデータをリアルタイムでさいしんのものを取得できる？
Amazon FSx for Windows
AWS Managed Active Directory
* SWF
  * レガシーなワークフロー
AWS DMS
AWS ADS
AWS MGN

AWS DataSync
* ENI
  * Elastic Network Interface
  * VPCの論理ネットワークコンポーネント
* WLM
  * Workload Management
  * Redshiftのクエリ処理に対して割り当てるRedshuftのリソースを指定する

* Amazon Polly
  * 文章を音声変換
* Amazon SageMaker
  * 機械学習モデルのワークフロー
* Amazon Lex
  * 音声認識
* AWS application Discovery Service
  * オンプレのサーバにエージェントをインストールすることでデータセンターの利用状況を収集することができる
* Amazon QuickSight
  * クラウド型BIツール
* Amazon WorkSpaces
  * マネージドでセキュアな仮想デスクトップ環境
* AWS Outposts
  * RDSをオンプレミス環境にセットアップできる