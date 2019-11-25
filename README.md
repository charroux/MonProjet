# monProjet

git clone https://github.com/charroux/monProjet

	git init
	git pull
	par défaut on est sur la branche master

4/ 

Créer un fichier => n'importe quel éditeur
git add dossier/
git commit -a -m "ajout fichier"
git push https://github.com/charroux/monProjet

5/

git branch branche1
git checkout branche1

	Travailler :
		Créer un fichier => n'importe quel éditeur
		git add dossier/
		git commit -a -m "ajout fichier"

Attention ! La branche master contient 1 fichier, la branche "branche1" en contient 2

git checkout master		=> retour sur le branche master
git merge branche1 		=> on a nos deux fichiers !

Attention aux conflits => quand on édite un même fichier dans 2 branches
	
	git checkout branche1
	édite le fichier
	git commit -a -m "modif fichier"
	git checkout master
	git merge branche1	=> fastforward => force fusion

Pousser branche sur le serveur

git push https://github.com/charroux/monProjet branche1:branche1	
		=> branche locale:branche distante

Attention git pull récupère la branche master => faire : 

git pull https://github.com/charroux/monProjet branche1:branche1	
		=> branche distante:branche locale 