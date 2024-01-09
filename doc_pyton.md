# Python
## Variable
### Texte
	\subsubsection{Préfix}
		\textit{R} ou \textit{r} : chaines brutes, traitent la barre oblique inversée comme un caractère normal\\
		\textit{F} ou \textit{f} : littérale formatée ; \{\} peuvent contenir des champs à remplacer
	\subsubsection{Argument}
		\textit{\textbackslash n} : saut de ligne ;\\
		\textit{\textbackslash r} : retour chariot ;\\
		\textit{\textbackslash t} : tabulation ;\\
		\textit{'''texte'''} ou \textit{"""texte""" }: Les retours à la ligne sont automatiquement inclus, mais on peut l'empêcher en ajoutant \ à la fin de la ligne
	\subsubsection{Operateur}
		\textit{str(ojt)} : Renvoie une représentation en chaîne de caractères de object
	\subsubsection{Classes}
		\textit{text.capitalize()} : son premier caractère en majuscule et le reste en minuscule\\
		\textit{text.title()} : les mots commencent par une capitale\\
		\textit{text.split([sep=None, maxsplit=- 1])} : liste des mots de la chaîne, en utilisant sep comme séparateur de mots, maxsplit est le nombre maximum de divisions.\\
		\textit{text.substitute(mapping={}, /, **clef)}\\
		\textit{text.strip([chars])} : Renvoie une copie de la chaîne dont des caractères initiaux et finaux sont supprimés\\
		\textit{f'{}'.format(*args, **kwargs)} : 
			https://peps.python.org/pep-3101/, 
			https://docs.python.org/fr/3/library/string.html\#formatstrings\\
		\textit{text.uper()} : mettre en majuscule une chaine de caractères

### Nombres
	Type
		int : nombre entier ;
		float : décimaux ;
		bool : bouléin ;
	Indexation
		* : etoile ;
		\_ : Atrap-tout ; la dernière expression affichée
	Operateur
		+,-,*,/,**,//
		int(float) : nombres entiers ;
		round()
	Comparateur
		<,>,<=,>=,==,!=
Iterable
	Type
		n-uplt ou tuple
		list
	Opérateurs
		\^ : diference
		\& : intersection
		| : union
	Indexation
		liste[nombre] : pour lire le n ieme nombre de la sequance
		liste[debut:fin] : pour lire l'inteval de n1-n0 commence en n0 et fini en n1
	Operateur
		len(tuple) : renvoie la longueur
		list(tuple) : transforme en liste
		rang() : occupe toujours la même (petite) quantité de mémoire
			rang(fin) : itérer sur une suite de nombres, elle commance a 0 et fini fin-1
			rang(debut:fin) : itérer sur une suite de nombres, elle commance a debut et fini fin-1
			rang(debut:fin,etpe) : itérer sur une suite de nombres, elle commance a debut et fini fin-1 par etap
		reversed(list) : Inverse l'ordre des éléments dans la liste.
		set(list) : élimine les doublons
		sum(list[,start]) : Additionne les valeurs
	Classes
		list.append(var) : sujet+=[var]
		list.clear() : Supprime tous les éléments
		list0.extend(list1) : mettre bout à bout deux listes
		list.insert(nmbr, var) : Insère un élément à la position indiquée.
		sep.join(list) : transformer une liste en de caractère separer par sep
		list.pop([nmbr]) : Enlève de la liste l'élément situé à la position indiquée et le renvoie en valeur de retour
		list.remove(var) : Supprime de la liste le premier élément dont la valeur est égale à var
