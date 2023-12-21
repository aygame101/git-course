## Fonctions principales :

- Initialise un dépôt Git : `.git init`  
- Consulte l'état de l'espace de travail : `.git status`  
- Ajoute des modifications à la zone d'attente : `git add .`  
- Enregistre les modifications en attente dans un commit (-m "message du commit") : `.git commit`  
- Affiche l'historique des versions : `.git log`  
- Affiche les modifications en cours : `.git diff` 
- Affiche les modifications d'un commit donné : `.git show` 
- Ignore des fichiers en les répertoriant dans ce fichier : `.gitignore` 
- Pousse les nouveautés du dépôt local vers le serveur : `.git push`  
- Reçoit les nouveautés du serveur sur le dépôt local : `.git pull` 


## Branche de travail :

Préserve le contenu de la branche principale en attendant la validation de la branche de travail.
Les branches de travail peuvent être synchronisées avec le serveur.

- Crée une branche avec le nom spécifié dans <branch_name> : `.git checkout -b <branch_name>`  
- Bascule d'une branche à l'autre : `.git checkout <branch_name>` 
- Affiche les branches existantes : `.git branch`  
- La fusion sur la branche principale (git merge) s'effectue en ajoutant le nom de la branche à fusionner. Pour une représentation graphique des branches et de la fusion, utilisez : `.git log --all --graph`
- Supprime une branche inutile : `.git branch -D <nom_branche_a_suppr>` 
- Revient au dernier commit sur tous les fichiers (.) : `git restore .` 
- Supprime les fichiers non conformes au dernier commit : `.git clean . -f` 
- Met de côté une partie des modifications : `.git statch` 
- Réaffiche ce qui avait été mis de côté : `.git statch pop`  
- Visualise les changements en réserve : `.git statch list` 
- Ajoute de nouvelles modifications au dernier commit : `.git commit --amend` 
- Conserve le code actuel tout en supprimant des commits superflus : `.git reset <id>` 