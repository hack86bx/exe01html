# création d'un dépôt GIT

## création d'un dépôt GIT en local 

dans la console, initialisation du dépôt :

````bash
git init 
´´´´
ceci crée un dossier caché nommé .git qui contient tout l historique du projet
## visualisation de l'état de GIT

````bash
git status````

### pour voir les fichiers et dossiers unix 

````bash
ls -a
````

## pour ajouter un fichier à la futur sauvegarde 

````bash
git add README.md
````
## pour effectuer la sauvegarde 

les fichiers en attentes de sauvegarde sont en vert >
les fichiers non suivi en rouge.
seul les fichiers en **staging** seront sauvés 
````bash
git commut -m"message du commit"
````
un commit est une sauvegarde, on peut y accèder avec un `git log`( affichage des identifiants des sauvegardes et `git show` ( sans paramètre, affichage du derniet commit ) 

##pour ajouter tous les fichiers en staging

````bash git add .
````
## ajouté retirer un fichier staging
````bash
git restore --staged README.md
````
le fichier 

## ajout d'un serveur

nous allons utulisier un dépot que l'on va créer sur github.com
après connexion. comme c'est un travail personnel, son URL sera de ce type 
https://github.com/votre_username/lenomduprojet

nous créons un new Repository, puis nous copions la clefs SSH : 

git@github.com:hack86bx/exe01html.git
nous retournous dans notre console : 
````bash
git remote add origin URL/.git
git remote git@github.com:hack86bx/exe01html.git
````
pour voir si ça à fonctionné :

````bash 
git remote -v
````
