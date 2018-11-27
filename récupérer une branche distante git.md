La première chose que l’on me demande de faire est de récupérer le code du projet. Notre projet est hébergé sur Github, j’ai les accès en lecture et en écriture au dépôt distant du code (dépot distant intitulé par défaut origin)

$ git clone git@github.com:okiwi/atbdx.git atbdx
Cloning into 'atbdx'...

Je viens de récupérer la branche principale du projet (commande: clone) sur mon poste et j’ai mis mon environnement de travail dans le dossier atbdx. Une seule branche a été clonée, la branche principale (par défaut cette branche s’appelle master). Pour voir l’ensemble des branches du projet, vous pouvez tapper la commande suivante

$ git branch
* master

git branch m’indique que je n’ai sur mon poste en local qu’une seule branche intitulé master. 
Par défaut clone ne copie pas toutes les branches sur mon poste. Je dois lui préciser de récupérer une branche particulière depuis le dépôt distant.

$ git checkout -b dev origin/dev

Branch dev set up to track remote branch dev from origin.
Switched to a new branch 'dev'

$ git branch
* dev*
* master

git checkout -b dev origin/dev : créé moi une nouvelle branche locale intitulé dev qui est une copie d’une branche distante du dépôt origin. Et place toi sur cette branche.
