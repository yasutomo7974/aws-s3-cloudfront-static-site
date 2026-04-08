# S3 + CloudFront 静的サイトホスティング

## 概要
Amazon S3 と CloudFront を使用した静的ウェブサイトのホスティング構成です。

## アーキテクチャ
![構成図](img/aws-s3-cloudfront2.png)

## 使用サービス
- Amazon S3（静的ファイルの保存）
- Amazon CloudFront（CDN・HTTPS対応）
- Amazon Route 53（独自ドメイン設定）

## 構成のポイント
- S3バケットへの直接アクセスを禁止し、CloudFront経由のみ許可
- HTTPS対応済み
- CloudFrontのキャッシュ設定によりパフォーマンス最適化

## 実装したサイト
https://swell-webworks.com
