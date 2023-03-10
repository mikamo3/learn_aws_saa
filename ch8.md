# データベース

## データベースサービス
以下がある

* RDS リレーショナルDB
* DynamoDB NoSQL
* Redshift データウェアハウス
* ElastiCache インメモリキャッシュ

## 8-2 RDS

* Oracle SQLServer MySQL PostgreSQLが選択可能
* AZレベルでの冗長化、リードレプリカ作成可能
* パッチ適用、アップグレードはGUIからできる
* ポイントタイムインリカバリで５分前などに戻せる
* インスタンスタイプ選択でスケールアップが可能

### ユースケース

一般的なリレーショナルDBとして

### リードレプリカ

マスタから同期された読み込み専用DB

読み込み負荷軽減

### Aurora

* Amazon謹製DBサービス
* MySql、PostgreSQLデータベースエンジン選択可能
* ストレージが自動拡張する
* 3AZに２つ合計Hつのデータコピー作成可能
* リードレプリカがあれば１分程度でフェイルオーバー可能
* ゼロダウンタイムパッチ

### 注意点

* オートスケールしない
* スケールアップ時はダウンタイムあり

## 8-3 DynamoDB

* Amazon謹製
* トランザクション処理は試験的にサポートされている
* 事前にリソース確保はしなくていい
* KVSとしてはコスパよし

* ハイスケーラブル、低レイテンシ
* 高可用性
* 容量制限なし
* 運用管理が楽
* スループットキャパシティ

### スループットキャパシティ

書き込み、読み込みに必要な分だけのスループットを割り当てる

キャパシティユニット単位で課金される

### ユースケース

* KVS
* ログDB
* モバイルアプリのバックエンド
* バッチ処理の状態管理
* メタデータストア

## 8-4 ElastiCache

フルマネージドなインメモリデータストアサービス

* Redis,Memcachedがつかえる
* AZれべるでのじょうちょうかやリードレプリカが作成可能
* バックアップ、リストア可能

### ユースケース

* セッション管理
* DBキャッシュ
* ストリームデータ分析
* メタデータストア

## 8-5 Redshift

フルマネージドなデータウェアハウス

* Postgresベース
* ペタバイト級までスケールアウト
* ただし手動で調整
* カラム型データベース


