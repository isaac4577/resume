# 職務経歴書

## 基本情報

| 項目 | 内容 |
|------|------|
| 氏名 | 石原 拓海（Ishihara Takumi） |
| 生年月日 | 1996/11/20 |
| 最終学歴 | 国立熊本高等専門学校 制御情報システム工学科 卒業 |
| 居住地 | 熊本 |
| 性別 | 男性 |

## 自己PR

インフラエンジニアとして、AWS を中心とした IaC・CI/CD 整備、運用・監視改善を軸に経験を積んできました。  
新規システムの 0→1 構築を得意とし、既存インフラのクラウドネイティブへの段階的移行も経験しています。

フリーランス期間を通じて、顧客企業の IT 部門との調整・折衝を多く担当してきました。  
インフラ担当として参加しながらも、緊急時にはバックエンド・フロントエンドにも積極的に踏み込んでプルリクエストを上げるなど、役割を固定せずシステム全体を見渡して動くのが自分のスタイルです。

技術的な問題解決だけでなく、チームの中で"何でも相談しやすい人"であることを常に意識しています。

座右の銘は「仕組みを憎んで、人を憎まず。」  
新卒の時に当時の事業部長が仰っていた言葉で、以来、問題が起きた時はいつも仕組みに疑問を持つよう心掛けています。

---

## 職歴サマリ

| 期間 | 案件・所属 | 雇用形態 | 役割 |
|------|------|------|------|
| 2026/01〜現在 | 商社向け週報AIシステム | 業務委託 | インフラエンジニア |
| 2025/04〜2025/09 | 自動運転SDK開発プロジェクトの社内CI/CD基盤 | 業務委託 | インフラエンジニア |
| 2023/07〜2024/10 | 飲食チェーン メンバーシップサイト | 業務委託 | インフラエンジニア |
| 2022/06〜2023/06 | 行政サービス | 業務委託 | インフラエンジニア |
| 2022/03〜2022/06 | 電子契約SaaS | 業務委託 | インフラエンジニア |
| 2022/02〜2022/05 | リーガルテックSaaS企業 | 正社員→業務委託 | SRE |
| 2020/04〜2022/01 | Webアプリ開発会社 | 正社員 | インフラエンジニア |
| 2017/04〜2019/08 | ロボットSIer | 正社員 | 制御エンジニア |

---

## 職務経歴（詳細）

### 1. 商社向け週報AIシステム

| 期間 | 雇用形態 | チーム | フェーズ |
|------|------|------|------|
| 2026/01〜現在 | 業務委託 | 8名（インフラ担当: 自分のみ） | 設計 / 構築 / テスト / 運用 |

**サービス概要**
商社の海外駐在員から毎週送られる週報データをAIで解析・リスク分析し、チャットボット経由でこれらのデータを元に回答するシステム。コンサルティングから受託開発として発展した案件。

**担当業務**
- インフラ全般の設計・構築・運用（担当者1名）
- ECS / Fargate によるバックエンドホスティング
- Aurora PostgreSQL + pgvector を用いたベクトル検索基盤の構築
- CloudFront VPC Origins を用いた internal ALB への接続
- Bedrock / Bedrock Guardrails を用いた AI 基盤の構築
- k6 を用いたシナリオ負荷試験の実施・パフォーマンスチューニング

**使用技術**
- クラウド: AWS (ECS / Fargate / Aurora PostgreSQL / CloudFront / ALB / Bedrock / Bedrock Guardrails)
- 言語: Python, Terraform
- フレームワーク: FastAPI
- SaaS: GitHub

---

### 2. セルフホスティングCI/CD環境のドキュメント作成

| 期間 | 雇用形態 | チーム | フェーズ |
|------|------|------|------|
| 2025/04〜2025/09 | 業務委託 | 2名（メンバー） | 運用 |

**サービス概要**
自動運転用SDKの開発プロジェクトにおける社内CI/CD基盤のドキュメント整備。

**担当業務**
- 既存 Terraform コードを読み解き、セルフホスティング CI/CD 環境の Markdown ドキュメントを作成
- 独自シェルスクリプトでラップされた Terraform 構成の解析
- tfstate 管理用 S3 バケット自体を Terraform で管理するバッドプラクティスの把握・ドキュメント化

**使用技術**
- クラウド: AWS (ECS / EC2 / Lambda / S3)
- 言語: Terraform, Python
- SaaS: GitHub, GitHub Enterprise
- 作業OS: Windows (WSL)

---

### 3. 飲食チェーン店メンバーシップサイトのサーバ運用

| 期間 | 雇用形態 | チーム | フェーズ |
|------|------|------|------|
| 2023/07〜2024/10 | 業務委託 | 10名（メンバー） | 運用 |

**サービス概要**
飲食チェーン店向けメンバーシップサイトのインフラ運用・監視改善。

**担当業務**
- IaC 化されていないインフラの Terraform 化
- 監視改善（アラート改善 / ログ収集改善）

**使用技術**
- クラウド: AWS (ECS / EC2 / CloudWatch / Aurora / WAF / GuardDuty / Lambda / S3)
- 言語: Terraform, Python
- SaaS: GitHub
- ツール: Grafana, Prometheus
- 作業OS: macOS

---

### 4. 行政サービスのサーバ運用

| 期間 | 雇用形態 | チーム | フェーズ |
|------|------|------|------|
| 2022/06〜2023/06 | 業務委託 | 3名（メンバー） | 運用 |

