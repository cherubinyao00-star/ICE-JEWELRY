# 💎 ICE JEWELRY - Site E-commerce

Site e-commerce de bijouterie avec dashboard admin complet.

## 📁 Structure du projet

```
ice-jewelry/
├── index.html              # Page principale de la boutique
├── admin-dashboard.html    # Dashboard admin
├── clear-data.html         # Page de nettoyage des données
├── test-storage.html       # Page de test localStorage
├── vercel.json            # Configuration Vercel
├── _redirects             # Redirections Netlify (optionnel)
└── README.md              # Ce fichier
```

## 🚀 Déploiement sur Vercel

### Méthode 1 : Via l'interface Vercel (Recommandé)

1. **Créez un compte sur [Vercel](https://vercel.com)**
2. Cliquez sur **"New Project"**
3. Uploadez tous les fichiers du dossier
4. Cliquez sur **"Deploy"**
5. Votre site sera en ligne en quelques secondes !

### Méthode 2 : Via Vercel CLI

```bash
# Installer Vercel CLI
npm i -g vercel

# Se connecter
vercel login

# Déployer
vercel
```

## 🔐 Accès Admin

- **URL** : `votre-site.vercel.app/admin`
- **Identifiant par défaut** : `admin`
- **Mot de passe par défaut** : `admin123`

⚠️ **Changez ces identifiants** dans `admin-dashboard.html` (lignes 336-337)

## ⚙️ Configuration

### Modifier les identifiants admin
Ouvrez `admin-dashboard.html` et trouvez :
```javascript
var ADMIN_USER = 'admin';       // ← Changez ici
var ADMIN_PASS = 'admin123';    // ← Changez ici
```

### Configurer les réseaux sociaux
1. Connectez-vous au dashboard admin
2. Allez dans **"⚙️ Paramètres"**
3. Remplissez vos informations :
   - Numéro WhatsApp
   - Nom d'utilisateur TikTok
   - Email et téléphone

## 📦 Fonctionnalités

### Site Client
- ✅ Catalogue de produits dynamique
- ✅ Panier d'achat
- ✅ Système de commande avec livraison
- ✅ Calcul automatique des frais de livraison (13 communes d'Abidjan)
- ✅ Barre d'annonces
- ✅ Liens réseaux sociaux (WhatsApp, TikTok)

### Dashboard Admin
- ✅ Gestion des commandes
- ✅ Gestion des produits (avec photos)
- ✅ Gestion des catégories
- ✅ Gestion des annonces
- ✅ Paramètres (réseaux sociaux, contact)
- ✅ Statistiques

## 💾 Stockage des données

Les données sont stockées dans le **localStorage** du navigateur :
- `iceJewelryProducts` - Produits
- `iceJewelryCategories` - Catégories
- `iceJewelryOrders` - Commandes
- `iceJewelryAnnouncements` - Annonces
- `iceJewelrySettings` - Paramètres

## 🛠️ Outils inclus

- **`clear-data.html`** - Nettoyer les données de test
- **`test-storage.html`** - Voir le contenu du localStorage

## 🌐 Domaine personnalisé

Pour utiliser votre propre domaine :
1. Allez dans **Settings** de votre projet Vercel
2. Cliquez sur **Domains**
3. Ajoutez votre domaine
4. Configurez les DNS selon les instructions

## 📞 Support

Pour toute question, contactez le développeur ou consultez la [documentation Vercel](https://vercel.com/docs).

---

**© 2026 ICE JEWELRY by MOSTPE**
