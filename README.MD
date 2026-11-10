# LoreKeeper — Site vitrine

<p align="center">
  <img src="lorekeeper-logo-alpha.png" alt="Logo LoreKeeper" width="120" />
</p>

Site vitrine statique de **LoreKeeper**, l'application desktop *local-first* dédiée aux maîtres du jeu et aux joueurs de jeux de rôle (JDR) : gestion de campagnes, génération de PNJ et scénarios assistée par IA locale, et suivi de session / lancers de dés.

---

## 📋 Aperçu du contenu

La page [`index.html`](index.html) présente l'application et regroupe les sections suivantes :

- **En-tête (Hero)** : logo, présentation de LoreKeeper, boutons de téléchargement pour **macOS** et **Windows** (liens vers les *Releases* GitHub) et bouton de soutien (**Ko-fi**).
- **Fonctionnalités clés** :
  - **100% Hors-ligne** : stockage local dans une base SQLite embarquée.
  - **Assisté par IA** : génération de PNJ et de scénarios à la volée avec Ollama (Mistral).
  - **Multijoueur Local** : partage des lancers de dés et suivis de session en direct via token.
- **Mentions légales** :
  - **Conditions d'Utilisation** (`#terms`) : mise à disposition « tel quel », usage personnel ou associatif, responsabilité matérielle liée aux modèles d'IA locaux.
  - **Règles de Confidentialité** (`#privacy`) : aucune collecte ni revente de données personnelles, 100 % des données conservées localement.

---

## 🛠️ Stack technique

Le site est volontairement léger, sans étape de *build* ni dépendances à installer :

- **HTML5** (langue `fr`)
- **Tailwind CSS** chargé via CDN (`https://cdn.tailwindcss.com`)
- **Ressources statiques** : icône et logo PNG (`lorekeeper-logo-alpha.png`)

---

## 📁 Structure du projet

```text
LoreKeeper-site/
├── index.html                  # Page principale du site vitrine
├── lorekeeper-logo-alpha.png   # Logo et favicon de l'application
├── .gitignore                  # Fichiers ignorés par Git (.DS_Store)
└── README.MD                   # Documentation du dépôt
```

---

## 🚀 Prévisualisation en local

Aucune installation de paquets n'est requise. Vous pouvez :

1. **Ouvrir directement le fichier** `index.html` dans votre navigateur.
2. **Ou lancer un petit serveur HTTP local** depuis la racine du projet :

```bash
# Avec Python 3
python3 -m http.server 8080
```

Puis ouvrir [http://localhost:8080](http://localhost:8080) dans votre navigateur.

---

## ⚙️ Personnalisation avant mise en ligne

Avant de publier le site, pensez à mettre à jour les URLs *placeholder* dans [`index.html`](index.html) :

- **Liens de téléchargement (Mac & Windows)** : remplacer `https://github.com/TON-PSEUDO/lorekeeper/releases/latest` par l'URL réelle de vos *releases* (ex. `https://github.com/superfeedboy/lorekeeper/releases/latest`).
- **Lien de soutien** : remplacer `https://ko-fi.com/ton-lien` par votre page Ko-fi (ou supprimer/adapter le bouton si non utilisé).

---

## 🌐 Déploiement

S'agissant d'un site purement statique, il peut être hébergé gratuitement sur n'importe quelle plateforme statique :

- **GitHub Pages** : activer Pages sur la branche principale (`master` / `main`), dossier racine `/`.
- **Netlify / Vercel / Cloudflare Pages** : connecter le dépôt sans commande de *build* et publier le répertoire racine `.`.

---

## 📄 Licence & Crédits

© 2026 LoreKeeper — Fait avec passion pour les passionnés de JDR.
