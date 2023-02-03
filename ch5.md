# 5-1 仮想ネットワーク

## VPC

Virtual Private Cloud

AWS上にプライベートネットワークを構築する

つかわないときほんES2はすべてDMZに配置

サブネットはアベイラビリティゾーンをまたいで作成できないので1つのVPCないでアベイラビリティゾーンごとにサブネットを作る

社内ネットワークと接続する可能性があるときはIPが重複しないように

/28プレフィックス長以上を推奨

ELB/ALB/NLBを配置するときはサブネットに余裕をもたせる

IPを確保できないとスケールアウトできないため

## ルートテーブル

= linuxのroute

## パブリックサブネットとプライベートサブネット

パブリックサブネットにはVPCにインターネットへ出るためのGWがあタッチされる

プライベートにはそれがない

プライベートでインターネットにアクセスしたい場合はNATGatewayなどつかう

## NATゲートウェイ

プライベートサブネットを構築してインターネットへなにか通信したい場合などにつかう

アベイラビリティゾーンごとに1津配置する必要がある

インターネット側からNATゲートウェイにあくせすはできない

インターネット側からプライベートサブネットにアクセスしたい場合は踏み台構成にする

## VPCエンドポイント

AWSの一部のサービスでプライベート通信が可能

## Elastic IP

パブリックIPはインスタンス起動ごとにランダムで割り振られる

ElasticIPを利用おするには固定のグローバルIPを確保する

EC2インスタンスからインターネットに出る場合、いずれかのIPがヘッダに付与される

インスタンスごとにIPを付与すると手間になるためNATゲートウェイに割り振って集約することもできる