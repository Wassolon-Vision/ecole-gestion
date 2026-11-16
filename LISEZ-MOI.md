# Application de gestion de l'école – mise en ligne

Cette application tourne sur **GitHub Pages** (affichage) et **Firebase** (données et connexions).

## 1. Relier l'application à Firebase
1. Ouvrez le fichier `firebase-config.js`.
2. Remplacez chaque `COLLER_ICI` par la valeur du bloc **firebaseConfig** de votre projet Firebase
   (Firebase > Paramètres du projet > Vos applications).

## 2. Publier les règles de sécurité
1. Dans Firebase, ouvrez **Firestore Database > Règles**.
2. Effacez le contenu, collez tout le fichier `firestore.rules`, puis touchez **Publier**.

## 3. Mettre les fichiers sur GitHub
1. Ouvrez votre dépôt `ecole-wassolon` sur github.com.
2. Touchez **Add file > Upload files**.
3. Envoyez `index.html` et `firebase-config.js` (pas besoin d'envoyer `firestore.rules` ni ce fichier).
4. Touchez **Commit changes**.

## 4. Activer GitHub Pages
1. Dans le dépôt : **Settings > Pages**.
2. Source : **Deploy from a branch**, branche **main**, dossier **/ (root)**, puis **Save**.
3. Après 1 à 2 minutes, l'adresse est : `https://VOTRE-NOM.github.io/ecole-wassolon/`

## 5. Première utilisation
Ouvrez l'adresse, puis créez l'école et le compte de la direction **tout de suite**
(le premier à le faire devient la direction). Ensuite, la direction peut créer les élèves
(le matricule et le code du parent sont créés automatiquement) et les comptes du personnel.

## À savoir
- Les parents et les élèves se connectent avec le **matricule** et le **code**. Le personnel, avec le **téléphone** et le **mot de passe**.
- La direction peut revoir un code avec le bouton « Code » ou « Mot de passe ».
- Si le message « auth/unauthorized-domain » apparaît : Firebase > Authentication > Paramètres > Domaines autorisés, ajoutez `VOTRE-NOM.github.io`.
- Les photos des élèves, les notes, les frais, l'appel, etc. seront ajoutés module par module.
