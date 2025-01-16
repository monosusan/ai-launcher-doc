- [English](./README.md)
- [简体中文](./README.ZH-CN.md)
- [正體中文](./README.ZH-TW.md)

## Quick Start

1. Purchase on AI Launcher Official Website
   
   [https://ai-startups.uk/#pricing](https://ai-startups.uk/#pricing)

2. After Payment, Enter Order Center
   
   [https://ai-startups.uk/my-orders](https://ai-startups.uk/my-orders)
   
   Select your order for activation.
   <img width="1276" alt="Xnip2025-01-13_22-10-13" src="https://github.com/user-attachments/assets/04002ad8-4ad7-4c87-b136-f858a5e9a3e9" />

3. Bind Your Github Username for Activation
   
   <img width="507" alt="Xnip2025-01-14_00-45-09" src="https://github.com/user-attachments/assets/79d5fd6f-2a08-4876-a2fe-b656f925330b" />

4. After successful activation, you will receive an invitation in your Github notifications. Click to join the AI Launcher code repository.

## Clone Project Code

1. Access the AI Launcher Code Repository (will show 404 if you haven't joined)
   
   [https://github.com/monosusan/ai-launcher-code-template](https://github.com/monosusan/ai-launcher-code-template)

2. Choose to Git Clone or Directly Download the Source Code to Your Local Computer

   <img width="918" alt="image" src="https://github.com/user-attachments/assets/080f1d93-c08d-4360-a9c4-012683a45bee" />

## Install Project

1. Navigate to Project Root Directory
   
   ```bash
   cd ai-launcher-code-template
   ```

2. Install Project Dependencies

   ```bash
   pnpm install
   ```

## Development and Debugging

1. Copy Environment Variable Configuration File

   ```bash
   cp .env.example .env.development
   ```

2. Start Development Server

   ```bash
   pnpm dev
   ```

3. Local Preview
   
   Open [http://localhost:3000](http://localhost:3000/) in your browser to preview your project

   <img width="1345" alt="image" src="https://github.com/user-attachments/assets/c6419f32-d296-4f71-bdc6-67cbfa5f0c9a" />

## Customization

### Modify Website Colors

1. Choose a shadcn Theme Debugger
   * [shadcn themes](https://ui.shadcn.com/themes)
   * [shadcn-ui-theme-generator](https://zippystarter.com/tools/shadcn-ui-theme-generator)

2. Create a Theme Color Scheme for Your Project

![image](https://github.com/user-attachments/assets/76f95a54-3fc9-4d72-b9ae-e6ae4f2ce1f3)

3. Copy Theme Styles and Paste into Project Files

<img width="770" alt="image" src="https://github.com/user-attachments/assets/25ce525e-9a16-4066-a695-f5ed824d8ab4" />

4. Refresh the Project Preview Page to See Your Custom Theme

### Modify Landing Page Content

1. Open the Landing Page Content File, Use AI to Generate New Landing Page Content

<img width="1756" alt="image" src="https://github.com/user-attachments/assets/7b12d54b-2b81-4945-b025-97eda51c4506" />

2. Apply AI-generated Landing Page Content, Make Manual Adjustments, and Preview the New Landing Page
3. Continue Adjusting Other JSON Files to Make Website Content Match Your Project

### Modify Multilingual Text

In the directory, configure page content through files. Chinese and English are supported by default. Before project launch, modify the text to match your project.

<img width="1100" alt="image" src="https://github.com/user-attachments/assets/fc15d407-8b96-4756-aa2f-c4bb58954471" />

You can use AI to assist in content generation.

### Modify Website Policies

Before officially launching the website, update the website policies according to your website's services.

1. Update Privacy Policy
   
   In Windsurf, generate new privacy policy content using prompts.
   
   ```
   update privacy-policy according to landing page content @en.json
   with brand name "AILauncher", domain "ai-startups.uk", contact email is "contact@ai-startups.uk"
   ```
   
   Replace file content to update privacy policy.

2. Update Terms of Service
   
   In Windsurf, generate new terms of service content using prompts.

   ```
   update terms-of-service according to landing page content @en.json
   with brand name "AILauncher", domain "ai-startups.uk", contact email is "contact@ai-startups.uk"
   ```
   
   Replace file content to update terms of service.

## Modify Environment Variables

Modify environment variables according to actual needs to enable data storage / login / analytics / payment and other features

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

## Deployment

1. Create a Github repository

2. Commit the modified project code to the Github repository

3. Create a new project in the Vercel console, import the code repository, and deploy with one click

   <img width="685" alt="image" src="https://github.com/user-attachments/assets/3baf7b2c-ad94-4022-b391-26ebb6df14dc" />


4. After the build is complete, you can see your project in the Vercel console

   <img width="1241" alt="image" src="https://github.com/user-attachments/assets/5c0e0252-0e1d-4bc9-8012-f5e122b0d7f8" />



