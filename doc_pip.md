# Pip
système de gestion de paquets pour installer et gérer des librairies écrites en Python.
[*instalation*](https://pip.pypa.io/en/latest/index.html) 
## Fonction
- `pip freeze` : Affiche toutes les lib installées et leur version
- `pip freeze > lib.txt` : exportez cette liste
- `pip install -r lib.txt` : importez cette liste
- `pip search lib` : recherche une librairie
- `pip show lib` : informations à propos d'un paquet précis
- `pip install lib` : installer une librarie
-	`pip list --outdated` : indique quels librairie n'est plus à jour
-	`pip install lib --upgrade` : metre a jour
-	`pip bundle bund.pybundle -r lib.txt` : zip qui contient toutes les dépendances
-	`pip install bund.pybundle` : installer les lib
-	`pip uninstall lib` : desinstal la librairie
