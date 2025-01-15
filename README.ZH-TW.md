- [English](./README.md)
- [简体中文](./README.ZH-CN.md)
- [正體中文](./README.ZH-TW.md)

## 快速開始

1. 在 AI Launcher 官網下單購買
   
   [https://ai-startups.uk/#pricing](https://ai-startups.uk/#pricing)

2. 支付完成後，進入訂單中心
   
   [https://ai-startups.uk/my-orders](https://ai-startups.uk/my-orders)
   
   選擇訂單進行啟用。
   <img width="1276" alt="Xnip2025-01-13_22-10-13" src="https://github.com/user-attachments/assets/04002ad8-4ad7-4c87-b136-f858a5e9a3e9" />

3. 綁定你的 Github Username 進行啟用
   
   <img width="507" alt="Xnip2025-01-14_00-45-09" src="https://github.com/user-attachments/assets/79d5fd6f-2a08-4876-a2fe-b656f925330b" />

4. 啟用成功後，你將在 Github 通知中心收到邀請，點擊加入 AI Launcher 程式碼儲存庫

## 取得專案程式碼

1. 進入 AI Launcher 程式碼儲存庫（如果未加入儲存庫，打開會是 404）
   
   [https://github.com/monosusan/ai-launcher-code-template](https://github.com/monosusan/ai-launcher-code-template)

2. 選擇 git clone 的方式，或者直接下載原始碼到你的本機電腦

   <img width="918" alt="圖片" src="https://github.com/user-attachments/assets/080f1d93-c08d-4360-a9c4-012683a45bee" />

## 安裝專案

1. 進入專案根目錄
   
   ```bash
   cd ai-launcher-code-template
   ```

2. 安裝專案相依套件

   ```bash
   pnpm install
   ```

## 開發除錯

1. 複製環境變數設定檔

   ```bash
   cp .env.example .env.development
   ```

2. 啟動開發伺服器

   ```bash
   pnpm dev
   ```

3. 本機預覽
   
   在瀏覽器打開 [http://localhost:3000](http://localhost:3000/) ，即可預覽你的專案

   <img width="1345" alt="圖片" src="https://github.com/user-attachments/assets/c6419f32-d296-4f71-bdc6-67cbfa5f0c9a" />

## 客製化修改

### 修改網頁配色

1. 選擇一個 shadcn 主題除錯器
   * [shadcn themes](https://ui.shadcn.com/themes)
   * [shadcn-ui-theme-generator](https://zippystarter.com/tools/shadcn-ui-theme-generator)

2. 為你的專案調製一套主題配色

![圖片](https://github.com/user-attachments/assets/76f95a54-3fc9-4d72-b9ae-e6ae4f2ce1f3)

3. 複製主題樣式，貼上到專案檔案

<img width="770" alt="圖片" src="https://github.com/user-attachments/assets/25ce525e-9a16-4066-a695-f5ed824d8ab4" />

4. 重新進入專案預覽頁面，即可看到你客製化的主題

### 修改登陸頁內容

1. 打開登陸頁內容檔案，AI 輔助生成新的登陸頁內容

<img width="1756" alt="圖片" src="https://github.com/user-attachments/assets/7b12d54b-2b81-4945-b025-97eda51c4506" />

2. 應用 AI 生成的新登陸頁內容，人工稍加調整，重新預覽新的登陸頁
3. 繼續調整其他的 json 檔案，使網頁顯示的內容與你的專案相符

### 修改多語言文案

在目錄下，透過檔案配置頁面內容，預設支援中文和英文，在目錄下，可以看到兩個檔案，在專案發布之前，修改成與你專案相符合的文案即可。

<img width="1100" alt="圖片" src="https://github.com/user-attachments/assets/fc15d407-8b96-4756-aa2f-c4bb58954471" />

可以讓 AI 輔助生成內容。

### 修改網站協議

在網站正式上線之前，請根據你網站提供的服務，更新目錄下的網站協議。

1. 更新隱私政策
   
   在 Windsurf 中，透過提示詞生成新的隱私政策內容。
   
   ```
   update privacy-policy according to landing page content @en.json
   with brand name "AILauncher", domain "ai-startups.uk", contact email is "contact@ai-startups.uk"
   ```
   
   替換檔案中的內容，更新隱私政策。

2. 更新服務條款
   
   在 Windsurf 中，透過提示詞生成新的服務條款內容。

   ```
   update terms-of-service according to landing page content @en.json
   with brand name "AILauncher", domain "ai-startups.uk", contact email is "contact@ai-startups.uk"
   ```
   
   替換檔案中的內容，更新服務條款。

## 修改環境變數

根據實際需求，修改環境變數，開啟資料儲存 / 登入 / 資料統計 / 支付等功能

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
NEXT_PUBLIC_PAY_FAIL_URL = "http://localhost:3000/#pricing"
NEXT_PUBLIC_PAY_CANCEL_URL = "http://localhost:3000/#pricing"

NEXT_PUBLIC_LOCALE_DETECTION = "false"

ADMIN_EMAILS = ""
```


## 部署
1. 建立 Github 儲存庫

2. 將修改後的專案程式碼，提交到專案 Github 儲存庫

3. 在 Vercel 控制台建立新專案，匯入程式碼儲存庫，一鍵部署

4. 等建置完成，即可在 Vercel 控制台看到你的專案

5. 開啟網域，即可存取你的專案