

# "Design Patterns" Paradigmes de programmation en Java

## Paradigmes de programmation

En développement du logiciel, différentes approches ont été utilisées pour concevoir des langages de programmation. Pour chaque langage de programmation, nous avons un ensemble de concepts, de principes et de règles. Un tel ensemble de concepts, de principes et de règles s'appelle un paradigme de programmation. En théorie, les langues ne sont considérées que dans un seul paradigme, mais, dans la pratique, les paradigmes de programmation sont généralement combinés dans une seule langue.

En savoir plus : [Paradigmes de programmation](Paradigmes/)

## "Design Patterns" et principes

Le développement de logiciels n’est pas uniquement un travail d’écriture de code, que vous travailliez dans une grande équipe ou dans un projet unique. La manière dont une application est structurée a un impact énorme sur le succès d'une application logicielle.

Lorsque nous parlons d’une application logicielle performante, nous ne discutons pas seulement de la façon dont l’application fait ce qu’elle est censée faire, mais aussi des efforts que nous avons déployés pour la développer et de la facilité de test et de maintenance de cette dernière. Si cela n'est pas effectué correctement, les coûts de développement, qui montent en flèche, se traduiront par une application dont personne ne veut.

Les applications logicielles sont créées pour répondre à des besoins en constante évolution. Une candidature réussie devrait également fournir un moyen simple de l’étendre pour répondre aux attentes en constante évolution.

Heureusement, nous ne sommes pas les premiers à rencontrer ces problèmes. Certains problèmes ont déjà été résolus et résolus. Ces problèmes courants peuvent être évités ou résolus si un ensemble de principes et de modèles de conception orientés objet est appliqué lors de la conception et du développement de logiciels. 

Les modèles de conception ou principes de conception représentent les meilleures pratiques utilisées par les développeurs de logiciels orientés objet expérimentés. Les modèles de conception sont des solutions aux problèmes généraux rencontrés par les développeurs de logiciels lors du développement de logiciels. Ces solutions ont été obtenues par essais et erreurs par de nombreux développeurs de logiciels sur une période assez longue.

Les [principes de conception](Principes/) orientés objet sont également appelés [SOLID](Principes/). Ces principes constituent un ensemble de règles pouvant être appliquées lors de la conception et du développement de logiciels, afin de créer des programmes faciles à gérer et à développer. Ils ont été introduits pour la première fois par Robert C. Martin et font partie du processus de développement logiciel agile. [Les principes SOLID](Principes/) incluent le principe de [responsabilité unique](Principes/#ru), le [principe d'ouverture / fermeture](Principes/#of), le [principe de substitution de Liskov](Principes/#lsp), le principe de [séparation des interfaces](Principes/#isp) et le principe d'[inversion de dépendance](Principes/#dip). 

Outre les principes de conception, il existe des modèles de conception orientés objet. Les modèles de conception sont des solutions réutilisables générales qui peuvent être appliquées aux problèmes courants. Suivant le concept de Christopher Alexander, Kent Beck et Ward Cunningham ont d'abord appliqué les modèles de conception à la programmation, puis les ont popularisés avec le livre intitulé Gang Of Four (GOF) en 1994. Dans la section suivante, nous présenterons les principes de conception SOLID. , qui sera suivi des modèles de conception dans les prochains chapitres.

*Un pattern est une règle en trois parties exprimant une relation entre un **contexte**, un **problème** et une **solution** ( Alexander)*



## Public concerné
* Complément de cours pour les auditeurs du Cnam Liban pour les UEs NFP121, NSY208, NSY209, GLG203, GLG204, NFP103.
* Mais aussi des développeurs expérimentés pour fournir les meilleures solutions à certains problèmes rencontrés lors du développement de logiciels.
* Et pour les développeurs non expérimentés apprennent la conception des logiciels de manière simple et rapide.
## Pré-requis
Un minimum de programmation Java, avoir déjà réalisé quelques petit projet en Java ou pas. Pour les auditeurs du Cnam Liban par exemple avoir le niveaux des UE NFA031,NFA032 et NFA035
# Introduction et préparation
## Quels sont et pourquoi des principes de conceptions?
Représenter un ensemble de lignes directrices qui nous aident à éviter d'avoir un mauvais design (Robert Martin)

### Caractéristiques d'une mauvaise conception

* Rigidité - Difficile à changer car chaque changement affecte trop de parties du système
* Fragilité - Lorsque vous effectuez un changement, des parties inattendues du système se détériore
* Non ré-utilisabilité (immobilité) - Difficile à réutiliser dans une autre application parce qu'il ne peut pas être extrait de l'application actuelle

### Caractéristiques d'une bonne conception

* Propre et modulaire (opposé à la non ré-utilisabilité)
* Très cohésif (opposé à la rigidité)
* À couplage lâche (opposé à la fragilité)

## Le gang des 4 GOF (Gang of Four)
En 1994, quatre auteurs, Erich Gamma, Richard Helm, Ralph Johnson et John Vlissides ont publié un livre intitulé *"Design Patterns - Elements of Réutilisable Object-Oriented Software"*, qui a initié le concept de Design Pattern dans le développement de logiciels.

Ces auteurs sont connus collectivement sous le nom de **Gang of Four (GOF)**. Selon ces auteurs, les modèles de conception reposent principalement sur les principes suivants de conception orientée objet.

1. Programmer en passant par une interface pas directement l'implémentation
2. Favoriser la composition d'objets pas l'héritage
## Types de design patterns
Dans le livre de référence sur les modèles de conception, **Design Patterns - Elements of Réutilisable Object-Oriented Software**, il existe 23 modèles de conception pouvant être classés en trois catégories: 
1. les modèles "Creational", 
2. "Structural" 
3. et "Behavioral". 

Nous allons également discuter d'une autre catégorie de modèle de conception: les modèles de conception J2EE.

Type de pattern | Description 
----------------| ------------
Pattern de création| Permettent de créer des objets tout en masquant la logique de création, plutôt que d'instancier directement les objets à l'aide d'un nouvel opérateur. Cela donne au programme plus de flexibilité pour décider quels objets doivent être créés pour un cas d'utilisation donné. 
Pattern de structure | Concernent la composition des classes et des objets. Le concept d'héritage est utilisé pour composer des interfaces et définir des manières de composer des objets pour obtenir de nouvelles fonctionnalités.
Pattern de comportement | Concernent la communication entre objets.
Pattern J2EE | quelques modèles complémentaires concernent spécifiquement le niveau de présentation dans le cadre de développement coté serveur et le Java Entreprise JAVA EE. Ces modèles ont été identifiés par Sun Java Center.

## Les principaux modèle par type

## Les modèles de création
Dans cette catégorie, il existe 5 modèles principaux :

| Nom	| Rôle
| -----  | -----
| Fabrique (Factory)	| Créer un objet dont le type dépend du contexte
| Fabrique abstraite (abstract Factory)	| Fournir une interface unique pour instancier des objets d'une même famille sans avoir à connaître les classes à instancier
| Monteur (Builder)	 | -
| Prototype (Prototype)	| Création d'objet à partir d'un prototype
| Singleton (Singleton)	| Classe qui ne pourra avoir qu'une seule instance

... //TODO à completer ...
https://java-design-patterns.com/