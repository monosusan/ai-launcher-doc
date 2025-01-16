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

## Snelle Start

1. Koop op de Officiële AI Launcher Website
   
   [https://ai-startups.uk/#pricing](https://ai-startups.uk/#pricing)

2. Na betaling, ga naar het Ordercentrum
   
   [https://ai-startups.uk/my-orders](https://ai-startups.uk/my-orders)
   
   Selecteer uw bestelling voor activering.
   <img width="1276" alt="Xnip2025-01-13_22-10-13" src="https://github.com/user-attachments/assets/04002ad8-4ad7-4c87-b136-f858a5e9a3e9" />

3. Koppel uw Github gebruikersnaam voor activering
   
   <img width="507" alt="Xnip2025-01-14_00-45-09" src="https://github.com/user-attachments/assets/79d5fd6f-2a08-4876-a2fe-b656f925330b" />

4. Na succesvolle activering ontvangt u een uitnodiging in uw Github meldingen. Klik om lid te worden van de AI Launcher code repository.

## Project Code Klonen

1. Toegang tot AI Launcher Code Repository (toont 404 als u geen lid bent)
   
   [https://github.com/monosusan/ai-launcher-code-template](https://github.com/monosusan/ai-launcher-code-template)

2. Kies om Git te klonen of download de broncode direct naar uw lokale computer

   <img width="918" alt="image" src="https://github.com/user-attachments/assets/080f1d93-c08d-4360-a9c4-012683a45bee" />

## Project Installatie

1. Navigeer naar de hoofdmap van het project
   
   ```bash
   cd ai-launcher-code-template
   ```

2. Installeer projectafhankelijkheden

   ```bash
   pnpm install
   ```

## Ontwikkeling en Debugging

1. Kopieer het omgevingsvariabelen configuratiebestand

   ```bash
   cp .env.example .env.development
   ```

2. Start de ontwikkelingsserver

   ```bash
   pnpm dev
   ```

3. Lokale preview
   
   Open [http://localhost:3000](http://localhost:3000/) in uw browser om het project te bekijken

   <img width="1345" alt="image" src="https://github.com/user-attachments/assets/c6419f32-d296-4f71-bdc6-67cbfa5f0c9a" />

## Aanpassing

### Website Kleuren Wijzigen

1. Kies shadcn thema debugger
   * [shadcn themes](https://ui.shadcn.com/themes)
   * [shadcn-ui-theme-generator](https://zippystarter.com/tools/shadcn-ui-theme-generator)

2. Maak een kleurenschema voor uw project

![image](https://github.com/user-attachments/assets/76f95a54-3fc9-4d72-b9ae-e6ae4f2ce1f3)

3. Kopieer de themastijlen en plak ze in uw projectbestanden

<img width="770" alt="image" src="https://github.com/user-attachments/assets/25ce525e-9a16-4066-a695-f5ed824d8ab4" />

4. Vernieuw de projectpreviewpagina om uw aangepaste thema te bekijken

### Homepage Inhoud Wijzigen

1. Open het homepage inhoudsbestand en gebruik AI om nieuwe inhoud te genereren

<img width="1756" alt="image" src="https://github.com/user-attachments/assets/7b12d54b-2b81-4945-b025-97eda51c4506" />

2. Pas de AI-gegenereerde inhoud toe, maak handmatige aanpassingen en bekijk de nieuwe homepage
3. Blijf andere JSON-bestanden aanpassen om de website-inhoud af te stemmen op uw project

### Meertalige Tekst Wijzigen

In de directory configureert u de paginainhoud via bestanden. Chinees en Engels worden standaard ondersteund. Pas de tekst aan uw project aan voordat u live gaat.

<img width="1100" alt="image" src="https://github.com/user-attachments/assets/fc15d407-8b96-4756-aa2f-c4bb58954471" />

U kunt AI gebruiken voor het genereren van inhoud.

### Website Beleid Wijzigen

Voordat u uw website officieel lanceert, werk het websitebeleid bij volgens uw sitediensten.

1. Privacy Beleid Bijwerken
   
   Gebruik in Windsurf de prompt om nieuwe privacybeleid inhoud te genereren.
   
   ```
   update privacy-policy according to landing page content @en.json
   with brand name "AILauncher", domain "ai-startups.uk", contact email is "contact@ai-startups.uk"
   ```
   
   Vervang de bestandsinhoud om het privacybeleid bij te werken.

2. Servicevoorwaarden Bijwerken
   
   Gebruik in Windsurf de prompt om nieuwe servicevoorwaarden inhoud te genereren.

   ```
   update terms-of-service according to landing page content @en.json
   with brand name "AILauncher", domain "ai-startups.uk", contact email is "contact@ai-startups.uk"
   ```
   
   Vervang de bestandsinhoud om de servicevoorwaarden bij te werken.

## Omgevingsvariabelen Wijzigen

Wijzig de omgevingsvariabelen volgens uw werkelijke behoeften om dataopslag/login/analytics/betalingen en andere functies in te schakelen

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

1. Maak een Github repository aan

2. Commit uw aangepaste projectcode naar de Github repository

3. Maak een nieuw project aan in de Vercel console, importeer de coderepository en deploy met één klik

<img width="685" alt="image" src="https://github.com/user-attachments/assets/3baf7b2c-ad94-4022-b391-26ebb6df14dc" />

4. Configureer de domeinnaaminstellingen en SSL-certificaat in de Vercel console

<img width="1241" alt="image" src="https://github.com/user-attachments/assets/5c0e0252-0e1d-4bc9-8012-f5e122b0d7f8" />

5. Start de officiële website