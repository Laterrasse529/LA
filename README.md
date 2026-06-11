# La Terrasse – Menu Digital 🍃

Menu digital mobile-first pour **La Terrasse Café & Resto**, Korba, Tunisia.

## Structure des fichiers

```
index.html   → Structure de la page
style.css    → Design (couleurs, typographie, accordéon)
script.js    → Chargement du menu + logique accordéon
logo.png     → Logo du café (à uploader)
README.md    → Ce fichier
```

---

## Déploiement sur GitHub Pages (gratuit)

1. Créez un repo GitHub public (ex: `laterrasse-menu`)
2. Uploadez tous les fichiers
3. Allez dans **Settings → Pages → Source : main branch / root**
4. Votre site sera accessible sur : `https://votre-compte.github.io/laterrasse-menu/`

---

## Connecter Google Sheets (optionnel)

Sans Google Sheets, le menu affiche des **données d'exemple** incluses dans `script.js`.

Pour utiliser votre vrai menu depuis Google Sheets :

### 1. Préparez votre feuille
Créez une feuille avec ces colonnes exactes en **ligne 1** :

| Catégorie | Catégorie_EN | Icône | Nom | Description | Prix |
|-----------|-------------|-------|-----|-------------|------|
| Cafés | Coffee | ☕ | Espresso | Café court et intense | 1.500 DT |
| Cafés | Coffee | ☕ | Cappuccino | Espresso, lait vapeur | 2.500 DT |

### 2. Publiez en CSV
`Fichier → Partager → Publier sur le Web → Format : CSV → Publier`

Copiez l'URL générée.

### 3. Collez l'URL dans script.js
Ouvrez `script.js` et remplacez :
```js
const SHEET_CSV_URL = "VOTRE_URL_GOOGLE_SHEETS_CSV_ICI";
```
par votre vraie URL.

### 4. Icônes disponibles
☕ 🍵 🫖 🍹 🥤 🧇 🥪 🍔 🥗 🍰 🍦 🍽️ 🥐 🧃 🍫

---

## Modifier les données sans Google Sheets

Éditez directement le tableau `DEFAULT_MENU` dans `script.js`.

---

## Personnalisation rapide

| Ce que vous voulez changer | Où |
|---|---|
| Numéro WhatsApp | `index.html` ligne `wa.me/yourNumber` |
| Couleur principale | `style.css` variable `--brown` |
| Adresse / Horaires | `index.html` section `.info-bar` |
| Articles du menu | `script.js` tableau `DEFAULT_MENU` |

---

**Hébergement gratuit via GitHub Pages ✓**
