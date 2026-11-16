# Mon reste — version 3

Ce que je peux vraiment dépenser jusqu'à la prochaine paie, sur tous mes comptes.

## Ce qui change

- **4 comptes** suivis (compte courant, Revolut, LDD, Livret A), renommables, avec un objectif possible sur les livrets.
- Un seul bouton **+** pour noter une **dépense**, une **rentrée** ou un **virement entre comptes**.
- Chaque compte a un solde qui suit tes opérations. **Recaler** = recopier le vrai solde de la banque quand tu veux remettre les compteurs justes.
- Ce qui revient chaque mois (**Prévu › Récurrents**) passe tout seul le lendemain de sa date.
- **Historique** par période de paie, modifiable, avec le total par catégorie.

## Mettre à jour le site (2 fichiers)

Sur github.com, dépôt `mon-reste` › **Add file › Upload files** › glisse `index.html` et `sw.js` › **Commit changes**.
Les icônes et `manifest.webmanifest` n'ont pas changé.

Avant, garde une copie de ton `index.html` actuel (bouton **Download raw file** sur GitHub) : c'est ton retour arrière.

Sur l'iPhone et le PC, ouvre l'appli avec du réseau : la nouvelle version arrive toute seule.

## Tes données

- Elles sont **reprises automatiquement** à la première ouverture : tes lignes mensuelles deviennent des récurrents, tes notes des opérations, tes rappels restent des rappels.
- Les données de l'ancienne version **ne sont ni modifiées ni supprimées** (sur l'appareil comme dans le gist de synchro).
- **Retour arrière** : remets l'ancien `index.html` sur GitHub. Tu retrouves l'appli d'avant, dans l'état où tu l'avais laissée. Ce que tu auras saisi dans la version 3 n'y apparaîtra pas.
- À faire une fois : indiquer le solde de tes livrets, et vérifier dans **Prévu › Récurrents** que chaque virement d'épargne arrive sur le bon compte.

## Synchro PC + iPhone

Rien à refaire : le jeton et la phrase secrète sont repris. La version 3 écrit dans un nouveau fichier du même gist secret.

Première mise en place (si la synchro n'était pas activée) :

1. Crée un jeton GitHub : github.com › ta photo › Settings › Developer settings ›
   Personal access tokens › Tokens (classic) › Generate new token (classic).
   Note « Mon reste », Expiration « No expiration », coche **uniquement « gist »**. Copie le code `ghp_…`.
2. Sur le PC : Réglages › Synchroniser mes appareils › colle le jeton, choisis une phrase secrète › Activer la synchro.
3. Sur l'iPhone (depuis l'icône) : même jeton, **même phrase secrète**.

Tes données sont chiffrées sur l'appareil avant d'être envoyées : GitHub ne voit que du charabia.
Si tu oublies la phrase secrète, personne ne peut la retrouver (les données de chaque appareil restent intactes).

## Sur l'iPhone

Ouvre l'adresse dans **Safari** › **Partager** › **Sur l'écran d'accueil**.
Utilise-la toujours depuis cette icône : c'est là que tes données sont gardées.

## Sauvegarde

Réglages › **Copier ma sauvegarde**, à coller dans tes Notes de temps en temps. **Restaurer** accepte aussi une sauvegarde de l'ancienne version.

## Mises à jour suivantes

Remplace `index.html`, et change le numéro de `VERSION` dans `sw.js` (`mon-reste-v20` → `mon-reste-v21`).
