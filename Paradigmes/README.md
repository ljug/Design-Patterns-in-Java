# Paradigmes de programmation

En développement du logiciel, différentes approches ont été utilisées pour concevoir des langages de programmation. Pour chaque langage de programmation, nous avons un ensemble de concepts, de principes et de règles. Un tel ensemble de concepts, de principes et de règles s'appelle un paradigme de programmation. En théorie, les langues ne sont considérées que dans un seul paradigme, mais, dans la pratique, les paradigmes de programmation sont généralement combinés dans une seule langue.

Dans ces Compléments de cours à NFP121, nous soulignerons les paradigmes de programmation sur lesquels est basé le langage de programmation Java, ainsi que les principaux concepts décrivant ces paradigmes. Celles-ci sont une programmation impérative, orientée objet, déclarative et fonctionnelle.

## Programmation impérative

La programmation impérative est un paradigme de programmation dans lequel des instructions sont écrites pour modifier l'état du programme. Ce concept est apparu au début de l'informatique et est très proche de la structure interne de l'ordinateur. Le programme est un ensemble d'instructions qui est exécuté sur l'unité de traitement et il modifie l'état (qui est stocké sous forme de variables dans la mémoire) de manière impérative. Le nom impératif implique le fait que les instructions exécutées dictent le fonctionnement du programme.

Aujourd'hui, la plupart des langages de programmation les plus populaires reposent plus ou moins sur le paradigme de l'impératif. Le meilleur exemple de langage principalement impératif est le C.

## Paradigme orienté objet
Le paradigme orienté objet est souvent associé à la programmation impérative, mais, dans la pratique, les paradigmes fonctionnels et orientés objet peuvent coexister. Java est un exemple de cette collaboration en particulier a partir de la version 8.

Dans la page suivante ([Paradigme OO java](OO_java/)), nous présentons brièvement les principaux concepts orientés objet tels qu'ils sont implémentés dans le langage Java.

## Paradigme déclaratif

Contrairement à la programmation impérative, la programmation déclarative est un paradigme de programmation qui spécifie ce que doit faire un programme sans spécifier comment le faire. Parmi les langages purement déclaratifs figurent les langages de requête de base de données, tels que SQL et XPath, et les expressions régulières.

Les langages de programmation déclaratifs sont plus abstraits que les impératifs. Ils n'imitent pas la structure matérielle et, par conséquent, ne modifient pas les états des programmes, mais les transforment en nouveaux états, et sont plus proches de la logique mathématique.

En général, les styles de programmation qui ne sont pas impératifs sont considérés comme relevant de la catégorie déclarative. C'est pourquoi de nombreux types de paradigmes entrent dans la catégorie déclarative. Dans ces pages, nous examinerons le seul qui soit pertinent pour notre parcours (dans le cadre de Java): la programmation fonctionnelle.

### Programmation fonctionnelle

La programmation fonctionnelle est un sous-paradigme de la programmation déclarative. Contrairement à la programmation impérative, la programmation fonctionnelle ne modifie pas l'état interne du programme.

En programmation impérative, les fonctions peuvent être davantage considérées comme des séquences d'instructions, de routines ou de procédures. Ils dépendent non seulement de l'état stocké dans la mémoire, mais peuvent également changer cet état. De cette manière, l'invocation d'une fonction impérative avec les mêmes arguments peut produire des résultats différents selon l'état du programme actuel. Parallèlement, la fonction exécutée peut modifier les variables du programme.

Dans la terminologie de programmation fonctionnelle, les fonctions sont similaires aux fonctions mathématiques et la sortie d'une fonction ne dépend que de ses arguments, quel que soit l'état du programme, qui, dans le même temps, reste inchangé par l'exécution de la fonction.

Paradoxalement, bien que la programmation impérative existe depuis la création des ordinateurs, les concepts de base de la programmation fonctionnelle remontent à avant. La plupart des langages fonctionnels sont basés sur le lambda calcul, un système formel de logique mathématique créé dans les années 1930 par le mathématicien Alonzo Church.

L'une des raisons pour lesquelles les langages fonctionnels sont devenus si populaires à cette époque est qu'ils peuvent facilement s'exécuter dans des environnements parallèles. Cela ne doit pas être confondu avec le multithreading. La principale caractéristique qui permet aux langages fonctionnels de fonctionner en parallèle est le principe de base sur lequel ils résident: les fonctions reposent uniquement sur les arguments d'entrée et non sur l'état du programme. En d’autres termes, elles peuvent être exécutées n’importe où, et les résultats des multiples exécutions parallèles sont ensuite joints et utilisés ultérieurement.




