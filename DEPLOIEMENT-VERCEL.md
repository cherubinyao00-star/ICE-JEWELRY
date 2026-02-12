# 🚀 Guide de Déploiement sur Vercel - ICE JEWELRY

## 📋 Avant de commencer

Vous aurez besoin de :
- ✅ Tous les fichiers du site
- ✅ Un compte Vercel (gratuit)
- ✅ Un navigateur web

---

## 🎯 Méthode 1 : Déploiement via Interface Web (RECOMMANDÉ)

### Étape 1 : Créer un compte Vercel

1. Allez sur **[vercel.com](https://vercel.com)**
2. Cliquez sur **"Sign Up"**
3. Connectez-vous avec :
   - GitHub (recommandé)
   - GitLab
   - Bitbucket
   - Ou par email

### Étape 2 : Créer un nouveau projet

1. Cliquez sur **"Add New..."** → **"Project"**
2. Choisissez **"Continue with a Git repository"** OU **"Import Third-Party Git Repository"**
3. OU cliquez sur **"Browse"** pour uploader les fichiers directement

### Étape 3 : Uploader vos fichiers

**Fichiers à uploader :**
- ✅ `index.html`
- ✅ `admin-dashboard.html`
- ✅ `clear-data.html`
- ✅ `test-storage.html`
- ✅ `vercel.json`
- ✅ `README.md`

**Vous pouvez glisser-déposer un dossier ZIP ou les fichiers individuels**

### Étape 4 : Configuration du projet

1. **Project Name** : `ice-jewelry` (ou le nom de votre choix)
2. **Framework Preset** : Laissez "Other"
3. **Root Directory** : `./` (par défaut)
4. Cliquez sur **"Deploy"**

### Étape 5 : Attendre le déploiement

- ⏱️ Le déploiement prend 30-60 secondes
- 🎉 Vous verrez une animation de confettis quand c'est terminé !

### Étape 6 : Accéder à votre site

Votre site sera accessible à :
```
https://ice-jewelry.vercel.app
```
ou
```
https://votre-projet-nom.vercel.app
```

---

## 🌐 URLs importantes

Une fois déployé, vous aurez :

- **Site principal** : `https://votre-site.vercel.app`
- **Dashboard admin** : `https://votre-site.vercel.app/admin`
- **Nettoyage données** : `https://votre-site.vercel.app/clear-data.html`
- **Test storage** : `https://votre-site.vercel.app/test-storage.html`

---

## ⚙️ Configuration post-déploiement

### 1. Changer les identifiants admin

**IMPORTANT** : Changez les identifiants par défaut !

1. Dans Vercel, allez dans votre projet
2. Cliquez sur **"Settings"** → **"Environment Variables"**
3. Ou modifiez directement le fichier `admin-dashboard.html` avant déploiement

### 2. Configurer les réseaux sociaux

1. Allez sur `https://votre-site.vercel.app/admin`
2. Connectez-vous
3. Allez dans **"⚙️ Paramètres"**
4. Remplissez :
   - 📱 Numéro WhatsApp
   - 🎵 TikTok
   - 📧 Email
   - 📞 Téléphone

### 3. Ajouter vos produits

1. Dans le dashboard, allez dans **"💎 Produits"**
2. Cliquez sur **"➕ Ajouter un produit"**
3. Remplissez les informations
4. Uploadez une photo
5. Enregistrez

---

## 🎨 Domaine personnalisé

Pour utiliser votre propre domaine (ex: `www.icejewelry.ci`) :

### Étape 1 : Acheter un domaine
- **Recommandé** : Namecheap, GoDaddy, OVH

### Étape 2 : Configurer dans Vercel

1. Allez dans **Settings** → **Domains**
2. Cliquez sur **"Add"**
3. Entrez votre domaine : `icejewelry.ci`
4. Suivez les instructions DNS

### Étape 3 : Configurer les DNS

Ajoutez ces enregistrements chez votre registrar :

```
Type    Name    Value
A       @       76.76.21.21
CNAME   www     cname.vercel-dns.com
```

⏱️ **Délai de propagation** : 24-48 heures

---

## 🔄 Mises à jour

Pour mettre à jour votre site :

### Via interface Vercel
1. Allez dans **Deployments**
2. Cliquez sur **"..."** → **"Redeploy"**

### Via upload de fichiers
1. Modifiez vos fichiers localement
2. Retournez sur Vercel
3. Uploadez les nouveaux fichiers
4. Vercel redéploie automatiquement

---

## 🛡️ Sécurité

### ⚠️ Changez IMMÉDIATEMENT ces identifiants

**Dans `admin-dashboard.html` ligne 336-337 :**
```javascript
var ADMIN_USER = 'admin';       // ← CHANGEZ ICI
var ADMIN_PASS = 'admin123';    // ← CHANGEZ ICI
```

**Conseils pour un mot de passe sécurisé :**
- ✅ Minimum 12 caractères
- ✅ Mélange de lettres, chiffres, symboles
- ✅ Pas de mots du dictionnaire
- ✅ Exemple : `IcE2026!JwL#SecuRe`

---

## 📊 Statistiques et Analytics

Pour suivre les visiteurs, ajoutez **Vercel Analytics** :

1. Dans votre projet Vercel
2. Allez dans **Analytics**
3. Cliquez sur **"Enable"**
4. C'est gratuit pour 100k événements/mois !

---

## ❓ Dépannage

### Le site ne s'affiche pas
- ✅ Vérifiez que tous les fichiers sont uploadés
- ✅ Regardez les logs dans **Deployments** → **Function Logs**
- ✅ Vérifiez `vercel.json`

### L'admin ne fonctionne pas
- ✅ Essayez : `votre-site.vercel.app/admin-dashboard.html`
- ✅ Vérifiez les identifiants
- ✅ Ouvrez la console (F12) pour voir les erreurs

### Les données ne se sauvent pas
- ✅ C'est normal ! Les données sont dans le localStorage du navigateur
- ✅ Chaque utilisateur a ses propres données
- ✅ Si vous voulez une vraie base de données, contactez-moi

---

## 💡 Conseils Pro

### Performance
- ✅ Vercel optimise automatiquement vos images
- ✅ CDN mondial gratuit
- ✅ HTTPS automatique

### Backups
- ✅ Téléchargez régulièrement vos données via `clear-data.html`
- ✅ Exportez les produits du dashboard
- ✅ Gardez une copie locale des fichiers

### Marketing
- ✅ Partagez `votre-site.vercel.app` sur TikTok
- ✅ Ajoutez le lien dans votre bio WhatsApp Business
- ✅ Créez des stories Instagram avec votre lien

---

## 🎉 Félicitations !

Votre site est maintenant en ligne et accessible à tous ! 🚀

**Prochaines étapes :**
1. ✅ Changez les identifiants admin
2. ✅ Configurez les réseaux sociaux
3. ✅ Ajoutez vos produits
4. ✅ Créez votre première annonce
5. ✅ Partagez votre site !

---

**Besoin d'aide ?**
- 📧 Support Vercel : support@vercel.com
- 📚 Documentation : vercel.com/docs
- 💬 Communauté : github.com/vercel/vercel/discussions

**© 2026 ICE JEWELRY by MOSTPE**
