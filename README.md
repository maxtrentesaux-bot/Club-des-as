# Le Club des As — maquette PWA

Maquette fonctionnelle du programme de fidélisation Le Club des As (Onefaktory SASU).
Application autonome, données en mémoire, aucune base de données.

## Publier en 5 minutes (GitHub Pages)

1. Sur github.com : **New repository** → nom `club-des-as` → **Public** → Create.
2. **Add file › Upload files** → glisser tous les fichiers de ce dossier → Commit.
3. **Settings › Pages** → Source : `Deploy from a branch` → Branch : `main` / `/ (root)` → Save.
4. Attendre 1 à 2 minutes. L'adresse s'affiche :
   `https://<ton-compte>.github.io/club-des-as/`

## Installer l'icône sur le téléphone

- **iPhone (Safari obligatoire)** : ouvrir l'adresse → bouton Partager → *Sur l'écran d'accueil*.
- **Android (Chrome)** : ouvrir l'adresse → menu ⋮ → *Installer l'application*.

L'icône (écusson sur fond crème) et le nom « Club des As » apparaissent sur l'écran d'accueil.
L'appli s'ouvre en plein écran, sans barre de navigateur.

## Pourquoi HTTPS est indispensable

GitHub Pages fournit HTTPS automatiquement, ce qui débloque :
- l'appareil photo intégré avec les guides de cadrage,
- la géolocalisation du bouton SOS,
- l'installation sur l'écran d'accueil.

Ouvert en fichier local, ces trois fonctions restent inactives.

## Fichiers

| Fichier | Rôle |
|---|---|
| `index.html` | l'application complète |
| `manifest.webmanifest` | nom, couleurs et icônes de l'appli installée |
| `sw.js` | service worker : installation et fonctionnement hors connexion |
| `icon-192.png`, `icon-512.png` | icônes Android |
| `apple-touch-icon.png` | icône iPhone / iPad |
| `favicon-32.png` | icône d'onglet |

## Mise à jour

Remplacer `index.html` et incrémenter `club-des-as-v1` en `-v2` dans `sw.js`
(sinon les téléphones gardent l'ancienne version en cache).
