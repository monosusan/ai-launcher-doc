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

## 빠른 시작

1. AI Launcher 공식 웹사이트에서 구매
   
   [https://ai-startups.uk/#pricing](https://ai-startups.uk/#pricing)

2. 결제 후 주문 센터 접속
   
   [https://ai-startups.uk/my-orders](https://ai-startups.uk/my-orders)
   
   활성화를 위해 주문을 선택하세요.
   <img width="1276" alt="Xnip2025-01-13_22-10-13" src="https://github.com/user-attachments/assets/04002ad8-4ad7-4c87-b136-f858a5e9a3e9" />

3. 활성화를 위해 Github 사용자 이름 연동
   
   <img width="507" alt="Xnip2025-01-14_00-45-09" src="https://github.com/user-attachments/assets/79d5fd6f-2a08-4876-a2fe-b656f925330b" />

4. 활성화 성공 후, Github 알림에서 초대를 받게 됩니다. AI Launcher 코드 저장소에 참여하려면 클릭하세요.

## 프로젝트 코드 클론

1. AI Launcher 코드 저장소 접속 (참여하지 않은 경우 404 표시)
   
   [https://github.com/monosusan/ai-launcher-code-template](https://github.com/monosusan/ai-launcher-code-template)

2. Git 클론을 선택하거나 소스 코드를 로컬 컴퓨터에 직접 다운로드

   <img width="918" alt="image" src="https://github.com/user-attachments/assets/080f1d93-c08d-4360-a9c4-012683a45bee" />

## 프로젝트 설치

1. 프로젝트 루트 디렉토리로 이동
   
   ```bash
   cd ai-launcher-code-template
   ```

2. 프로젝트 종속성 설치

   ```bash
   pnpm install
   ```

## 개발 및 디버깅

1. 환경 변수 설정 파일 복사

   ```bash
   cp .env.example .env.development
   ```

2. 개발 서버 시작

   ```bash
   pnpm dev
   ```

3. 로컬 미리보기
   
   브라우저에서 [http://localhost:3000](http://localhost:3000/)을 열어 프로젝트를 미리보기

   <img width="1345" alt="image" src="https://github.com/user-attachments/assets/c6419f32-d296-4f71-bdc6-67cbfa5f0c9a" />

## 커스터마이징

### 웹사이트 색상 변경

1. shadcn 테마 디버거 선택
   * [shadcn themes](https://ui.shadcn.com/themes)
   * [shadcn-ui-theme-generator](https://zippystarter.com/tools/shadcn-ui-theme-generator)

2. 프로젝트의 색상 스키마 생성

![image](https://github.com/user-attachments/assets/76f95a54-3fc9-4d72-b9ae-e6ae4f2ce1f3)

3. 테마 스타일을 복사하여 프로젝트 파일에 붙여넣기

<img width="770" alt="image" src="https://github.com/user-attachments/assets/25ce525e-9a16-4066-a695-f5ed824d8ab4" />

4. 프로젝트 미리보기 페이지를 새로고침하여 사용자 정의 테마 확인

### 홈페이지 콘텐츠 변경

1. 홈페이지 콘텐츠 파일을 열고 AI를 사용하여 새로운 콘텐츠 생성

<img width="1756" alt="image" src="https://github.com/user-attachments/assets/7b12d54b-2b81-4945-b025-97eda51c4506" />

2. AI 생성 콘텐츠를 적용하고 수동으로 조정한 후 새로운 홈페이지 미리보기
3. 다른 JSON 파일도 계속 조정하여 웹사이트 콘텐츠가 프로젝트와 일치하도록 함

### 다국어 텍스트 변경

디렉토리에서 파일을 통해 페이지 콘텐츠를 구성합니다. 중국어와 영어가 기본적으로 지원됩니다. 프로젝트 출시 전에 텍스트를 프로젝트에 맞게 수정하세요.

<img width="1100" alt="image" src="https://github.com/user-attachments/assets/fc15d407-8b96-4756-aa2f-c4bb58954471" />

콘텐츠 생성에 AI를 활용할 수 있습니다.

### 웹사이트 정책 변경

웹사이트를 공식적으로 출시하기 전에 사이트의 서비스에 따라 웹사이트 정책을 업데이트하세요.

1. 개인정보 처리방침 업데이트
   
   Windsurf에서 프롬프트를 사용하여 새로운 개인정보 처리방침 콘텐츠를 생성합니다.
   
   ```
   update privacy-policy according to landing page content @en.json
   with brand name "AILauncher", domain "ai-startups.uk", contact email is "contact@ai-startups.uk"
   ```
   
   개인정보 처리방침을 업데이트하기 위해 파일 내용을 교체하세요.

2. 서비스 약관 업데이트
   
   Windsurf에서 프롬프트를 사용하여 새로운 서비스 약관 콘텐츠를 생성합니다.

   ```
   update terms-of-service according to landing page content @en.json
   with brand name "AILauncher", domain "ai-startups.uk", contact email is "contact@ai-startups.uk"
   ```
   
   서비스 약관을 업데이트하기 위해 파일 내용을 교체하세요.

## 환경 변수 변경

데이터 저장소/로그인/분석/결제 및 기타 기능을 활성화하기 위해 실제 요구 사항에 따라 환경 변수를 수정하세요.

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

## 배포

1. Github 저장소 생성

2. 수정된 프로젝트 코드를 Github 저장소에 커밋

3. Vercel 콘솔에서 새 프로젝트를 생성하고 코드 저장소를 가져와 원클릭 배포

   <img width="685" alt="image" src="https://github.com/user-attachments/assets/3baf7b2c-ad94-4022-b391-26ebb6df14dc" />

4. 빌드가 완료되면 Vercel 콘솔에서 프로젝트를 볼 수 있습니다

   <img width="1241" alt="image" src="https://github.com/user-attachments/assets/5c0e0252-0e1d-4bc9-8012-f5e122b0d7f8" />

5. 도메인 이름을 열어 프로젝트에 접속