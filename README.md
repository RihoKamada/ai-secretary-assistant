# AI Secretary Assistant 🤖📋

AI Secretary Assistant は、Googleカレンダー・Gmail・LINEを活用し、予定の要約・メール対応・通知を自動化する AI アシスタントです。

---

## ✨ 主な機能

- 📆 **Googleカレンダーの予定取得・要約**
- 📧 **Gmailの受信メール要約・返信文の自動生成**
- 💬 **LINE Messaging API によるプッシュ通知**
- 🗂 **Google Sheets を使った顧客対応履歴の管理**
- 📄 **PDFドキュメントに対する質問応答（RAG構成）**

---

## 🔧 技術スタック

- Python 3.x
- OpenAI GPT API（ChatGPT）
- Google API（Calendar / Gmail / Docs / Sheets）
- LINE Messaging API
- LangChain / FAISS / PyPDF2 / dotenv
- Flask または FastAPI（※今後追加予定）

---

## 🛠 セットアップ手順

1. プロジェクトディレクトリ直下に `.env` ファイルを作成し、以下を記述します：

OPENAI_API_KEY=sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxx

go
コピーする
編集する

2. 必要なパッケージをインストール：

```bash
pip install -r requirements.txt
FAISSインデックスを初回のみ構築（PDF読み込み処理）：

bash
コピーする
編集する
python pdf_qa_setup.py
🧪 使い方
ターミナルでプロジェクトのディレクトリに移動：

bash
コピーする
編集する
cd temp-ai-secretary
PDF質問応答システムを起動：

bash
コピーする
編集する
python pdf_qa.py
実行後に質問を入力：

text
コピーする
編集する
📦 FAISSインデックスを読み込んでいます...
❓ 質問を入力してください：
> この制度の目的は？

💬 回答：この制度の目的は、意思決定の透明性や公正性を確保し、行政処分の適正性を促進することを目的としています。
📂 ディレクトリ構成（例）
bash
コピーする
編集する
temp-ai-secretary/
├── pdf_qa.py                # 質問応答のメインファイル
├── pdf_qa_setup.py          # PDF読み込み・ベクトル化
├── pdf_reader.py            # PDF → テキスト変換処理
├── samplePDF.pdf            # 使用するPDFサンプル
├── .env                     # APIキーなど（※.gitignore推奨）
├── credentials.json         # Google API認証ファイル（※.gitignore推奨）
├── requirements.txt
└── README.md
🚀 今後の開発予定
Slackとの連携による通知受信・返信機能

NotionやGoogle Docsへの自動議事録転送

LINE Botからの会話型応答

音声入力対応

🙋‍♀️ 開発者
Riho Kamada（@riho_dev）

フリーランス / AI × 自動化ツール開発学習中

お問い合わせ・ご相談は GitHub Issues まで📮

📝 ライセンス
MIT License
