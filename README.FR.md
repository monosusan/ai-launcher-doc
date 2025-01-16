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

## Démarrage Rapide

1. Achat sur le Site Officiel d'AI Launcher
   
   [https://ai-startups.uk/#pricing](https://ai-startups.uk/#pricing)

2. Après le Paiement, Accéder au Centre de Commandes
   
   [https://ai-startups.uk/my-orders](https://ai-startups.uk/my-orders)
   
   Sélectionnez votre commande pour l'activation.
   <img width="1276" alt="Xnip2025-01-13_22-10-13" src="https://github.com/user-attachments/assets/04002ad8-4ad7-4c87-b136-f858a5e9a3e9" />

3. Lier Votre Nom d'Utilisateur Github pour l'Activation
   
   <img width="507" alt="Xnip2025-01-14_00-45-09" src="https://github.com/user-attachments/assets/79d5fd6f-2a08-4876-a2fe-b656f925330b" />

4. Après l'activation réussie, vous recevrez une invitation dans vos notifications Github. Cliquez pour rejoindre le dépôt de code AI Launcher.

## Cloner le Code du Projet

1. Accéder au Dépôt de Code AI Launcher (affichera 404 si vous n'avez pas rejoint)
   
   [https://github.com/monosusan/ai-launcher-code-template](https://github.com/monosusan/ai-launcher-code-template)

2. Choisissez de Cloner Git ou de Télécharger Directement le Code Source sur Votre Ordinateur Local

   <img width="918" alt="image" src="https://github.com/user-attachments/assets/080f1d93-c08d-4360-a9c4-012683a45bee" />

## Installer le Projet

1. Naviguer vers le Répertoire Racine du Projet
   
   ```bash
   cd ai-launcher-code-template
   ```

2. Installer les Dépendances du Projet

   ```bash
   pnpm install
   ```

## Développement et Débogage

1. Copier le Fichier de Configuration des Variables d'Environnement

   ```bash
   cp .env.example .env.development
   ```

2. Démarrer le Serveur de Développement

   ```bash
   pnpm dev
   ```

3. Aperçu Local
   
   Ouvrez [http://localhost:3000](http://localhost:3000/) dans votre navigateur pour prévisualiser votre projet

   <img width="1345" alt="image" src="https://github.com/user-attachments/assets/c6419f32-d296-4f71-bdc6-67cbfa5f0c9a" />

## Personnalisation

### Modifier les Couleurs du Site Web

1. Choisir un Débogueur de Thème shadcn
   * [shadcn themes](https://ui.shadcn.com/themes)
   * [shadcn-ui-theme-generator](https://zippystarter.com/tools/shadcn-ui-theme-generator)

2. Créer un Schéma de Couleurs pour Votre Projet

![image](https://github.com/user-attachments/assets/76f95a54-3fc9-4d72-b9ae-e6ae4f2ce1f3)

3. Copier les Styles du Thème et les Coller dans les Fichiers du Projet

<img width="770" alt="image" src="https://github.com/user-attachments/assets/25ce525e-9a16-4066-a695-f5ed824d8ab4" />

4. Actualiser la Page d'Aperçu du Projet pour Voir Votre Thème Personnalisé

### Modifier le Contenu de la Page d'Accueil

1. Ouvrir le Fichier de Contenu de la Page d'Accueil, Utiliser l'IA pour Générer un Nouveau Contenu

<img width="1756" alt="image" src="https://github.com/user-attachments/assets/7b12d54b-2b81-4945-b025-97eda51c4506" />

2. Appliquer le Contenu Généré par l'IA, Faire des Ajustements Manuels et Prévisualiser la Nouvelle Page d'Accueil
3. Continuer à Ajuster d'Autres Fichiers JSON pour que le Contenu du Site Web Corresponde à Votre Projet

### Modifier les Textes Multilingues

Dans le répertoire, configurez le contenu de la page via des fichiers. Le chinois et l'anglais sont pris en charge par défaut. Avant le lancement du projet, modifiez le texte pour qu'il corresponde à votre projet.

<img width="1100" alt="image" src="https://github.com/user-attachments/assets/fc15d407-8b96-4756-aa2f-c4bb58954471" />

Vous pouvez utiliser l'IA pour aider à la génération de contenu.

### Modifier les Politiques du Site Web

Avant de lancer officiellement le site web, mettez à jour les politiques du site web selon les services de votre site.

1. Mettre à Jour la Politique de Confidentialité
   
   Dans Windsurf, générez un nouveau contenu de politique de confidentialité en utilisant des prompts.
   
   ```
   update privacy-policy according to landing page content @en.json
   with brand name "AILauncher", domain "ai-startups.uk", contact email is "contact@ai-startups.uk"
   ```
   
   Remplacez le contenu du fichier pour mettre à jour la politique de confidentialité.

2. Mettre à Jour les Conditions d'Utilisation
   
   Dans Windsurf, générez un nouveau contenu des conditions d'utilisation en utilisant des prompts.

   ```
   update terms-of-service according to landing page content @en.json
   with brand name "AILauncher", domain "ai-startups.uk", contact email is "contact@ai-startups.uk"
   ```
   
   Remplacez le contenu du fichier pour mettre à jour les conditions d'utilisation.

## Modifier les Variables d'Environnement

Modifiez les variables d'environnement selon les besoins réels pour activer le stockage de données / connexion / analyse / paiement et autres fonctionnalités

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

## Déploiement

1. Créer un Dépôt Github

2. Valider le Code du Projet Modifié dans le Dépôt Github

3. Créer un Nouveau Projet dans la Console Vercel, Importer le Dépôt de Code et Déployer en Un Clic

   <img width="685" alt="image" src="https://github.com/user-attachments/assets/3baf7b2c-ad94-4022-b391-26ebb6df14dc" />

4. Une Fois la Construction Terminée, Vous Pourrez Voir Votre Projet dans la Console Vercel

   <img width="1241" alt="image" src="https://github.com/user-attachments/assets/5c0e0252-0e1d-4bc9-8012-f5e122b0d7f8" />

5. Ouvrir le Nom de Domaine pour Accéder à Votre Projet