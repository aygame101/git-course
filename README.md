# git-course
## Prise de notes
Git : prise en main d'un système de gestion de versions

Permet de revenir en arrière si on casse notre code.
Avoir des points de versions qui foncitonne.
Permet d'avoir une sérénité d'esprit pour tester du code sans avoir peur de tout casser sans pouvoir revenir en arrière.

Eviter de s'envoyer des Zip avec le code, on peut passer directement par github et l'envoyer via le lien du Repo.

git merge : fusionner, pour travailler à plusieurs sur le meme projet.

Permet de travailler sur plusieurs versions en même temps. Exemple classique : main, dev, v2.

D'autres version control system (système de gestion de versions) ont existé avant :
Les systèmes centralisés et
Les systèmes distribués : Permet d'avoir une zone intermédiraire en local. Faire des brouillons en local sans envoyer sur la version en ligne.

Git est un système distribué car chaque personne a une copie sur son ordi en local.
Possibilité de modifier son historique localement avant de le publier sur le serveur.
Distribué mais pas décentralisé.

Git :
- Gérer du texte
- Agnostique vis à vis du langage
- Sauvegarde de l'historique des versions
- Aide à la résolution des conflits entre versions parallèles
- Aide au passage d'une version à l'autre

Possibilité d'installer GitHub Desktop si on veut une interface graphique mais cela n'inclu pas forcémenent l'ensemble des fonctions de Git.

Fonctions principales :
`git init` : Initialiser un dépot git
`git status` : Consulter l'état de l'espace de travail

`git add` : Ajouter des modifications à la zone d'attente
`git commit` : Enregistrer les modifications en attente dans un commit (-m "message du commit").

`git log` : Afficher l'historique des versions
`git diff` : Affficher les modifications en cours
`git show` : Afficher les modifications d'un commit donné

`.gitignore`: Ignorer des fichiers en mettant leur nom dans ce fichier.

`git push` : pousser les nouveautés du dépôt locl vers le serveur.
`git pull` : Recevoir les nouveautés du serveur sur le dépôt local.

Branche de travail : 
- Permet de préserver le contenu de la branche principale en attendant de valider le contenu de la branche de travail.
- Les branches de travail oeuvent aussi être synchronisées avec le serveur.

`git checkout -b <branch_name>` : Créer une branche avec le nom contenu dans <branch_name>.
`git checkout <branch_name>` : Basculer d'une branche à l'autre.
`git branch` : Afficher les branches existantes.