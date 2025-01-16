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

## Inicio Rápido

1. Comprar en el Sitio Web Oficial de AI Launcher
   
   [https://ai-startups.uk/#pricing](https://ai-startups.uk/#pricing)

2. Después del Pago, Entrar al Centro de Pedidos
   
   [https://ai-startups.uk/my-orders](https://ai-startups.uk/my-orders)
   
   Seleccione su pedido para la activación.
   <img width="1276" alt="Xnip2025-01-13_22-10-13" src="https://github.com/user-attachments/assets/04002ad8-4ad7-4c87-b136-f858a5e9a3e9" />

3. Vincular Su Nombre de Usuario de Github para la Activación
   
   <img width="507" alt="Xnip2025-01-14_00-45-09" src="https://github.com/user-attachments/assets/79d5fd6f-2a08-4876-a2fe-b656f925330b" />

4. Después de la activación exitosa, recibirá una invitación en sus notificaciones de Github. Haga clic para unirse al repositorio de código de AI Launcher.

## Clonar el Código del Proyecto

1. Acceder al Repositorio de Código de AI Launcher (mostrará 404 si no se ha unido)
   
   [https://github.com/monosusan/ai-launcher-code-template](https://github.com/monosusan/ai-launcher-code-template)

2. Elija Clonar Git o Descargar Directamente el Código Fuente a su Computadora Local

   <img width="918" alt="image" src="https://github.com/user-attachments/assets/080f1d93-c08d-4360-a9c4-012683a45bee" />

## Instalar el Proyecto

1. Navegar al Directorio Raíz del Proyecto
   
   ```bash
   cd ai-launcher-code-template
   ```

2. Instalar las Dependencias del Proyecto

   ```bash
   pnpm install
   ```

## Desarrollo y Depuración

1. Copiar el Archivo de Configuración de Variables de Entorno

   ```bash
   cp .env.example .env.development
   ```

2. Iniciar el Servidor de Desarrollo

   ```bash
   pnpm dev
   ```

3. Vista Previa Local
   
   Abra [http://localhost:3000](http://localhost:3000/) en su navegador para previsualizar su proyecto

   <img width="1345" alt="image" src="https://github.com/user-attachments/assets/c6419f32-d296-4f71-bdc6-67cbfa5f0c9a" />

## Personalización

### Modificar los Colores del Sitio Web

1. Elegir un Depurador de Temas shadcn
   * [shadcn themes](https://ui.shadcn.com/themes)
   * [shadcn-ui-theme-generator](https://zippystarter.com/tools/shadcn-ui-theme-generator)

2. Crear un Esquema de Colores para su Proyecto

![image](https://github.com/user-attachments/assets/76f95a54-3fc9-4d72-b9ae-e6ae4f2ce1f3)

3. Copiar los Estilos del Tema y Pegarlos en los Archivos del Proyecto

<img width="770" alt="image" src="https://github.com/user-attachments/assets/25ce525e-9a16-4066-a695-f5ed824d8ab4" />

4. Actualizar la Página de Vista Previa del Proyecto para Ver su Tema Personalizado

### Modificar el Contenido de la Página de Inicio

1. Abrir el Archivo de Contenido de la Página de Inicio, Usar IA para Generar Nuevo Contenido

<img width="1756" alt="image" src="https://github.com/user-attachments/assets/7b12d54b-2b81-4945-b025-97eda51c4506" />

2. Aplicar el Contenido Generado por IA, Realizar Ajustes Manuales y Previsualizar la Nueva Página de Inicio
3. Continuar Ajustando Otros Archivos JSON para que el Contenido del Sitio Web Coincida con su Proyecto

### Modificar Textos Multilingües

En el directorio, configure el contenido de la página a través de archivos. Chino e inglés están soportados por defecto. Antes del lanzamiento del proyecto, modifique el texto para que coincida con su proyecto.

<img width="1100" alt="image" src="https://github.com/user-attachments/assets/fc15d407-8b96-4756-aa2f-c4bb58954471" />

Puede usar IA para ayudar en la generación de contenido.

### Modificar las Políticas del Sitio Web

Antes de lanzar oficialmente el sitio web, actualice las políticas del sitio web según los servicios de su sitio.

1. Actualizar la Política de Privacidad
   
   En Windsurf, genere nuevo contenido de política de privacidad usando prompts.
   
   ```
   update privacy-policy according to landing page content @en.json
   with brand name "AILauncher", domain "ai-startups.uk", contact email is "contact@ai-startups.uk"
   ```
   
   Reemplace el contenido del archivo para actualizar la política de privacidad.

2. Actualizar los Términos de Servicio
   
   En Windsurf, genere nuevo contenido de términos de servicio usando prompts.

   ```
   update terms-of-service according to landing page content @en.json
   with brand name "AILauncher", domain "ai-startups.uk", contact email is "contact@ai-startups.uk"
   ```
   
   Reemplace el contenido del archivo para actualizar los términos de servicio.

## Modificar Variables de Entorno

Modifique las variables de entorno según las necesidades reales para habilitar el almacenamiento de datos / inicio de sesión / análisis / pago y otras características

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

## Despliegue

1. Crear un Repositorio Github

2. Confirmar el Código del Proyecto Modificado al Repositorio Github

3. Crear un Nuevo Proyecto en la Consola de Vercel, Importar el Repositorio de Código y Desplegar con un Clic

   <img width="685" alt="image" src="https://github.com/user-attachments/assets/3baf7b2c-ad94-4022-b391-26ebb6df14dc" />

4. Después de que la Construcción esté Completa, Podrá Ver su Proyecto en la Consola de Vercel

   <img width="1241" alt="image" src="https://github.com/user-attachments/assets/5c0e0252-0e1d-4bc9-8012-f5e122b0d7f8" />

5. Abrir el Nombre de Dominio para Acceder a su Proyecto