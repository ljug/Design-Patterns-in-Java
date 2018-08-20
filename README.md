# "Design Patterns" en Java
Les modèles de conception ou principes de conception représentent les meilleures pratiques utilisées par les développeurs de logiciels orientés objet expérimentés. Les modèles de conception sont des solutions aux problèmes généraux rencontrés par les développeurs de logiciels lors du développement de logiciels. Ces solutions ont été obtenues par essais et erreurs par de nombreux développeurs de logiciels sur une période assez longue.
## Public concerné
* Complément de cours pour les auditeurs du Cnam Liban pour les UEs NFP121, NSY208, NSY209, GLG203, GLG204, NFP103.
* Mais aussi des développeurs expérimentés pour fournir les meilleures solutions à certains problèmes rencontrés lors du développement de logiciels.
* Et pour les développeurs non expérimentés apprennent la conception des logiciels de manière simple et rapide.
## Pré-requis
Un mimimum de programmation Java, avoir déjà réalisé quelues petit ptojet en Java. Pour les auditeurs du Cnam Liban par exemple avoir le nuveaux des UE NFA031,NFA032 et NFA035
# Introduction et préparation
## Quels sont et pourquoi des principes de conceptions?
Représenter un ensemble de lignes directrices qui nous aident à éviter d'avoir un mauvais design (Robert Martin)

### Caractéristiques d'une mauvaise conception

* Rigidité - Difficile à changer car chaque changement affecte trop de parties du système
* Fragilité - Lorsque vous effectuez un changement, des parties inattendues du système se détériore
* Non-réutilisabilité (immobilité) - Difficile à réutiliser dans une autre application parce qu'il ne peut pas être extrait de l'application actuelle

### Caractéristiques d'une bonne conception

* Propre et modulaire (opposé à la non-réutilisabilité)
* Très cohésif (opposé à la rigidité)
* À couplage lâche (opposé à la fragilité)

## Le gang des 4 GOF (Gagg of Four)
En 1994, quatre auteurs, Erich Gamma, Richard Helm, Ralph Johnson et John Vlissides ont publié un livre intitulé *"Design Patterns - Elements of Réutilisable Object-Oriented Software"*, qui a initié le concept de Design Pattern dans le développement de logiciels.

Ces auteurs sont connus collectivement sous le nom de **Gang of Four (GOF)**. Selon ces auteurs, les modèles de conception reposent principalement sur les principes suivants de conception orientée objet.

1. Programmer em pasant par une interface pas directement l'implémentation
2. Favoriser la composition d'objets pas l'héritage
## Types de design paterns
Dans le livre de référence sur les modèles de conception, **Design Patterns - Elements of Réutilisable Object-Oriented Software**, il existe 23 modèles de conception pouvant être classés en trois catégories: 
1. les modèles Creational, 
2. Structural 
3. et Behavioral. 

Nous allons également discuter d'une autre catégorie de modèle de conception: les modèles de conception J2EE.

Type de pattern | Description 
----------------| ------------
Pattern de création| Permettent de créer des objets tout en masquant la logique de création, plutôt que d'instancier directement les objets à l'aide d'un nouvel opérateur. Cela donne au programme plus de flexibilité pour décider quels objets doivent être créés pour un cas d'utilisation donné. 
Pattern de structure | Concernent la composition des classes et des objets. Le concept d'héritage est utilisé pour composer des interfaces et définir des manières de composer des objets pour obtenir de nouvelles fonctionnalités.
Pattern de comportement | Concernent la communication entre objets.
Pattern J2EE | Concernent spécifiquement le niveau de présentation dans le cadre de dévellopement coté serveur et le Java Entreprise JAVA EE. Ces modèles ont été identifiés par Sun Java Center.
