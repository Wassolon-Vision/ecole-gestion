# Application de gestion de l'école – guide complet

## Fichiers à mettre sur GitHub (dépôt `ecole-wassolon`)
`index.html`, `manifest.json`, `sw.js`, `icon-192.png`, `icon-512.png`, `icon-maskable-512.png`
(Add file > Upload files > sélectionnez les 6 fichiers > Commit changes.)
Le fichier `firestore.rules` se colle dans Firebase, il ne va pas sur GitHub.
Les anciens fichiers `…-ecole.html`, `firebase-config.js` peuvent être supprimés du dépôt (ils ne servent plus).

## 1. Règles de sécurité (obligatoire)
Firebase > Firestore Database > Règles : effacez tout, collez le contenu de `firestore.rules`, puis Publier.

## 2. Activer GitHub Pages (une seule fois)
Dépôt > Settings > Pages > Deploy from a branch > main > / (root) > Save.
Adresse : `https://wassolon-vision.github.io/ecole-wassolon/`

## 3. Première utilisation
Ouvrez l'adresse, créez l'école et le compte de la direction tout de suite (le premier devient la direction).
Si l'école existe déjà, connectez-vous avec le téléphone et le mot de passe de la direction.

## 4. Essai sans Firebase
Ajoutez `?demo` à l'adresse. Pour revenir à Firebase : `?firebase`.
Comptes d'essai : direction 620 00 00 00 / demo123, enseignant 620 00 00 02 / demo123, parent WSF-2026-0001 / 123456.
Si l'essai montre d'anciennes données : bouton « Réinitialiser » dans le cadre de démonstration.

## 5. Installer l'application
- Android (Chrome) : touchez « 📲 Installer l'application » (page de connexion ou menu), ou menu ⋮ > « Installer l'application ».
- iPhone (Safari) : Partager > « Sur l'écran d'accueil ».
- Ordinateur (Chrome ou Edge) : icône d'installation à droite de la barre d'adresse, ou bouton « 📲 Installer l'application ».

## Qui voit quoi
- Direction : tout voir et tout modifier (élèves, classes, enseignants, notes, frais, appel, discipline, réclamations, messages, emploi du temps, comptes, paramètres, journal).
- Enseignant : consulte les élèves, classes, notes, emplois du temps ; fait l'appel ; ajoute des notes de discipline ; écrit à la direction.
- Parent ou élève (matricule + code) : bulletin, frais, absences, emploi du temps, annonces, réclamations et messages concernant son enfant.

## À savoir
- Le journal des modifications est dans Paramètres > Journal.
- La direction peut revoir un code ou un mot de passe créé par l'application (bouton « Code » ou « Mot de passe »).
- Si « auth/unauthorized-domain » apparaît : Firebase > Authentication > Paramètres > Domaines autorisés, ajoutez `wassolon-vision.github.io`.
- Photos des élèves : non incluses (le stockage de photos de Firebase est payant).
