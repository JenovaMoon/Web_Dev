# Les commandes Git (git-command)
(Pour créer cette liste, je me suis aidée du site [Git](https://git-scm.com/book/fr/v1) et du repo d'[aquelito](https://gist.github.com/aquelito/8596717).)


Bonjour à toutes et à tous,
dans ce répertoire de commande Git je vais lister les commandes les plus utilisées, en tentant de les expliquer au mieux.

Pour avoir plus de commandes et des explications plus approfondies,  je vous conseille de consulter [le site de git](https://git-scm.com/book/fr/v1)

A la fin vous trouverez un petit plus pour vous simplifier la vie lorsque vous tapez vos commandes.

Ps : Je vais donner les termes en français, le plus possible mais je mettrai l'équivalent en anglais entre (), "car on code en anglais"! :p


## Commandes de Configuration

Vous permet de rentrer le nom qui va vous indentifier dans Git (Identity Name).

/--Attention!--/ C'est le nom qui sera afficher dans vos commit. Evitez donc les pseudo discutable xD.

$ git config --global user.name "votre nom"


Vous permet de rentrer l'email qui va vous indentifier dans Git (Identity Email).

$ git config --global user.email "votre adresse mail"


Git utilise votre éditeur(editor) de texte par defaut, pour la création ou l'édition des messages. Pour rentrer celui désiré, 
faites (ici l'exemple est avec sublime text).

$ git config --global core.editor subl


Outils de fusion et de différence (Diff tool)
Git a une implémentation interne de diff mais si vous les desirez, vous pouvez utiliser un outil externe.

$ git config --global merge.tool filemerge


Vous affiche la liste des configurations Git

$ git config --list


## Commandes principales

Vous affiche le status des fichiers (status). Cela vous indique ce qui se trouve dans votre dossier.

$ git status

Vous affiche les branches (branch) qui se trouve dans votre dépot (repository).

Une `*` vous indique la branche actuelle où vous vous trouvez.

$ git branch


Vous permet de créer une branche (branch).

$ git branch nom_de_ma_branch


Vous permet de changer de branche (branch).

$ git checkout nom_de_ma_branch


Pour le premier commit, on utilise "initial commit" (commite initial ou commite du début) pour bien voir que c'est le premier effectuer.

Cela le rend plus simple à reconnaitre lorsque l'on effectue un "git log".

$ git add .$ git commit - m "initial commit"


Pour les commits suivant, vous rentrez juste le nom de votre fichier et le titre de commit que vous désirez.

$ git add chemin_vers_mon_fichier
$ git commit -m "message du commit"


Vous permet d'annuler le dernier commit et les dernières modifications. 

$ git reset --hard md5_commit
$ git push --force


Vous permet de mettre à jour le dépôt local, c'est à dire (ici) Git.

$ git pull


Vous permet d'envoyer ses commits vers le dépôt distant, par exemple GitHub.


$ git push


Vous permet de supprimer un fichier du répertoire de travail et de l'index.

$ git rm nom_du_fichier


Vous permet de supprimer un fichier de l'index.

$ git rmg --cached nom_du_fichier


## Les différences

Vous affiche la différence entre le contenu du dernier commit et celui du répertoire de travail.

Cela correspond à ce qui serait commité par git commit -a.

$ git diff HEAD


Vous affiche la différence entre le contenu pointé par A et celui pointé par B.

$ git diff A B


Diff entre un dossier présent sur deux branches

$ git diff master..MA_BRANCH chemin/vers/mon_dossier



## Log

$ git log
# Affiche X derniers commits
$ git log -n X
# Affiche un ensemble de commits par date
$ git log --since=date --until=date


Affiche la représentation de l’historique à partir de HEAD (commit / branch)

$ git log --oneline --graph --decorate


Affiche la représentation de l’historique à partir d'un fichier (commit / branch)

$ git log --oneline --graph --decorate nom_du_fichier


## Pour annuler un commit de Git (soft)
Seul le commit est retiré de Git. Vos fichiers, eux restent inchangés. 
Si besoin est, vous pouvez à nouveau changer vos fichiers et refaire un commit.

Vous permet d'annuler le dernier commit effectué

$ git reset HEAD^


Pour indiquer à quel commit on souhaite revenir, il existe plusieurs notations :

* HEAD : dernier commit ;
* HEAD^ : avant-dernier commit ;
* HEAD^^ : avant-avant-dernier commit ;
* HEAD~2 : avant-avant-dernier commit (notation équivalente) ;
* d6d98923868578a7f38dea79833b56d0326fcba1 : indique un numéro de commit précis ;

## Pour annuler un commit de Git (hard)
Si vous voulez annuler votre dernier commit et les changements effectués dans les fichiers, il faut faire un reset hard.

/--Attention!--/ Cela annulera sans confirmation tout votre travail !

Pour annuler les commits et perdre tous les changements

$ git reset --hard HEAD^


Pour annuler les modifications d’un fichier avant un commit

Si vous avez modifié plusieurs fichiers mais que vous n’avez pas encore envoyé le commit et que vous voulez restaurer un fichier,
tel qu’il était au dernier commit :

$ git checkout nom_du_fichier


Pour annuler/supprimer un fichier avant un commit

Exemple : Vous ajoutez un fichier à Git avec `git add` et vous etes sur le point de le « commiter ».
MAIS, vous vous rendez compte que ce fichier est une mauvaise idée et vous voulez annuler votre `git add`.

Il est possible de retirer un fichier qui avait été ajouté pour être « commité » avec 

$ git reset HEAD -- nom_du_fichier_a_supprimer


## Alias git

Les alias vous permettent de créer des raccourcis pour les commandes que vous voulez.

Exemple : Lorsque je désire consulter le status de mon fichier j'utilise le commande "git status". 
Avec la commande 

$ git config --global alias.s status

je peux afficher le status de mon fichier en tapant tout simplement 

$ git s


## Aller plus haauuuut....euh plus loin, pardon ^^.

Le site de [Git](https://git-scm.com/book/fr/v1) qui pourra répondre à vos questions sur son utilisation.

Je vous link aussi un [cours](https://www.youtube.com/playlist?list=PLlxQJeQRaKDRBd_FazeI7gLq5wyrt7f7J) bien expliqué et assez rapide à réaliser.
