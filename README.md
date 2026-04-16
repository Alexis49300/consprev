# FormaCRM — Version GitHub Pages

Application de suivi des dossiers de formation, en HTML pur, hébergeable gratuitement sur GitHub Pages.

## Déploiement en 2 minutes

### 1. Créer un repo GitHub

1. Allez sur [github.com](https://github.com) → **New repository**
2. Nom : `formacrm` (ou ce que vous voulez)
3. Visibilité : **Public** (requis pour GitHub Pages gratuit)
4. Cliquez **Create repository**

### 2. Uploader le fichier

**Option A — via l'interface GitHub (le plus simple) :**
1. Dans votre repo, cliquez **Add file → Upload files**
2. Glissez `index.html`
3. Cliquez **Commit changes**

**Option B — via Git :**
```bash
git init
git add index.html
git commit -m "Initial commit"
git remote add origin https://github.com/VOUS/formacrm.git
git push -u origin main
```

### 3. Activer GitHub Pages

1. Dans votre repo → **Settings → Pages**
2. Source : **Deploy from a branch**
3. Branch : **main** / **(root)**
4. Cliquez **Save**
5. Attendez 1-2 minutes → votre app est en ligne sur :
   `https://VOTRE-USERNAME.github.io/formacrm/`

---

## Fonctionnalités

- **Tableau de bord** — indicateurs, alertes, graphiques
- **Pipeline** — vue kanban par étape
- **Dossiers** — tableau filtrable complet
- **Apporteurs d'affaires** — suivi commissions

## Workflow des étapes

1. Création dossier
2. Devis & contrat — devis signé
3. Documents pré-formation — KBIS, Urssaf, DU, contrat travail, RIB, contacts, TVA, Net Entreprise
4. Formation
5. Documents post-formation — émargements, attestation entreprise, attestation Minimis, avenant contrat
6. Demande de financement — OPCO/CPF, accord, versement

## Stockage des données

Les données sont sauvegardées dans le **localStorage** du navigateur.
Elles persistent entre les sessions sur le même navigateur/appareil.

Pour sauvegarder ou partager les données, utilisez le bouton **↓ Export CSV**.

---

## Prochaine étape : synchronisation Google Sheets

Pour avoir les données partagées entre plusieurs utilisateurs,
il est possible d'ajouter une synchronisation avec Google Sheets
via Google Apps Script (sans serveur, gratuit).
