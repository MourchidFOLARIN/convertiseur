# Contribuer au Convertisseur Universel

Merci de vouloir améliorer le projet ! Toute contribution est la bienvenue : nouvel encodage, amélioration de l'analyseur, correction de bug, design, traduction.

## Démarrer

1. **Forkez** le dépôt depuis GitHub.
2. **Clonez** votre fork :
   ```bash
   git clone https://github.com/<votre-pseudo>/convertiseur.git
   cd convertiseur
   ```
3. Créez une branche :
   ```bash
   git checkout -b feature/mon-amelioration
   ```
4. Ouvrez simplement `index.html` dans votre navigateur : aucune installation, aucune dépendance.

## Ajouter un encodage

Chaque format est une entrée du tableau `ENCODINGS` dans `index.html` avec une fonction `encode` (texte → format) et `decode` (format → texte). Pour qu'il soit aussi reconnu automatiquement, ajoutez un détecteur dans l'analyseur intelligent.

## Proposer vos changements

1. Testez l'aller-retour encode/décode avec un texte simple et un texte accentué.
2. Commitez avec un message clair : `git commit -m "Ajout de l'encodage XYZ"`.
3. Poussez votre branche et ouvrez une **Pull Request** en décrivant ce que vous avez changé.

## Règles

- Le projet reste **un seul fichier**, **sans dépendance** et **hors ligne**.
- Tout texte affiché doit être échappé (pas de XSS).
- Interface en français.

Une idée sans le temps de la coder ? Ouvrez une **issue** !
