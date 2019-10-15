Liste des étapes du création du projet:

1) Création d'un dossier projet.
	mkdir Demonstration-git
2) Aller dans le dossier Demonstration-git.
	cd Demonstration-git
3) Initialisation du projet en git.
	git init
	git config --global user.name "Florent"
4) Création d'un premier fichier readme.md
	touch readme.md
	git add "readme.md"
	git commit -m "Ajout du fichier readme.md"
5) Insertion du fichier html dans le projet.
	git add "*.html"
	git commit -m "Ajout du fichier index.html"
6) Création d'un répertoire sur GitHub et ajout des collaborateurs du projet.
7) Envoyer son projet Git sur GitHub.
	git remote add origin "Lien vers le répertoire GitHub" (ici: https://github.com/Flolpb/Demonstration-git.git)
	git push origin master
8)La deuxième personne récupère le projet
	git clone "Lien vers le répertoire GitHub"  || (ici: https://github.com/Flolpb/Demonstration-git.git)
	git config --global user.name "Hervé"
9) Modification du fichier html
	git add --all
	git commit -m "Modification du fichier html"
	git push origin master
10) Récupération des modifications du projet à partir de la première personne
	git pull origin master
	git log