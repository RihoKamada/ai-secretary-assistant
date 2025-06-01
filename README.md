# 📄 PDF QA System

PDF QA System は、PDF ファイルを読み込んで、自然言語での質問に対して的確に回答してくれる AI アシスタントです。LangChain + OpenAI + FAISS を活用し、PDF 文書をベクトル化して効率的に検索・応答を行います。

---

## ✨ 主な機能

- 📚 PDFファイルの読み込み
- 🔍 質問に対するベクトル検索 + GPT応答
- 🧠 長文PDFにも対応（MapReduce使用）
- 🧾 FAISSによる効率的な類似文書検索

---

## 🛠 セットアップ手順

1. `.env` ファイルを作成し、以下を記述します：

```env
OPENAI_API_KEY=sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxx
必要なパッケージをインストール：

bash
コピーする
編集する
pip install -r requirements.txt
FAISSインデックスの作成（初回のみ）：

bash
コピーする
編集する
python pdf_qa_setup.py
質問を実行：

bash
コピーする
編集する
python pdf_qa.py
🧪 使用例
bash
コピーする
編集する
❓ 質問を入力してください：この制度の目的は？

💬 回答：
この制度の目的は、意思決定の透明性や公正性を確保し、行政処分の適正性を促進することを目的としています。
📁 ディレクトリ構成
plaintext
コピーする
編集する
pdf-qa-system/
├── pdf_qa.py              # 質問処理ロジック
├── pdf_qa_setup.py        # FAISSインデックス作成用
├── pdf_reader.py          # PDFテキスト抽出
├── requirements.txt       # 必要パッケージ
├── samplePDF.pdf          # サンプルPDF
├── faiss_index/           # ベクトルデータ保存先
├── .env                   # OpenAIキーなど（git管理対象外）
└── README.md              # このファイル
🖼️ スクリーンショット
📌 実行画面の例



※画像リンクは GitHub 上に画像をアップロード後に、自動生成される URL に置き換えてください。

🙋‍♀️ 開発者
Riho Kamada
フリーランスAIプログラマー。業務効率化や自然言語処理を活用したアシスタント開発が得意です。
📩 Twitter: @riho_dev（例）

📝 ライセンス
MIT License
