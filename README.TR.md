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

## Hızlı Başlangıç

1. AI Launcher Resmi Web Sitesinden Satın Alın
   
   [https://ai-startups.uk/#pricing](https://ai-startups.uk/#pricing)

2. Ödeme Sonrası Sipariş Merkezine Giriş Yapın
   
   [https://ai-startups.uk/my-orders](https://ai-startups.uk/my-orders)
   
   Aktivasyon için siparişinizi seçin.
   <img width="1276" alt="Xnip2025-01-13_22-10-13" src="https://github.com/user-attachments/assets/04002ad8-4ad7-4c87-b136-f858a5e9a3e9" />

3. Aktivasyon için Github Kullanıcı Adınızı Bağlayın
   
   <img width="507" alt="Xnip2025-01-14_00-45-09" src="https://github.com/user-attachments/assets/79d5fd6f-2a08-4876-a2fe-b656f925330b" />

4. Başarılı aktivasyondan sonra Github bildirimlerinizde bir davet alacaksınız. AI Launcher kod deposuna katılmak için tıklayın.

## Proje Kodunu Klonlama

1. AI Launcher Kod Deposuna Erişim (üye değilseniz 404 gösterir)
   
   [https://github.com/monosusan/ai-launcher-code-template](https://github.com/monosusan/ai-launcher-code-template)

2. Git klonlamayı seçin veya kaynak kodu doğrudan yerel bilgisayarınıza indirin

   <img width="918" alt="image" src="https://github.com/user-attachments/assets/080f1d93-c08d-4360-a9c4-012683a45bee" />

## Proje Kurulumu

1. Proje ana dizinine gidin
   
   ```bash
   cd ai-launcher-code-template
   ```

2. Proje bağımlılıklarını yükleyin

   ```bash
   pnpm install
   ```

## Geliştirme ve Hata Ayıklama

1. Ortam değişkenleri yapılandırma dosyasını kopyalayın

   ```bash
   cp .env.example .env.development
   ```

2. Geliştirme sunucusunu başlatın

   ```bash
   pnpm dev
   ```

3. Yerel Önizleme
   
   Projeyi görüntülemek için tarayıcınızda [http://localhost:3000](http://localhost:3000/) adresini açın

   <img width="1345" alt="image" src="https://github.com/user-attachments/assets/c6419f32-d296-4f71-bdc6-67cbfa5f0c9a" />

## Özelleştirme

### Web Sitesi Renklerini Değiştirme

1. shadcn tema hata ayıklayıcısını seçin
   * [shadcn themes](https://ui.shadcn.com/themes)
   * [shadcn-ui-theme-generator](https://zippystarter.com/tools/shadcn-ui-theme-generator)

2. Projeniz için bir renk şeması oluşturun

![image](https://github.com/user-attachments/assets/76f95a54-3fc9-4d72-b9ae-e6ae4f2ce1f3)

3. Tema stillerini kopyalayın ve proje dosyalarınıza yapıştırın

<img width="770" alt="image" src="https://github.com/user-attachments/assets/25ce525e-9a16-4066-a695-f5ed824d8ab4" />

4. Özel temanızı görmek için proje önizleme sayfasını yenileyin

### Ana Sayfa İçeriğini Değiştirme

1. Ana sayfa içerik dosyasını açın ve yeni içerik oluşturmak için AI'yı kullanın

<img width="1756" alt="image" src="https://github.com/user-attachments/assets/7b12d54b-2b81-4945-b025-97eda51c4506" />

2. AI tarafından oluşturulan içeriği uygulayın, manuel düzeltmeler yapın ve yeni ana sayfayı önizleyin
3. Web sitesi içeriğini projenize uyarlamak için diğer JSON dosyalarını düzenlemeye devam edin

### Çok Dilli Metni Değiştirme

Dizinde sayfa içeriğini dosyalar aracılığıyla yapılandırın. Çince ve İngilizce varsayılan olarak desteklenir. Yayına almadan önce metni projenize uyarlayın.

<img width="1100" alt="image" src="https://github.com/user-attachments/assets/fc15d407-8b96-4756-aa2f-c4bb58954471" />

İçerik oluşturmak için AI'yı kullanabilirsiniz.

### Web Sitesi Politikalarını Değiştirme

Web sitenizi resmi olarak başlatmadan önce, site hizmetlerinize göre web sitesi politikalarını güncelleyin.

1. Gizlilik Politikasını Güncelleme
   
   Windsurf'te yeni gizlilik politikası içeriği oluşturmak için promptu kullanın.
   
   ```
   update privacy-policy according to landing page content @en.json
   with brand name "AILauncher", domain "ai-startups.uk", contact email is "contact@ai-startups.uk"
   ```
   
   Gizlilik politikasını güncellemek için dosya içeriğini değiştirin.

2. Hizmet Şartlarını Güncelleme
   
   Windsurf'te yeni hizmet şartları içeriği oluşturmak için promptu kullanın.

   ```
   update terms-of-service according to landing page content @en.json
   with brand name "AILauncher", domain "ai-startups.uk", contact email is "contact@ai-startups.uk"
   ```
   
   Hizmet şartlarını güncellemek için dosya içeriğini değiştirin.

## Ortam Değişkenlerini Değiştirme

Veri depolama/giriş/analitik/ödeme ve diğer özellikleri etkinleştirmek için ortam değişkenlerini gerçek ihtiyaçlarınıza göre değiştirin

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

## Dağıtım

1. Bir Github deposu oluşturun

2. Özelleştirilmiş proje kodunuzu Github deposuna commit edin

3. Vercel konsolunda yeni bir proje oluşturun, kod deposunu içe aktarın ve tek tıklamayla dağıtın

<img width="685" alt="image" src="https://github.com/user-attachments/assets/3baf7b2c-ad94-4022-b391-26ebb6df14dc" />

4. Vercel konsolunda ortam değişkenlerini yapılandırın
   
   <img width="1241" alt="image" src="https://github.com/user-attachments/assets/5c0e0252-0e1d-4bc9-8012-f5e122b0d7f8" />

5. Resmi web sitesini başlatın

