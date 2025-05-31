# AI Secretary Assistant 🤖📋

AI Secretary Assistant は、Googleカレンダー・Gmail・LINEを活用し、予定の要約・メール対応・通知を自動化するAIアシスタントです。

## ✨ 機能

- 📆 Googleカレンダーの予定取得・要約
- 📧 Gmailの受信メール要約・返信文自動生成
- 💬 LINE Messaging APIを通じたプッシュ通知
- 🗂 顧客対応履歴の管理（Google Sheetsと連携）

## 🔧 技術スタック

- Python 3.x
- OpenAI GPT API
- Google API (Calendar, Gmail, Docs, Sheets)
- LINE Messaging API
- Flask / FastAPI（※今後追加予定）

## 🛠 セットアップ方法

1. `.env` に必要なAPIキー・シークレットを設定
2. `pip install -r requirements.txt`
3. 各モジュールを個別に実行 or スケジューラと連携して実行

## 📸 スクリーンショット
<img width="1050" alt="操作確認画面" src="https://github.com/user-attachments/assets/f7b2a832-af8f-4edf-8e71-a1e149c67418" />

![AI秘書スクリーンショット]操作確認画面


## 🚀 今後の開発予定

- Slackとの連携
- より自然な会話型応答の導入
- Notionへの議事録転送

---

## 📂 ディレクトリ構成（例）

temp-ai-secretary/
├── main.py
├── gmail_summary.py
├── calendar_summary.py
├── line_push.py
├── token.json
├── credentials.json（※.gitignore推奨）
├── README.md

yaml
コピーする
編集する

---

## 🙋‍♀️ 開発者

Riho Kamada（[@riho_dev](https://github.com/RihoKamada)）

---

## 📝 ライセンス

MIT License# AI Secretary Assistant
