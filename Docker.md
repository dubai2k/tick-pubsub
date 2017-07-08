# Docker

## Dockerを使用しない運用例
### 開発

- 稼働環境を構築
- 手順書などの資料作成
### 運用
- 運用手順書作成
- 手順書に従いリハーサル
- 手順書に従い本番環境へ

    台数が多く、自動化しても時間がかかる

## Docker
### 開発
- Dockerfile作成
- DockerImage作成
### 運用
- リハーサル
    DockerImageからConainer起動
- 本番環境
    DockerImageからConainer起動

    Container起動は日々のプロセス再立ち上げと同等
