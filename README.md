# Introduction à git
## Comment récuperer un projet git
- `git clone <urlrepo.git>` : Récupérer un projet git pour travailler desssus.

&nbsp;
 
## Partie 1 : Fonctions principales

### Initialisation du dépôt
- `git init` : Initialise un dépôt Git.

### Surveillance de l'état
- `git status` : Consulte l'état de l'espace de travail.

### Gestion des modifications
- `git add .` : Ajoute des modifications à la zone d'attente.
- `git commit -m "message du commit"` : Enregistre les modifications en attente dans un commit.

### Historique
- `git log` : Affiche l'historique des versions.

### Comparaison des modifications
- `git diff` : Affiche les modifications en cours.
- `git show [commit_hash]` : Affiche les modifications d'un commit donné.

### Gestion des fichiers
- `.gitignore` : Ignore des fichiers en les répertoriant dans ce fichier.

### Interaction avec le serveur
- `git push` : Pousse les nouveautés du dépôt local vers le serveur.
- `git pull` : Reçoit les nouveautés du serveur sur le dépôt local.

&nbsp;

# Partie 2 : Branches de travail

### Création et navigation de branches
- `git checkout -b <branch_name>` : Crée une branche avec le nom spécifié.
- `git checkout <branch_name>` : Bascule d'une branche à l'autre.

### Affichage des branches
- `git branch` : Affiche les branches existantes.

### Fusion de branches
- `git merge <branch_name>` : Fusionne la branche spécifiée dans la branche actuelle.
- `git log --all --graph` : Représentation graphique des branches et de la fusion.

### Suppression de branches
- `git branch -D <nom_branche_a_suppr>` : Supprime une branche inutile.

### Restauration et nettoyage
- `git restore .` : Revient au dernier commit sur tous les fichiers.
- `git clean . -f` : Supprime les fichiers non conformes au dernier commit.

### Gestion des modifications en réserve
- `git stash` : Met de côté une partie des modifications.
- `git stash pop` : Réaffiche ce qui avait été mis de côté.
- `git stash list` : Visualise les changements en réserve.

### Modification des commits
- `git commit --amend` : Ajoute ou corrige de nouvelles modifications au dernier commit.
- `git reset <id>` : Conserve le code actuel tout en supprimant des commits superflus.

Groupe : Gino, Antoine, Nathan, Ewen.