# Mon reste

Ce que je peux vraiment dépenser jusqu'à la prochaine paie.

## Mettre en ligne avec GitHub Pages (une seule fois, ~5 min)

1. Sur github.com : **New repository** › nom `mon-reste` › **Public** › Create.
2. **Add file › Upload files** : glisse tous les fichiers de ce dossier (index.html, manifest.webmanifest, sw.js, les 3 icônes). **Commit changes**.
3. **Settings › Pages** › Source : *Deploy from a branch* › Branch : `main` / `(root)` › **Save**.
4. Après 1 à 2 minutes, l'adresse s'affiche : `https://sabrina97490.github.io/mon-reste/`

Le code est public, mais **aucun de tes chiffres n'y est** : ils restent dans le téléphone ou l'ordinateur qui ouvre la page.

## Sur l'iPhone

Ouvre l'adresse dans **Safari** › bouton **Partager** › **Sur l'écran d'accueil**.
Utilise-la toujours depuis cette icône : c'est là que tes données sont gardées.

## Mettre à jour plus tard

Remplace `index.html` dans le dépôt (Add file › Upload files), et change `mon-reste-v1` en `mon-reste-v2` dans `sw.js`.
Tes données ne sont pas touchées.

## Sauvegarde

Réglages › **Copier ma sauvegarde**, à coller dans tes Notes de temps en temps.

## Synchroniser le PC et l'iPhone

1. Crée un jeton GitHub (une seule fois) : github.com › ta photo › Settings › Developer settings ›
   Personal access tokens › Tokens (classic) › Generate new token (classic).
   Note « Mon reste », Expiration « No expiration », coche **uniquement « gist »**. Copie le code `ghp_…`.
2. **D'abord sur le PC** (là où sont tes données) : Mon reste › Réglages › Synchroniser mes appareils ›
   colle le jeton, choisis une phrase secrète › Activer la synchro.
3. **Puis sur l'iPhone** (depuis l'icône) : même jeton, **même phrase secrète** › Activer la synchro.
   Tout arrive tout seul.

Tes données sont chiffrées sur l'appareil avant d'être envoyées dans un gist secret : GitHub ne voit que du charabia.
Si tu oublies la phrase secrète, personne ne peut la retrouver (les données de chaque appareil restent intactes).
