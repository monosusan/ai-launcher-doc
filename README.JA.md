- [English](./README.md)
- [简体中文](./README.ZH-CN.md)
- [正體中文](./README.ZH-TW.md)
- [हिन्दी](./README.HI-IN.md)
- [Français](./README.FR.md)
- [한국어](./README.KO.md)
- [Español](./README.ES.md)
- [Polski](./README.PL.md)
- [Nederlands](./README.NL.md)
- [Deutsch](./README.DE.md)
- [日本語](./README.JA.md)
- [Tiếng Việt](./README.VI.md)
- [Türkçe](./README.TR.md)

## クイックスタート

1. AI Launcher公式ウェブサイトで購入
   
   [https://ai-startups.uk/#pricing](https://ai-startups.uk/#pricing)

2. 支払い後、注文センターにアクセス
   
   [https://ai-startups.uk/my-orders](https://ai-startups.uk/my-orders)
   
   アクティベーション用の注文を選択してください。
   <img width="1276" alt="Xnip2025-01-13_22-10-13" src="https://github.com/user-attachments/assets/04002ad8-4ad7-4c87-b136-f858a5e9a3e9" />

3. アクティベーション用にGithubユーザー名を紐付け
   
   <img width="507" alt="Xnip2025-01-14_00-45-09" src="https://github.com/user-attachments/assets/79d5fd6f-2a08-4876-a2fe-b656f925330b" />

4. アクティベーション成功後、Githubの通知に招待が届きます。クリックしてAI Launcherコードリポジトリに参加してください。

## プロジェクトコードのクローン

1. AI Launcherコードリポジトリにアクセス（参加していない場合は404が表示されます）
   
   [https://github.com/monosusan/ai-launcher-code-template](https://github.com/monosusan/ai-launcher-code-template)

2. Gitクローンを選択するか、ソースコードを直接ローカルコンピュータにダウンロード

   <img width="918" alt="image" src="https://github.com/user-attachments/assets/080f1d93-c08d-4360-a9c4-012683a45bee" />

## プロジェクトのインストール

1. プロジェクトのルートディレクトリに移動
   
   ```bash
   cd ai-launcher-code-template
   ```

2. プロジェクトの依存関係をインストール

   ```bash
   pnpm install
   ```

## 開発とデバッグ

1. 環境変数設定ファイルをコピー

   ```bash
   cp .env.example .env.development
   ```

2. 開発サーバーを起動

   ```bash
   pnpm dev
   ```

3. ローカルプレビュー
   
   ブラウザで[http://localhost:3000](http://localhost:3000/)を開いてプロジェクトをプレビュー

   <img width="1345" alt="image" src="https://github.com/user-attachments/assets/c6419f32-d296-4f71-bdc6-67cbfa5f0c9a" />

## カスタマイズ

### ウェブサイトの色を変更

1. shadcnテーマデバッガーを選択
   * [shadcn themes](https://ui.shadcn.com/themes)
   * [shadcn-ui-theme-generator](https://zippystarter.com/tools/shadcn-ui-theme-generator)

2. プロジェクトのカラースキームを作成

![image](https://github.com/user-attachments/assets/76f95a54-3fc9-4d72-b9ae-e6ae4f2ce1f3)

3. テーマスタイルをコピーしてプロジェクトファイルに貼り付け

<img width="770" alt="image" src="https://github.com/user-attachments/assets/25ce525e-9a16-4066-a695-f5ed824d8ab4" />

4. プロジェクトプレビューページを更新してカスタムテーマを確認

### ホームページコンテンツの変更

1. ホームページコンテンツファイルを開き、AIを使用して新しいコンテンツを生成

<img width="1756" alt="image" src="https://github.com/user-attachments/assets/7b12d54b-2b81-4945-b025-97eda51c4506" />

2. AI生成コンテンツを適用し、手動調整を行い、新しいホームページをプレビュー
3. 他のJSONファイルも調整を続け、ウェブサイトのコンテンツをプロジェクトに合わせる

### 多言語テキストの変更

ディレクトリ内で、ファイルを通じてページコンテンツを設定します。デフォルトで中国語と英語がサポートされています。プロジェクト立ち上げ前に、テキストをプロジェクトに合わせて修正してください。

<img width="1100" alt="image" src="https://github.com/user-attachments/assets/fc15d407-8b96-4756-aa2f-c4bb58954471" />

コンテンツ生成にAIを活用できます。

### ウェブサイトポリシーの変更

ウェブサイトを正式にローンチする前に、サイトのサービスに応じてウェブサイトポリシーを更新してください。

1. プライバシーポリシーの更新
   
   Windsurfで、プロンプトを使用して新しいプライバシーポリシーコンテンツを生成します。
   
   ```
   update privacy-policy according to landing page content @en.json
   with brand name "AILauncher", domain "ai-startups.uk", contact email is "contact@ai-startups.uk"
   ```
   
   プライバシーポリシーを更新するためにファイルの内容を置き換えてください。

2. 利用規約の更新
   
   Windsurfで、プロンプトを使用して新しい利用規約コンテンツを生成します。

   ```
   update terms-of-service according to landing page content @en.json
   with brand name "AILauncher", domain "ai-startups.uk", contact email is "contact@ai-startups.uk"
   ```
   
   利用規約を更新するためにファイルの内容を置き換えてください。

## 環境変数の変更

データストレージ/ログイン/アナリティクス/支払いなどの機能を有効にするために、実際のニーズに応じて環境変数を修正してください

```env
# -----------------------------------------------------------------------------
# Web Information
# -----------------------------------------------------------------------------
NEXT_PUBLIC_WEB_URL = "http://localhost:3000"
NEXT_PUBLIC_PROJECT_NAME = "AI Launcher"

# -----------------------------------------------------------------------------
# Database with Supabase
# -----------------------------------------------------------------------------
# https://supabase.com/docs/guides/getting-started/quickstarts/nextjs
# Set your Supabase URL and Anon Key
SUPABASE_URL = ""
SUPABASE_ANON_KEY = ""
SUPABASE_SERVICE_ROLE_KEY = ""

# -----------------------------------------------------------------------------
# Auth with next-auth
# https://authjs.dev/getting-started/installation?framework=Next.js
# Set your Auth URL and Secret
# Secret can be generated with `openssl rand -base64 32`
# -----------------------------------------------------------------------------
AUTH_SECRET = ""

# Google Auth
# https://authjs.dev/getting-started/providers/google
AUTH_GOOGLE_ID = ""
AUTH_GOOGLE_SECRET = ""
NEXT_PUBLIC_AUTH_GOOGLE_ID = ""
NEXT_PUBLIC_AUTH_GOOGLE_ENABLED = "false"
NEXT_PUBLIC_AUTH_GOOGLE_ONE_TAP_ENABLED = "false"

# Github Auth
# https://authjs.dev/getting-started/providers/github
AUTH_GITHUB_ID = ""
AUTH_GITHUB_SECRET = ""
NEXT_PUBLIC_AUTH_GITHUB_ENABLED = "false"

# -----------------------------------------------------------------------------
# Analytics with Google Analytics
# https://analytics.google.com
# -----------------------------------------------------------------------------
NEXT_PUBLIC_GOOGLE_ANALYTICS_ID = ""

# -----------------------------------------------------------------------------
# Analytics with OpenPanel
# https://openpanel.dev
# -----------------------------------------------------------------------------
NEXT_PUBLIC_OPENPANEL_CLIENT_ID = ""

# -----------------------------------------------------------------------------
# Payment with Stripe
# https://docs.stripe.com/keys
# -----------------------------------------------------------------------------
STRIPE_PUBLIC_KEY = ""
STRIPE_PRIVATE_KEY = ""
STRIPE_WEBHOOK_SECRET = ""

NEXT_PUBLIC_PAY_SUCCESS_URL = "http://localhost:3000/my-orders"
NEXT_PUBLIC_PAY_FAIL_URL = "http://localhost:3000"
NEXT_PUBLIC_PAY_CANCEL_URL = "http://localhost:3000/#pricing"

NEXT_PUBLIC_LOCALE_DETECTION = "false"

ADMIN_EMAILS = ""
```

## デプロイメント

1. Githubリポジトリを作成

2. 修正したプロジェクトコードをGithubリポジトリにコミット

3. Vercelコンソールで新しいプロジェクトを作成し、コードリポジトリをインポートしてワンクリックデプロイ

   <img width="685" alt="image" src="https://github.com/user-attachments/assets/3baf7b2c-ad94-4022-b391-26ebb6df14dc" />

4. ビルド完了後、Vercelコンソールでプロジェクトが確認できます

   <img width="1241" alt="image" src="https://github.com/user-attachments/assets/5c0e0252-0e1d-4bc9-8012-f5e122b0d7f8" />

5. ドメイン名を開いてプロジェクトにアクセス