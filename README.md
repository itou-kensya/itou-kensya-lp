# いとう建舎 LP

Meta広告用ランディングページ。`main` ブランチへの push でロリポップに自動デプロイされる。

## 構成

| ファイル | 役割 |
|---------|------|
| `index.html` | LP本体 |
| `reform-diagnosis.html` | リフォーム診断ツール |
| `images/` | LP使用画像 |
| `.github/workflows/deploy.yml` | GitHub Actions デプロイ設定 |

## 公開URL

- 本番: https://itou-kensya.com/lp/
- 診断ツール: https://itou-kensya.com/lp/reform-diagnosis.html

## デプロイ

`main` ブランチに push すると、GitHub Actions が自動でロリポップの公開ディレクトリへ同期する。

### 必要な GitHub Secrets

リポジトリ Settings → Secrets and variables → Actions から設定。

| Secret名 | 用途 |
|---------|-----|
| `FTP_SERVER` | デプロイ先サーバーホスト |
| `FTP_USERNAME` | FTP アカウント |
| `FTP_PASSWORD` | FTP パスワード |

### 手動デプロイ

GitHub の Actions タブから `Deploy LP to Lolipop` ワークフローを `Run workflow` で手動実行可能。

## サーバー情報

ホスティング・アカウント情報など機密情報は社内ドキュメントを参照（公開リポジトリに含めない）。
