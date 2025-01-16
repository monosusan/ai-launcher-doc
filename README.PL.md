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

## Szybki Start

1. Kup na oficjalnej stronie AI Launcher
   
   [https://ai-startups.uk/#pricing](https://ai-startups.uk/#pricing)

2. Po dokonaniu płatności, wejdź do Centrum Zamówień
   
   [https://ai-startups.uk/my-orders](https://ai-startups.uk/my-orders)
   
   Wybierz swoje zamówienie do aktywacji.
   <img width="1276" alt="Xnip2025-01-13_22-10-13" src="https://github.com/user-attachments/assets/04002ad8-4ad7-4c87-b136-f858a5e9a3e9" />

3. Powiąż swoją nazwę użytkownika Github do aktywacji
   
   <img width="507" alt="Xnip2025-01-14_00-45-09" src="https://github.com/user-attachments/assets/79d5fd6f-2a08-4876-a2fe-b656f925330b" />

4. Po pomyślnej aktywacji otrzymasz zaproszenie w powiadomieniach Github. Kliknij, aby dołączyć do repozytorium kodu AI Launcher.

## Klonowanie Kodu Projektu

1. Dostęp do repozytorium kodu AI Launcher (pokazuje 404, jeśli nie jesteś członkiem)
   
   [https://github.com/monosusan/ai-launcher-code-template](https://github.com/monosusan/ai-launcher-code-template)

2. Wybierz klonowanie Git lub pobierz kod źródłowy bezpośrednio na swój lokalny komputer

   <img width="918" alt="image" src="https://github.com/user-attachments/assets/080f1d93-c08d-4360-a9c4-012683a45bee" />

## Instalacja Projektu

1. Przejdź do głównego katalogu projektu
   
   ```bash
   cd ai-launcher-code-template
   ```

2. Zainstaluj zależności projektu

   ```bash
   pnpm install
   ```

## Rozwój i Debugowanie

1. Skopiuj plik konfiguracyjny zmiennych środowiskowych

   ```bash
   cp .env.example .env.development
   ```

2. Uruchom serwer deweloperski

   ```bash
   pnpm dev
   ```

3. Podgląd lokalny
   
   Otwórz [http://localhost:3000](http://localhost:3000/) w przeglądarce, aby zobaczyć projekt

   <img width="1345" alt="image" src="https://github.com/user-attachments/assets/c6419f32-d296-4f71-bdc6-67cbfa5f0c9a" />

## Dostosowywanie

### Zmiana Kolorów Strony

1. Wybierz debugger motywów shadcn
   * [shadcn themes](https://ui.shadcn.com/themes)
   * [shadcn-ui-theme-generator](https://zippystarter.com/tools/shadcn-ui-theme-generator)

2. Stwórz schemat kolorów dla swojego projektu

![image](https://github.com/user-attachments/assets/76f95a54-3fc9-4d72-b9ae-e6ae4f2ce1f3)

3. Skopiuj style motywu i wklej je do plików projektu

<img width="770" alt="image" src="https://github.com/user-attachments/assets/25ce525e-9a16-4066-a695-f5ed824d8ab4" />

4. Odśwież stronę podglądu projektu, aby zobaczyć niestandardowy motyw

### Zmiana Zawartości Strony Głównej

1. Otwórz plik zawartości strony głównej i użyj AI do wygenerowania nowej treści

<img width="1756" alt="image" src="https://github.com/user-attachments/assets/7b12d54b-2b81-4945-b025-97eda51c4506" />

2. Zastosuj wygenerowaną przez AI treść, dokonaj ręcznych korekt i podejrzyj nową stronę główną
3. Kontynuuj dostosowywanie innych plików JSON, aby zawartość witryny była zgodna z Twoim projektem

### Zmiana Tekstu Wielojęzycznego

W katalogu skonfiguruj zawartość strony poprzez pliki. Chiński i angielski są obsługiwane domyślnie. Dostosuj tekst do swojego projektu przed uruchomieniem.

<img width="1100" alt="image" src="https://github.com/user-attachments/assets/fc15d407-8b96-4756-aa2f-c4bb58954471" />

Możesz wykorzystać AI do generowania treści.

### Zmiana Polityk Witryny

Przed oficjalnym uruchomieniem witryny zaktualizuj polityki zgodnie z usługami Twojej strony.

1. Aktualizacja Polityki Prywatności
   
   W Windsurf użyj promptu do wygenerowania nowej treści polityki prywatności.
   
   ```
   update privacy-policy according to landing page content @en.json
   with brand name "AILauncher", domain "ai-startups.uk", contact email is "contact@ai-startups.uk"
   ```
   
   Zastąp zawartość pliku, aby zaktualizować politykę prywatności.

2. Aktualizacja Warunków Korzystania z Usług
   
   W Windsurf użyj promptu do wygenerowania nowej treści warunków korzystania z usług.

   ```
   update terms-of-service according to landing page content @en.json
   with brand name "AILauncher", domain "ai-startups.uk", contact email is "contact@ai-startups.uk"
   ```
   
   Zastąp zawartość pliku, aby zaktualizować warunki korzystania z usług.

## Zmiana Zmiennych Środowiskowych

Zmodyfikuj zmienne środowiskowe zgodnie z rzeczywistymi potrzebami, aby włączyć przechowywanie danych/logowanie/analitykę/płatności i inne funkcje

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

## Wdrożenie

1. Utwórz repozytorium Github

2. Zatwierdź zmodyfikowany kod projektu do repozytorium Github

3. Utwórz nowy projekt w konsoli Vercel, zaimportuj repozytorium kodu i wdróż jednym kliknięciem
  <img width="685" alt="image" src="https://github.com/user-attachments/assets/3baf7b2c-ad94-4022-b391-26ebb6df14dc" />

4. Skonfiguruj ustawienia nazwy domeny i certyfikat SSL w konsoli Vercel

<img width="1241" alt="image" src="https://github.com/user-attachments/assets/5c0e0252-0e1d-4bc9-8012-f5e122b0d7f8" />

5. Uruchom oficjalną stronę