# Introduction à git
![logo-git](git-logo_1.png)

## Git : Prise en main d'un système de gestion de versions

Git est un système de gestion de versions qui offre de nombreux avantages :

1. **Revenir en arrière en cas de problème** : Git permet de revenir en arrière si l'on casse notre code, ce qui est essentiel pour maintenir la stabilité d'un projet.

2. **Points de versions fonctionnels** : Il nous offre la possibilité de créer des points de versions stables qui fonctionnent correctement.

3. **Sérénité pour les tests** : Il offre une tranquillité d'esprit lors des tests du code, car on n'a pas à craindre de tout casser sans moyen de retour en arrière.

4. **Éviter les envois de Zip** : Git permet d'éviter l'envoi de fichiers compressés par email. On peut plutôt partager le code via GitHub en utilisant le lien du dépôt (Repo).

5. **Fusionner avec git merge** : Git permet de fusionner des branches, ce qui est essentiel pour travailler à plusieurs sur le même projet.

6. **Travailler sur plusieurs versions simultanément** : Git facilite le travail sur plusieurs versions en même temps. Par exemple, on peut avoir les branches "main", "dev", "v2", etc.

7. **Systèmes de gestion de versions antérieurs** : Avant Git, d'autres types de systèmes de gestion de versions existaient, notamment les systèmes centralisés et les systèmes distribués.

8. **Systèmes centralisés** : Ces systèmes sont basés sur un serveur central qui stocke le code source. Tous les utilisateurs travaillent directement sur ce serveur.

9. **Systèmes distribués** : Git est un système distribué, ce qui signifie que chaque personne a une copie du code source sur son propre ordinateur en local. Cela permet de faire des brouillons en local sans envoyer de modifications directement sur la version en ligne.

10. **Modifier l'historique localement** : Avec Git, vous avez la possibilité de modifier l'historique localement avant de le publier sur le serveur. Cela offre une flexibilité précieuse dans la gestion des versions.

11. **Distribué mais pas décentralisé** : Il est important de noter que Git est distribué, mais pas décentralisé, car il n'y a pas de point central unique de contrôle, mais chaque utilisateur a sa propre copie du dépôt.

## Créer son projet git de 0
Dans un premier temps, nous devons installer git avec la commande `sudo apt install git-all` pour une distribution basé sur Debian. Pour les autres OS vous pouvez voir en détail ce qu'il faut faire sur [__ce lien__](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git).

Maintenant que git est installé sur notre machine Nous allons créer un repo git. Pour cela nous pouvons passer par l'interface sur github.com et cliquer sur le "+" puis sur "New repository". 
Mais on peut également le faire via une commande : `git init`.

Maintenant que votre dossier git est initialisé, vous pouvez commencer à travailler sur le projet concerné. Pour cela, à chaque modification que vous pensez un minimum importante, vous pouvez effectuer différentes commandes. Pour voir quels fichiers ont été modifiés et si ils sont en attente d'être commité, vous pouvez faire un `git status`. Avec le retour qu'envoie cette commande, vous pouvez choisir de commiter tout les fichiers avec `git add .` (le . équivaut à tous les fichiers) ou alors vous pouvez choisir d'ajouter que certains fichier avec `git add example.py`. A partir de là, tout les fichiers ajouté seront associé au commit que vous allez réaliser avec `git commit -m "message du commit`.


## Comment récuperer un projet git
- `git clone <urlrepo.git>` : Récupérer un projet git pour travailler desssus.

### Initialisation du dépôt
- `git init` : Initialise un dépôt Git.

### Surveillance de l'état
- `git status` : Consulte l'état de l'espace de travail.

### Gestion des modifications
- `git add .` : Ajoute des modifications à la zone d'attente.
- `git commit -m "message du commit"` : Enregistre les modifications en attente dans un commit.

### Historique
- `git log` : Affiche l'historique des versions.
- `git log --all --graph` : Avoir une représentation graphique de nos branches et fusion de branche.

### Comparaison des modifications
- `git diff` : Voir le dernier titre du commit
- `git show [commit_hash]` : Affiche les modifications d'un commit donné.

### Gestion des fichiers
- `.gitignore` : Ignore des fichiers en les répertoriant dans ce fichier.

### Interaction avec le serveur
- `git push` : Pousse les nouveautés du dépôt local vers le serveur.
- `git pull` : Reçoit les nouveautés du serveur sur le dépôt local.

## Branches de travail :

### Création et navigation de branches
- `git checkout -b <branch_name>` : Crée une branche avec le nom spécifié.
- `git checkout <branch_name>` : Bascule d'une branche à l'autre.

### Affichage des branches
- `git branch` : Affiche les branches existantes.

### Fusion de branches
- `git merge <branch_name>` : Fusionne la branche spécifiée dans la branche actuelle.

### Suppression de branches
- `git branch -D <nom_branche_a_suppr>` : Supprime une branche inutile.

### Restauration et nettoyage
- `git restore .` : Revenir au dernier commit
- `git clean . -f` : Revenir au dernier commit et supprime les fichiers.

### Gestion des modifications en réserve
- `git stash` : Met de côté une partie des modifications.
- `git stash pop` : Réaffiche ce qui avait été mis de côté.
- `git stash list` : Visualise les changements en réserve.

### Modification des commits
- `git commit --amend` : Corriger un commit dans lequel on a oublé d'embarquer des changements
- `git reset <id>` : Supprimer l'historique commit que je ne souhaite plus. 




**Groupe** : Gino, Antoine, Nathan, Ewen.