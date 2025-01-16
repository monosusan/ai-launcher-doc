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

## त्वरित शुरुआत

1. AI Launcher की आधिकारिक वेबसाइट पर खरीदें
   
   [https://ai-startups.uk/#pricing](https://ai-startups.uk/#pricing)

2. भुगतान के बाद, ऑर्डर सेंटर में प्रवेश करें
   
   [https://ai-startups.uk/my-orders](https://ai-startups.uk/my-orders)
   
   सक्रियण के लिए अपना ऑर्डर चुनें।
   <img width="1276" alt="Xnip2025-01-13_22-10-13" src="https://github.com/user-attachments/assets/04002ad8-4ad7-4c87-b136-f858a5e9a3e9" />

3. सक्रियण के लिए अपना Github उपयोगकर्ता नाम बाइंड करें
   
   <img width="507" alt="Xnip2025-01-14_00-45-09" src="https://github.com/user-attachments/assets/79d5fd6f-2a08-4876-a2fe-b656f925330b" />

4. सफल सक्रियण के बाद, आपको अपनी Github सूचनाओं में एक आमंत्रण प्राप्त होगा। AI Launcher कोड रिपॉजिटरी में शामिल होने के लिए क्लिक करें।

## प्रोजेक्ट कोड क्लोन करें

1. AI Launcher कोड रिपॉजिटरी तक पहुंचें (यदि आप शामिल नहीं हुए हैं तो 404 दिखाएगा)
   
   [https://github.com/monosusan/ai-launcher-code-template](https://github.com/monosusan/ai-launcher-code-template)

2. Git क्लोन करें या सीधे सोर्स कोड को अपने लोकल कंप्यूटर पर डाउनलोड करें

   <img width="918" alt="image" src="https://github.com/user-attachments/assets/080f1d93-c08d-4360-a9c4-012683a45bee" />

## प्रोजेक्ट इंस्टॉल करें

1. प्रोजेक्ट रूट डायरेक्टरी में नेविगेट करें
   
   ```bash
   cd ai-launcher-code-template
   ```

2. प्रोजेक्ट की डिपेंडेंसी इंस्टॉल करें

   ```bash
   pnpm install
   ```

## विकास और डीबगिंग

1. एनवायरनमेंट वैरिएबल कॉन्फ़िगरेशन फ़ाइल की कॉपी करें

   ```bash
   cp .env.example .env.development
   ```

2. डेवलपमेंट सर्वर शुरू करें

   ```bash
   pnpm dev
   ```

3. लोकल प्रीव्यू
   
   अपने प्रोजेक्ट को प्रीव्यू करने के लिए अपने ब्राउज़र में [http://localhost:3000](http://localhost:3000/) खोलें

   <img width="1345" alt="image" src="https://github.com/user-attachments/assets/c6419f32-d296-4f71-bdc6-67cbfa5f0c9a" />

## कस्टमाइजेशन

### वेबसाइट के रंग बदलें

1. shadcn थीम डिबगर चुनें
   * [shadcn themes](https://ui.shadcn.com/themes)
   * [shadcn-ui-theme-generator](https://zippystarter.com/tools/shadcn-ui-theme-generator)

2. अपने प्रोजेक्ट के लिए कलर स्कीम बनाएं

![image](https://github.com/user-attachments/assets/76f95a54-3fc9-4d72-b9ae-e6ae4f2ce1f3)

3. थीम स्टाइल को कॉपी करें और प्रोजेक्ट फाइलों में पेस्ट करें

<img width="770" alt="image" src="https://github.com/user-attachments/assets/25ce525e-9a16-4066-a695-f5ed824d8ab4" />

4. अपनी कस्टम थीम देखने के लिए प्रोजेक्ट प्रीव्यू पेज को रिफ्रेश करें

### होमपेज कंटेंट बदलें

1. होमपेज कंटेंट फाइल खोलें, नई सामग्री जनरेट करने के लिए AI का उपयोग करें

<img width="1756" alt="image" src="https://github.com/user-attachments/assets/7b12d54b-2b81-4945-b025-97eda51c4506" />

2. AI जनरेटेड कंटेंट लागू करें, मैनुअल समायोजन करें और नए होमपेज का प्रीव्यू करें
3. अन्य JSON फाइलों को समायोजित करना जारी रखें ताकि वेबसाइट की सामग्री आपके प्रोजेक्ट से मेल खाए

### बहुभाषी टेक्स्ट बदलें

डायरेक्टरी में, फाइलों के माध्यम से पेज कंटेंट कॉन्फ़िगर करें। चीनी और अंग्रेजी डिफ़ॉल्ट रूप से समर्थित हैं। प्रोजेक्ट लॉन्च से पहले, टेक्स्ट को अपने प्रोजेक्ट से मेल खाने के लिए संशोधित करें।

<img width="1100" alt="image" src="https://github.com/user-attachments/assets/fc15d407-8b96-4756-aa2f-c4bb58954471" />

आप कंटेंट जनरेशन में मदद के लिए AI का उपयोग कर सकते हैं।

### वेबसाइट नीतियां बदलें

वेबसाइट को आधिकारिक तौर पर लॉन्च करने से पहले, अपनी साइट की सेवाओं के अनुसार वेबसाइट नीतियों को अपडेट करें।

1. गोपनीयता नीति अपडेट करें
   
   Windsurf में, प्रॉम्प्ट का उपयोग करके नई गोपनीयता नीति सामग्री जनरेट करें।
   
   ```
   update privacy-policy according to landing page content @en.json
   with brand name "AILauncher", domain "ai-startups.uk", contact email is "contact@ai-startups.uk"
   ```
   
   गोपनीयता नीति अपडेट करने के लिए फाइल की सामग्री को बदलें।

2. सेवा की शर्तें अपडेट करें
   
   Windsurf में, प्रॉम्प्ट का उपयोग करके नई सेवा शर्तों की सामग्री जनरेट करें।

   ```
   update terms-of-service according to landing page content @en.json
   with brand name "AILauncher", domain "ai-startups.uk", contact email is "contact@ai-startups.uk"
   ```
   
   सेवा की शर्तें अपडेट करने के लिए फाइल की सामग्री को बदलें।

## एनवायरनमेंट वैरिएबल बदलें

डेटा स्टोरेज / लॉगिन / एनालिटिक्स / भुगतान और अन्य सुविधाओं को सक्षम करने के लिए वास्तविक आवश्यकताओं के अनुसार एनवायरनमेंट वैरिएबल को संशोधित करें

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

## डिप्लॉयमेंट

1. Github रिपॉजिटरी बनाएं

2. संशोधित प्रोजेक्ट कोड को Github रिपॉजिटरी में कमिट करें

3. Vercel कंसोल में नया प्रोजेक्ट बनाएं, कोड रिपॉजिटरी को इम्पोर्ट करें और वन-क्लिक डिप्लॉय करें

   <img width="685" alt="image" src="https://github.com/user-attachments/assets/3baf7b2c-ad94-4022-b391-26ebb6df14dc" />

4. बिल्ड पूरा होने के बाद, आप Vercel कंसोल में अपना प्रोजेक्ट देख सकेंगे

   <img width="1241" alt="image" src="https://github.com/user-attachments/assets/5c0e0252-0e1d-4bc9-8012-f5e122b0d7f8" />

5. अपने प्रोजेक्ट तक पहुंचने के लिए डोमेन नाम खोलें