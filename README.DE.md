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

## Schnellstart

1. Kauf auf der offiziellen AI Launcher Website
   
   [https://ai-startups.uk/#pricing](https://ai-startups.uk/#pricing)

2. Nach der Zahlung ins Bestellcenter gehen
   
   [https://ai-startups.uk/my-orders](https://ai-startups.uk/my-orders)
   
   Wählen Sie Ihre Bestellung zur Aktivierung aus.
   <img width="1276" alt="Xnip2025-01-13_22-10-13" src="https://github.com/user-attachments/assets/04002ad8-4ad7-4c87-b136-f858a5e9a3e9" />

3. Binden Sie Ihren Github-Benutzernamen für die Aktivierung
   
   <img width="507" alt="Xnip2025-01-14_00-45-09" src="https://github.com/user-attachments/assets/79d5fd6f-2a08-4876-a2fe-b656f925330b" />

4. Nach erfolgreicher Aktivierung erhalten Sie eine Einladung in Ihren Github-Benachrichtigungen. Klicken Sie, um dem AI Launcher Code Repository beizutreten.

## Projekt-Code klonen

1. Zugriff auf das AI Launcher Code Repository (zeigt 404, wenn Sie noch nicht beigetreten sind)
   
   [https://github.com/monosusan/ai-launcher-code-template](https://github.com/monosusan/ai-launcher-code-template)

2. Wählen Sie Git Clone oder laden Sie den Quellcode direkt auf Ihren lokalen Computer herunter

   <img width="918" alt="image" src="https://github.com/user-attachments/assets/080f1d93-c08d-4360-a9c4-012683a45bee" />

## Projekt installieren

1. Navigieren Sie zum Projekt-Stammverzeichnis
   
   ```bash
   cd ai-launcher-code-template
   ```

2. Installieren Sie die Projektabhängigkeiten

   ```bash
   pnpm install
   ```

## Entwicklung und Debugging

1. Kopieren Sie die Umgebungsvariablen-Konfigurationsdatei

   ```bash
   cp .env.example .env.development
   ```

2. Starten Sie den Entwicklungsserver

   ```bash
   pnpm dev
   ```

3. Lokale Vorschau
   
   Öffnen Sie [http://localhost:3000](http://localhost:3000/) in Ihrem Browser, um Ihr Projekt anzuzeigen

   <img width="1345" alt="image" src="https://github.com/user-attachments/assets/c6419f32-d296-4f71-bdc6-67cbfa5f0c9a" />

## Anpassung

### Website-Farben ändern

1. Wählen Sie einen shadcn Theme Debugger
   * [shadcn themes](https://ui.shadcn.com/themes)
   * [shadcn-ui-theme-generator](https://zippystarter.com/tools/shadcn-ui-theme-generator)

2. Erstellen Sie ein Farbschema für Ihr Projekt

![image](https://github.com/user-attachments/assets/76f95a54-3fc9-4d72-b9ae-e6ae4f2ce1f3)

3. Kopieren Sie die Theme-Stile und fügen Sie sie in die Projektdateien ein

<img width="770" alt="image" src="https://github.com/user-attachments/assets/25ce525e-9a16-4066-a695-f5ed824d8ab4" />

4. Aktualisieren Sie die Projekt-Vorschauseite, um Ihr angepasstes Theme zu sehen

### Landing Page Inhalt ändern

1. Öffnen Sie die Landing Page Inhaltsdatei, verwenden Sie KI, um neue Landing Page Inhalte zu generieren

<img width="1756" alt="image" src="https://github.com/user-attachments/assets/7b12d54b-2b81-4945-b025-97eda51c4506" />

2. Wenden Sie KI-generierte Landing Page Inhalte an, nehmen Sie manuelle Anpassungen vor und prüfen Sie die neue Landing Page
3. Passen Sie weitere JSON-Dateien an, damit die Website-Inhalte zu Ihrem Projekt passen

### Mehrsprachige Texte ändern

Im Verzeichnis können Sie Seiteninhalte über Dateien konfigurieren. Chinesisch und Englisch werden standardmäßig unterstützt. Ändern Sie vor dem Projektstart die Texte entsprechend Ihrem Projekt.

<img width="1100" alt="image" src="https://github.com/user-attachments/assets/fc15d407-8b96-4756-aa2f-c4bb58954471" />

Sie können KI zur Unterstützung bei der Inhaltserstellung verwenden.

### Website-Richtlinien ändern

Aktualisieren Sie vor dem offiziellen Start der Website die Website-Richtlinien entsprechend Ihren Website-Diensten.

1. Datenschutzerklärung aktualisieren
   
   Generieren Sie in Windsurf neue Datenschutzerklärungsinhalte mit Prompts.
   
   ```
   update privacy-policy according to landing page content @en.json
   with brand name "AILauncher", domain "ai-startups.uk", contact email is "contact@ai-startups.uk"
   ```
   
   Ersetzen Sie den Dateiinhalt, um die Datenschutzerklärung zu aktualisieren.

2. Nutzungsbedingungen aktualisieren
   
   Generieren Sie in Windsurf neue Nutzungsbedingungen mit Prompts.

   ```
   update terms-of-service according to landing page content @en.json
   with brand name "AILauncher", domain "ai-startups.uk", contact email is "contact@ai-startups.uk"
   ```
   
   Ersetzen Sie den Dateiinhalt, um die Nutzungsbedingungen zu aktualisieren.

## Umgebungsvariablen ändern

Ändern Sie die Umgebungsvariablen entsprechend den tatsächlichen Anforderungen, um Datenspeicherung / Login / Analyse / Zahlung und andere Funktionen zu aktivieren

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

## Bereitstellung

1. Erstellen Sie ein Github-Repository

2. Übertragen Sie den modifizierten Projektcode in das Github-Repository

3. Erstellen Sie ein neues Projekt in der Vercel-Konsole, importieren Sie das Code-Repository und stellen Sie es mit einem Klick bereit

   <img width="685" alt="image" src="https://github.com/user-attachments/assets/3baf7b2c-ad94-4022-b391-26ebb6df14dc" />

4. Nach Abschluss des Builds können Sie Ihr Projekt in der Vercel-Konsole sehen

   <img width="1241" alt="image" src="https://github.com/user-attachments/assets/5c0e0252-0e1d-4bc9-8012-f5e122b0d7f8" />

5. Öffnen Sie die Domain, um auf Ihr Projekt zuzugreifen