\subsection{Calculatrice}
	\subsubsection{Operation}
		\textit{+} ; Adition\\
		\textit{-} ; Soustraction\\
		\textit{/} ; Divition\\
		\textit{//} ; Division Euclidienne\\
		\textit{\%} ; Reste\\
		\textit{**} ; Puissance
## Commande
### Fonction
- `input()` : faire une demande
- `print()` : affichée
  - `%(VAR)` : marque le début du marqueur
    - `#` : La conversion utilise la « forme alternative »
    - `0` : Les valeurs numériques converties sont complétées de zéros
  - `end=','` : pour le metre a la suite
- `round(NMBR)` : Arrondi un nombre
- `sorted(iterable,/,*[, key=None, reverse=False])` : Ordonne les éléments dans la sequance
  - `key` : doit être une fonction (ou autre appelable) qui prend un seul argument et renvoie une clef à utiliser à des fins de tri
  - `reverse` : pour déterminer l'ordre descendant des tris
### Classes
- `sujet.copy()` : Renvoie une copie superficielle
- `sujet.count(var[, start[, end]])` : Renvoie le nombre d'éléments ayant la valeur var dans la liste.
- `sujet.find(var[,debut[, fin]])` : donne la position et -1 si il n'est pas dedans
- `sujet.isnan()`
### Instruction
- `as` : capturer la valeur d'une partie d'un filtre avec le mot-clé
- `break` : sort de l’enceinte
- `continue` : continuer le flot d'exécution au prochain cycle de la boucle la plus imbriquée
- `del VAR` : Supprime var
- `in` ou `not in` : testent l’appartenance
- `is` :
- `pass` : ne fait rien, pour fournir une syntaxe correcteboucle if.
- `with` :
- `raise` :
### Boucle
- `while` : tan que ; 
- `for,else` : itère sur les éléments d'une séquence
- `if,elif,else` : 
- `math sujet` : Filtre, Seul le premier qui correspond est exécuté, elle permet aussi d'extraire dans des variables des composantes de la valeur (afectation),
- `try,except, else,finally` : Esayer ;
## Lire
- `open(file, mode='r', buffering=- 1, encoding=None, errors=None, newline=None, closefd=True, opener=None)` : lire ou écrire qu'un seul fichier
  - `file` : chemin du ficher
  - `mode` : spécifier dans quel mode le fichier est ouvert, se combine
    - `r` : en lecture (par défaut)
    - `w` : en écriture, en effaçant le contenu du fichier
    - `x` : pour une création exclusive, échouant si le fichier existe déjà
    - `a` : en écriture, ajoutant à la fin du fichier s'il existe
    - `b` : mode binaire
    - `t` : mode texte
    - `+` : ouvre en modification (lecture et écriture)
### Classes
- `FILE.close()` :
- `FILE.read([taille])` : lit une certaine quantité de données et la renvoie sous forme de chaîne
- `FILE.readline()` : lit une seule ligne du fichier
- `FILE.seek(decalage, origine)` : La position est calculée en ajoutant décalage à un point d'origine
- `FILE.tell()` : renvoie un entier indiquant la position actuelle dans le fichier
- `FILE.write(text)` : écrit le contenu de chaine dans le fichier et renvoie le nombre de caractères écrits. et la justaposition d'une

		https://peps.python.org/pep-0636/
		case condition : confronte la valeur d'une expression, si il es préfix de \_ il equivaut à else
		var0 | var1 : combiner plusieurs littéraux en un seul filtre
		*\_ : filtre qui reconnaît les séquences à plus élément
## Création
### Annotations
https://peps.python.org/pep-0448/ ; https://peps.python.org/pep-0572/
- `@` : fonction décorateur
### Argument 
Les arguments nommés doivent suivre les arguments positionnés
- `argmt:type` : 
- `argmt=defaut` : la valeur par défaut n'est évaluée qu'une seule fois par appel de la fonction
- `*argmt` : n-uplet contenant les arguments positionnés au-delà de la liste des paramètres formels, lors de l'appel de fontion *argmt permet de separe la liste
- `**argmt der` : dictionnaire contenant tous les arguments nommés à l'exception de ceux correspondant à un paramètre formel
- Spéciaux  il est logique de restreindre la façon dont les arguments peuvent être transmis, peut etre util en cas d'embuiguité
  - `argmt, /` : restreint le passage aux seuls arguments par position
  - `*, argmt` : n'autorise que les arguments nommés
### Fonction
- `lambda * : f(*)` : fonction anonyme
- `def nom(*)` : nouvelle fonction
  - `return` : renvoient une valeur
- class
  - `CLASS.__doc__` : la première ligne soit toujours courte et résume de manière concise l'utilité de l'objet
  - `CLASS.__annotations__` : dictionary and have no effect on any other part of the function
- `dict(dico,**clef)` : Renvoie un nouveau dictionnaire initialisé à partir d'un argument positionnel optionnel, et un "iterable" (vide ou non) d'arguments nommés.
  - `DICT0 |= DICT1` : Met à jour le dictionnaire dico0 avec les clés et les valeurs de dico1
  - `DICT.key()` : iterable des clef
  - `DICT.value()` : iterable des valeur
  - `DICT.items()` : iterable des clef et des valeur
- `zip(list0,list1)` : renvoie un itérateur de n-uplets, où le ie n-uplet contient le ie élément de chacun des itérables passés en arguments, s'arrête lorsque l'itérable le plus court est épuisé
- `iter(dico)` : Renvoie un itérateur sur les clés du dictionnaire =zip(dico.values(), d.keys())=[(var1, var0) for (var0, var1) in dico.items()]

class :
		Annotations
			Les objets peuvent interagir entre eux, regroupe des "méthodes" et des attributs qui définissent un objet
			utiliser une notation UpperCamelCase
		Argument
			sur\_class : 
		Operateur
			\_\_match\_arg\_\_(*\_) : prennent en charge le filtrage par arguments positionnels en définissant un ordre des attributs
			def \_\_missing\_\_(self, clef) : cré les clef si il sont manquant
			def \_\_init\_\_(self, clef) : self.clef=args ; initialise les clefs
			@proprerty def clef(self) : return self.clef ; Récupération du nombre
			@clef.setter def clef(self, args) : self.clef = args ; Changement du nombre
			def clef(self) : sur\_class.clef(self)

Module
	sudo apt-get install python-mod : installer le module si il n'y est pas
	Argument
		profile : analyser l'execution des fonctions
		calendar : calendrier ;
		time : temps ;
		math : les opérations mathématiques
		itertools :
			permutations : liste de tous les cas possibles
			product : tous les cas possibles d'une liste elle-même composée de liste
		random : aléatoires ;
			randint() : Retourne un entier aléatoire
			random() : Retourne une valeur aléatoir
			shuffle(list) : Mélange aléatoirement une liste
		re : expressions régulières ; https://python.doctor/page-expressions-regulieres-regular-python
		matplotlib : dessine des graphiques ; https://matplotlib.org/
		tkinter : Interface graphique, https://python.doctor/page-tkinter-interface-graphique-python-tutoriel
		glob : Recherche d'éléments par motif
			\_.glob(motif) : Liste les dossiers et les fichiers correspondants au motif
			\_.iglob(motif) : Idem que glob mais retourne un itérateur
		sys : fonctions systèmes ; accès à certaines variables utilisées et maintenues par l'interpréteur
			https://docs.python.org/fr/3/library/sys.html\#sys.builtin\_module\_names
			\_.argv : liste des arguments de la ligne de commande passés à un script Python
			\_.path : chemin de recherche de module est accessible à l'adresse
				\_.insert(0, "chemain") : pour ajouter un dossier
		os : interagir avec le système d'exploitation
			\_.path(chem) : Manipuler les chemins
			\_.listdir(chem) : Lister les fichiers d'un dossier
			\_.walk(chem, topdown=True, onerror=None, followlinks=False) : afficher tous les éléments d'un dossier ainsi que ses dossiers enfants
			\_.makedirs(path) : Créer récursivement tous les dossiers d'un path si ceux-ci n'existent pas
			\_.mkdir(path) : Créer le dernier dossier d'un path. Si un des dossiers n'existe pas une erreur est retournée
			\_.remove(path) : Supprime le fichier / dossier indiqué
			\_.rename(old, new) : Renomme le fichier / dossier indiqué
		lxml : Extensible Markup Language, (langage de balisage extensible en français) ; http://lxml.de/tutorial.html
		urllib2 : récupérer des informations sur internet
		cx\_freeze : compiler le code et le rendre exécutable ; https://cx-freeze.readthedocs.io/en/latest/
	Operateur
		from mod import fnctn as renom : importé qu’une fois par session de l’interpréteur, si non ajouter ; importlib.reload(mod)
		if \_\_name\_\_ == "\_\_main\_\_" : utilisable comme script aussi bien que comme module importable
\section{Envirenement}
	\subsection{Virtuel}
		Les applications seront parfois d'avoir besoin d'une version spécifique d'une bibliothèque.La solution à ce problème est de créer un environnement virtuel.\\
		\textit{python -m venv tutorial-env} : créera le \textit{tutorial-env} répertoire s'il n'existe pas, et crée également des répertoires à l'intérieur contenant une copie du Python interprète et divers fichiers de soutien.\\
		\textit{tutorial-env\textbackslash Scripts\textbackslash activate} : changer l'invite de votre shell à montrer ce qui environnement virtuel que vous utilisez\\
		\textit{deactivate} : désactiver un environnement virtuel

	\
	Type
		py : modifiable
		pyc : compilé
		pyw : executé sans lancement de terminal
	python [-bBdEhiIOqsSuvVWx?] [-c command | -m module-name | script | - ] [args] : lit les lignes de commande et les exécute jusqu'à ce qu'un caractère EOF
		args :
			nom de fichier : il lit et exécute le script contenu dans ce fichier
			répertoire : lit et exécute un script d’un certain nom dans ce répertoire
		EOF :
			Ctrl-Z, Enter : caractère fin de fichier
		
## Style
### Compréantion
- `LIST = [F(VAR) for VAR in range(NMBR)]` : ainsi var n'est pas remplacé et n'existe pas
- Iterateur : apporte un niveau d'abstraction plus élévé et donc peut augmenté la rapidité du programme
- Générateurs : permettent de créer plus facilement des itérateurs ;
  - `yield`, similaire au return des fonctions sauf qu'il ne signifie pas la fin de l'exécution de la fonction mais une mise en pause et à la prochaine itération la fonction recherchera le prochain yield
- Paquet : le dossier contien un ficher meme vide mais nomé "__init__.py"
- `from PAQUET import *` : dans le fichier "__init__.py" metre __all__ (liste contenant nom de module devant être importés par l'etoile)
- sou-packages :  from ./CHEMIN import mod ; importations relatives
### Ecriture
- Utilisez des indentations de 4 espaces et pas de tabulation.
- Les lignes ne dépassent pas 79 caractères.
- Lignes vides pour séparer les fonctions et les classes, ou pour scinder de gros blocs de code à l'intérieur de fonctions.
- Placez les commentaires sur leurs propres lignes.
- Espaces autour des opérateurs et après les virgules, mais pas juste à l'intérieur des parenthèses : a = f(1, 2) + g(3, 4).
- Utilisez toujours self comme nom du premier argument des méthodes.
- Prenez l'habitude de nommer votre classe uniquement avec des caractères alphanumériques et commençant par une majuscule, à l'inverse l'instance peut être nommée sans majuscule.
- Mettre les fonctions en majuscule pour bien faire la difference avec les varible en minuscule.
- Mettre les variable pour definire la fonction en entier, à la difference des variable courente en abrevier.
- Mettre les nom de dossier en minuscule et les noms de fichier avec la premier lettre en majuscule.

<!-- Cée par WyloW2RicardO le 2024-01-09 -->
