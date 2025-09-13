# toyooka-ai-learning
AIツールを使ってプロダクトを開発するためのレポジトリです。  
ここでは **v0**, **Vercel**, **Supabase**, **GitHub**, そしてローカル環境での **VS Code** を利用したアプリケーション開発方法を紹介します。

---

## 🛠️ 使用するツール

### [v0](https://v0.dev/)
- Vercelが提供するAIを活用した開発支援ツール  
- プロンプトを入力することでUIコンポーネントやコードを自動生成可能  
- デザインからコードへの変換を高速に行えるため、素早いプロトタイピングに有効

### [Vercel](https://vercel.com/)
- フロントエンド開発者向けのホスティングプラットフォーム  
- Next.jsとの親和性が高く、簡単にデプロイ可能  
- 自動ビルド、プレビュー環境、カスタムドメイン管理などが提供される

### [Supabase](https://supabase.com/)
- Firebaseの代替として注目されるオープンソースのBaaS (Backend as a Service)  
- PostgreSQLをベースとし、認証、リアルタイムDB、ストレージなどを提供  
- フロントエンドとシームレスに接続でき、サーバーレス構成が可能

### [GitHub](https://github.com/)
- ソースコード管理プラットフォーム  
- バージョン管理（Git）をベースに、コラボレーションやCI/CD連携も可能  
- IssuesやPull Requestを通じてチーム開発の効率を高められる

### [Visual Studio Code](https://code.visualstudio.com/)
- ローカル環境で利用する統合開発環境（IDE）  
- 多数の拡張機能があり、SupabaseやVercelとの連携も容易  
- デバッグ、Lint、フォーマット、自動補完など開発支援機能が豊富

---

## 🚀 セットアップ手順

```bash
# 0. Node.js と npm のインストール方法

# --- Mac (Homebrew を利用する場合) ---
brew install node

# --- Windows (Chocolatey を利用する場合) ---
choco install nodejs

# インストール確認
node -v
npm -v

参考リンク：
https://zenn.dev/vkao/articles/8678cb675d5ee5   

# 1. リポジトリをクローン
git clone https://github.com/<your-username>/toyooka-ai-learning.git
cd toyooka-ai-learning

# 2. 依存パッケージをインストール
npm install

# 3. 環境変数ファイルを作成
#   ルートディレクトリに `.env.local` を作成し、以下を記入してください
#   NEXT_PUBLIC_SUPABASE_URL=<your-supabase-url>
#   NEXT_PUBLIC_SUPABASE_ANON_KEY=<your-supabase-anon-key>

# 4. ローカル開発サーバーを起動
npm run dev
# → ブラウザで http://localhost:3000 を開く

# 5. Supabase のセットアップ
#   - https://supabase.com にログインし、新規プロジェクトを作成
#   - Database URL と Anon Key を取得して `.env.local` に設定

# 6. Vercel にデプロイ
#   - https://vercel.com にログイン
#   - 「New Project」からGitHubリポジトリをインポート
#   - 環境変数を設定して「Deploy」をクリック


# 6. 📚 参考リンク

- v0: https://v0.dev/
- Vercel: https://vercel.com/
- Supabase: https://supabase.com/
- GitHub: https://github.com/
- Visual Studio Code: https://code.visualstudio.com/
- Node.js: https://nodejs.org/