**サービス概要**
行政サービスのインフラ運用・監視改善。

**担当業務**
- 監視改善（CloudWatch アラートの見直し・整理）
- CloudWatch Synthetics Canary による外形監視の導入

**使用技術**
- クラウド: AWS (ECS / EC2 / CloudWatch / Aurora / WAF / Lambda / S3 / CodePipeline / CodeCommit / CodeBuild)
- 言語: Terraform, Python
- 作業OS: Windows (WSL)

---

### 5. 電子契約関連自社プロダクトのインフラ構築

| 期間 | 雇用形態 | チーム | フェーズ |
|------|------|------|------|
| 2022/03〜2022/06 | 業務委託 | 6名（メンバー） | 設計 / 構築 |

**サービス概要**
電子契約関連の自社プロダクトにおけるインフラ設計・構築。

**担当業務**
- 環境別インフラ（dev / stg / prd）の設計・構築
- CI/CD の整備
- 開発者向け Docker Compose 環境の整備

**使用技術**
- クラウド: AWS (ECS / Fargate / RDS / CloudWatch / WAF / S3 / SSO / Control Tower / Organizations), Azure AD
- 言語: Terraform
- SaaS: GitHub, GitHub Actions

---

### 6. リーガルテックSaaSの会社でSRE

| 期間 | 雇用形態 |
|------|------|
| 2022/02〜2022/03（正社員）、〜2022/05頃（業務委託） | 正社員→業務委託 |

正社員として入社後、短期で離職。その後は業務委託として同社のSRE業務を継続支援。

**担当業務**
- Terraform コードのリファクタリング

**使用技術**
- クラウド: AWS (ECS / Fargate)
- 言語: Terraform
- SaaS: Datadog

---

### 7. Webアプリケーション会社（自社/受託）インフラ構築・運用

| 期間 | 雇用形態 | チーム | フェーズ |
|------|------|------|------|
| 2020/04〜2022/01 | 正社員 | 1〜3名（インフラ担当） | 設計 / 構築 / テスト / 運用 |

**サービス概要**
自社プロダクトと受託案件のインフラを一手に担当。EC2 ベースのインフラを ECS/Fargate に移行するなど、モダンなクラウドネイティブ構成へのシフトを推進。

**担当業務**
- インフラ全般の構築・運用・改善（ビジネスロジック以外全般を担当）
- Terraform 導入（IaC 化）
- CI/CD 整備（GitHub Actions）
- 負荷試験環境の構築（k6 / Locust / GoReplay）
- 監視基盤の構築（Prometheus / Grafana）
- ミドルウェアのチューニング（nginx / php-fpm）
- 開発者向けローカル開発環境の整備（Dockerfile / docker-compose.yml の作成・配布・サポート）
- 情シス的業務（社内ツール・環境整備）

**使用技術**
- クラウド: AWS (ECS / Fargate / EC2 / RDS / Aurora / CloudWatch / WAF / S3)
- 言語: Terraform, Python, PHP
- SaaS: GitHub, GitHub Actions

---

### 8. ロボットSIerで制御エンジニア

| 期間 | 雇用形態 |
|------|------|
| 2017/04〜2019/08 | 正社員 |

**サービス概要**
産業用ロボットを組み込んだ半導体生産設備（搬送設備）を自社設計・製造し、客先へ納品。

**担当業務**
制御ハードウェアを中心に、1案件を単独で完結させることも多く、以下を幅広く担当。
- 電気回路設計・ケーブル設計
- 計装設計
- 部品調達・外注管理（電気工事の外注・管理を含む）
- 動作試験
- ソフトウェア開発（PLC ラダー（三菱電機 MELSEC）によるシーケンス制御、HMI 改修（Visual Basic））
- 工程管理

**使用技術**
- 言語: Visual Basic, PLC ラダー（三菱電機 MELSEC）
- ツール: AutoCAD（電気・機械）

---

## スキルセット

### Cloud

**AWS**
EC2 / ECS / Fargate / ELB / S3 / CloudWatch / RDS / Aurora / API Gateway / Lambda / WAFv2 / EFS / WorkSpaces / DynamoDB / Route53 / VPC / VPC Peering / Amplify / EventBridge / CodePipeline / CodeBuild / CodeDeploy / SES / SNS / CloudFront / CloudFront VPC Origins / DMS / KMS / Transfer Family / Athena / Cognito / Copilot / Step Functions / Control Tower / Organizations / CloudFormation / SAM / ACM / IAM / SSO / GuardDuty / Bedrock / Bedrock Guardrails

**Azure**
Azure AD

---

### Infrastructure as Code

Terraform / Serverless Framework / Docker / Packer / sops

---

### VCS
GitHub / GitHub Enterprise / GitLab

---

### CI/CD

GitHub Actions / CircleCI / GitLab CI/CD

---

### Middleware

nginx / php-fpm / MySQL / PostgreSQL / pgvector

---

### Programming Language

C / C++ / C# / Java / PHP / Ruby / Python / JavaScript (Node.js) / Visual Basic

---

### Framework

Laravel / Ruby on Rails / ASP.NET / FastAPI

---

### Monitoring

Prometheus / Grafana / Datadog

---

### Load Testing

k6 / Locust / GoReplay

---

### CAD

AutoCAD (Electrical / Mechanical)
