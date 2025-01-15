- [English](./README.md)
- [简体中文](./README.ZH-CN.md)


## 快速开始

1. 在 AI Launcher 官网下单购买
   
   [https://ai-startups.uk/#pricing](https://ai-startups.uk/#pricing)

2. 支付完成后，进入订单中心
   
   [https://ai-startups.uk/my-orders](https://ai-startups.uk/my-orders)
   
   选择订单进行激活。
   <img width="1276" alt="Xnip2025-01-13_22-10-13" src="https://github.com/user-attachments/assets/04002ad8-4ad7-4c87-b136-f858a5e9a3e9" />


3. 绑定你的 Github Username 进行激活
   
   <img width="507" alt="Xnip2025-01-14_00-45-09" src="https://github.com/user-attachments/assets/79d5fd6f-2a08-4876-a2fe-b656f925330b" />


4. 激活成功后，你将在 Github 通知中心收到邀请，点击加入 AI Launcher 代码仓库

## 拉取项目代码

1. 进入 AI Launcher 代码仓库（如果未加入仓库，打开会是 404）
   
   [https://github.com/monosusan/ai-launcher-code-template](https://github.com/monosusan/ai-launcher-code-template)

2. 选择 git clone 的方式，或者直接下载源代码到你的本地电脑

   <img width="918" alt="图片" src="https://github.com/user-attachments/assets/080f1d93-c08d-4360-a9c4-012683a45bee" />


## 安装项目

1. 进入项目根目录
   
   ```
   cd ai-launcher-code-template
   ```
2. 安装项目依赖

   ```
   pnpm install
   ```

## 开发调试

1. 复制环境变量配置文件

```
cp .env.example .env.development
```

2. 启动开发服务器

```
pnpm dev
```

3. 本地预览
   
   在浏览器打开 [http://localhost:3000](http://localhost:3000/) ，即可预览你的项目

   <img width="1345" alt="图片" src="https://github.com/user-attachments/assets/c6419f32-d296-4f71-bdc6-67cbfa5f0c9a" />


## 定制化修改

### 修改网页配色

1. 选择一个 shadcn 主题调试器
   * [shadcn themes](https://ui.shadcn.com/themes)
   * [shadcn-ui-theme-generator](https://zippystarter.com/tools/shadcn-ui-theme-generator)

2. 为你的项目调制一套主题配色

![图片](https://github.com/user-attachments/assets/76f95a54-3fc9-4d72-b9ae-e6ae4f2ce1f3)

   
4. 复制主题样式，粘贴到项目文件

<img width="770" alt="图片" src="https://github.com/user-attachments/assets/25ce525e-9a16-4066-a695-f5ed824d8ab4" />


5. 重新进入项目预览页面，即可看到你定制的主题

### 修改落地页内容

1. 打开落地页内容文件，AI 辅助生成新的落地页内容

<img width="1756" alt="图片" src="https://github.com/user-attachments/assets/7b12d54b-2b81-4945-b025-97eda51c4506" />


2. 应用 AI 生成的新落地页内容，人工稍加调整，重新预览新的落地页
3. 继续调整下的其他 json 文件，使网页显示的内容跟你的项目相符

### 修改多语言文案

在目录下，通过文件配置页面内容，默认支持中文和英文，在目录下，可以看到和两个文件，在项目发布之前，修改成跟你项目相符合的文案即可。

<img width="1100" alt="图片" src="https://github.com/user-attachments/assets/fc15d407-8b96-4756-aa2f-c4bb58954471" />

可以让 AI 辅助生成内容。

### 修改网站协议

在网站正式上线之前，请根据你网站提供的服务，更新目录下的网站协议。

1. 更新隐私政策
   
   在 Windsurf 中，通过提示词生成新的隐私政策内容。
   
```
update privacy-policy according to landing page content @en.json
with brand name "AILauncher", domain "ai-startups.uk", contact email is "contact@ai-startups.uk"
```
   
   替换文件中的内容，更新隐私政策。

3. 更新服务条款
   
   在 Windsurf 中，通过提示词生成新的服务条款内容。

```
update terms-of-service according to landing page content @en.json
with brand name "AILauncher", domain "ai-startups.uk", contact email is "contact@ai-startups.uk"
```
   
   替换文件中的内容，更新服务条款。

## 修改环境变量

根据实际需求，修改环境变量，开启数据存储 / 登录 / 数据统计 / 支付等功能

```
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

## 发布上线

1. 创建 Github 仓库

2. 将修改后的项目代码，提交到项目 Github 仓库

3. 在 Vercel 控制台创建新项目，导入代码仓库，一键部署

4. 等构建完成，即可在 Vercel 控制台看到你的项目

5. 打开域名，即可访问你的项目
