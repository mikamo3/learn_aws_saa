# セキュアな複数改装アプリケーション

## 9-1 セキュアな複数改装アプリケーション

### 複数回操作s部ネット

AWSではサブネットでパブリックサブネット、プライベートサブネットを作成して複数改装を持つサブネット構成にするのが一般的

## 9-2 階層パターン

### 1階層サブネット

パブリックサブネット1つの構成

* シンプル
* すべてのサーバはネットワーク的にインターネットからアクセス可能
* セキュリティグループでアクセス制限は可能だが設定誤りに注意

### 2階層サブネット

たとえばweb/DBの2階層

DBをプライベートサブネットに配置するのでインターネットから参照できない

### 3階層サブネット

パブリックサブネット: ELB,Bastion(踏み台)
プライベートサブネットA：web
プライベートサブネットB：DB

みたいな構成

よりセキュア

ELBはロードバランサ

## 9-3 セキュリティ面でのメリット

### パブリックサブネット、プライベートサブネット

セキュリティに柔軟なネットワーク構成を作成できる

### NATゲートウェイ

インターネットにアクセスできるサブネットが必要な場合に使う

インターネットからはアクセスできない

### VPCエンドポイント

S3,DnamoDBなどのAWSリソースを扱うときにAWSネットワークを経由してセキュアにアクセスできる

VPN、VPCエンドポイントとプロキシサーバーを組み合わせてオンプレからセキュアにアクセスできる

### 踏み台(bastion)

パブリックサブネットに配置してSSH経由などでプライベートサブネットにアクセスする

### VPN/Direct Connect

踏み台の脆弱性やセキュリティグループの設定のミスによるインシデントを気にしなくていい

### セキュリティグループの絞り方

IPベースではなくセキュリティグループIDベースでの制御も可能


