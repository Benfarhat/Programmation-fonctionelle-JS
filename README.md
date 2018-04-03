# Introduction à la programmation fonctionnelle 

- [Introduction à la programmation fonctionnelle](#introduction-%C3%A0-la-programmation-fonctionnelle)
    - [Introduction](#introduction)
    - [Paradigme de programmation](#paradigme-de-programmation)
        - [Quel paradigme choisir](#quel-paradigme-choisir)
    - [Principaux paradigmes](#principaux-paradigmes)
        - [programmation impérative](#programmation-imp%C3%A9rative)
            - [La programmation structurée](#la-programmation-structur%C3%A9e)
            - [La programmation procédurale](#la-programmation-proc%C3%A9durale)
        - [programmation orientée objet](#programmation-orient%C3%A9e-objet)
            - [La programmation orientée classe](#la-programmation-orient%C3%A9e-classe)
            - [La programmation orientée prototype](#la-programmation-orient%C3%A9e-prototype)
            - [La programmation orientée composant](#la-programmation-orient%C3%A9e-composant)
        - [La programmation déclarative](#la-programmation-d%C3%A9clarative)
            - [Programmation descriptive](#programmation-descriptive)
            - [la programmation logique](#la-programmation-logique)
            - [la programmation par contraintes](#la-programmation-par-contraintes)
            - [la programmation fonctionnelle](#la-programmation-fonctionnelle)
    - [Autres paradigmes](#autres-paradigmes)

## Introduction

Tous les développeurs front-end ont toujours un process interne de suivi, tests et maitrise des nouveautés qui généralement amélioreront la qualité du travail rendu. Les SPA (single page applicationà trop souvent confondu avec les sites à page unique utilisé en tant que vitrine, sont l'une de ces nouvelles techno du moment. Grace à React (notamment React viber) la vitesse de rendue est devenue incroyable, la mise à jour des composants d'une page est instantanée et pour jouir de cela, il faut en comprendre tous les mécanismes, depuis les nouveautés de javascript (à partir de ES6), React js et compagnie (comme la version React Native), de l'implémentation de flux via Redux,  on s'aperçoit que les nouveautés sont nombreuses, et en avancant dans nos études on se rend compte que les principes se regroupent, de l'immutabilités au fonction pure, des middlewares à base de fonction de haut niveau à la curryfication des fonctions, tous ces concept pointent vers un seul phénomène,celui de la programmation fonctionnelle. 

## Paradigme de programmation

Un développeur informatique comme pour toute les autres professions, est la pour satisfaire un besoin et pour atteindre ce besoin il faut résoudre un certain nombre de problèmes. 
Par analogie, le besoin est la destination ou vous voulez vous rendre, et le développeur n'est rien d'autre que le chauffeur. Il y a plusieurs facon de faire, certains choisirons le chemin le plus court, le plus logique a leur sens et qui sera éventuellement parsemer d'embuches, d'autres préfèreront le chemin le plus long mais avec le moins d'obstacles. 
Les différentes `approches` possible permettant de résoudre vos problèmes pour satisfaire un besoin, ce sont les paradigmes. Chaque paradigme repose sur un ensemble de concepts de programmation, des concepts qui sont parfois très voisins. Un langage de programmation peut suivre un ou plusieurs paradigmes (multi-paradigme), ceci est possible parce que certains concepts d'un paradigme à un autre se ressemble. 

Ce qui est intéressant dans le domaine du developpement front-end, c'est qu'on ne risque pas de tomber dans la monotonie, les besoins évoluent toujours et encore, chaque besoin résolu est une expérience à partager. Seulement voila, les besoins évoluent tellement vite que les programmes utilisant un paradigme donnée se compliquent vite, et là ... dite vous qu'à ce moment il y a matière à voir naitre un nouveau concept de programmation. C'est ce qu'on appel le `principe d'extension créatrice` (sans jeux de mots avec celui de la "destruction créatrice" en économie, quoi que...).

### Quel paradigme choisir

Cela dépend des problèmes, il faudra avoir besoin parfois d'appliquer des concepts provenant de paradigmes différents et donc le choix ne sera plus sur un seul paradigme mais sur un ensemble de paradigmes. Ainsi, dans la logique d'un développement qui pourrait necessité plusieurs concepts différents, un bon langage de programmation doit être multiparadigme (comme javascript). Cela a le mérite de ne pas avoir à jongler entre plusieurs langages. Les quelques paragraphes qui suivant se veulent d'éclaircir la question et donc de comprendre le "pourquoi du comment". C'est comme si une personne voulait faire devenir full stack MERN développeur sans connaitres les fonctions fléchées (arrow functions), l'affectation par décomposition (destructuration), le spread operator ou encore le fonctionnement des promesses.


## Principaux paradigmes
En programmation, il existe trois grandes familles de paradigme à savoir:

- la programmation impérative
- la programmation orientée objet
- la programmation déclarative

### programmation impérative
Si lors de notre programmation on impose les étapes que l'on doit "impérativement" faire pour résoudre nos problèmes, alors vous l'aurez compris, on parle de programmation impérative. C'est ce qui a notre sens, semble le plus naturel, mais n'est pas forcément la meilleure approche à utiliser.
La programmation impérative est composé de "sous catégories" à savoir la `programmation structurée` et la `programmation procédurale`.

#### La programmation structurée 

Historiquement parlant, l'une des instructions les plus utilisées et qui permettait de résoudre de nombreux soucis, était l'instruction "goto", c'est une des instructions de branchement faisant de nos codes sources une vraie chasse aux trésors. Lorsqu'elle était mal utilisée, on se retouvait dans de la `programmation spaghetti`. La programmation spaghetti est un anti-pattern (anti-patron) qui n'est plus utilisé et qui a laissé place à la programmation structurée utilisant des structures de contrôle (conditionnelles ou alternatives avec les if, else, switch et itératives avec les for et while). Ces nouvelles structures permettent de mieux contrôler le flux d'exécution d'un programme. Pour ne pas compliqué le flot d'exécution de vos programmes, il est recommandé de n'avoir qu'un seul point d'entrée pour chaque boucle.

#### La programmation procédurale

Lorsqu'on regroupe une suite d'instruction dans un bloc appelé procédure et que l'on fonde le développement de nos applications sur l'appel a ces procédures avec éventuellement de la récursivité (une procédure qui s'appelle elle même). Les procédures peuvent faire appel a des variables du contexte global et donc d'avoir des `effets de bord` (side effect en anglais). De plus cette réutilisation de code, cela permet un gain d'écriture, une simplification de la maintenabilité mais également d'éviter de faire de la programmation spaghetti

### programmation orientée objet

Alors que la programmation impérative utilise les variables globales et les sous-routines, la programmation orientée objet regroupe ces variable et ces opérations dans des objets qui sont une modélisation des entités d'une application (Produit, Facture, Etudiant, Voiture)
Par exemple un objet Voiture aura comme attribut sa vitesse max, son nombre de vitesse, sa couleur, son immatriculation, sa marque et il aura comme méthode ce qu'on appelle des setters (méthodes permettant de modifier les valeurs des attributes) et getters (méthodes permettant de récupérer les valeurs des attributs), ainsi que d'autre méthode de fonctionnement telles que accélerer, décélerer, réparer, charger (pour les voitures électriques) etc orientée objet offre des concepts tels que:
- l'encapsulation: la classe définit les données appelées attributs et les méthodes qui définissent le comportement de l'objet, ces détails internent et son fonctionnament son cacher, on appelle cela l'encapsulation
- l'instanciation: on définit une classe une seule fois, l'opération qui permet de créer autant d'objet que l'on veut à partir de cette classe, s'appelle l'instanciation, lors de l'instanciation, un constructeur permettra d'initialiser le contenu d'un objet. Ce constructeur est appelé automatiquement lors de l'instanciation.
- l'héritage: permettant de créer des classes dérivés qui conservent les mêmes attributs et méthodes et en rajoute d'autre ou en modifie (surcharge). La classe de base est appelée classe parent, la classe dérivée est appelée classe enfant. L'héritage permet de créer de nouvelle classe plus spécifiques comme par exemple les classes voiture, bus et vélo qui hériterait d'une classe de base véhicule et qui leur permettra d'hérité d'attribut tel que le nombre de roue, le puissance moteur ainsi que des méthodes tels que avancer, reculer, s'arreter, etcle polymorphisme: permettre d'avoir en apparence une même méthode pour plusieurs classes (cas du polymorphisme par sous typage les classes ont une méthode qui porte le même nom mais pas le même code), la surcharge est une sorte de polymorphisme ad-hoc
-  ou encore l'injection de dépendance (le découplage d'une classe qui a besoin d'une instance d'une autre classe, très facilement réalisable via le design pattern factory).

Il y a tois sous catégories de programmation orientée objets:
- la programmation orientée classe
- la programmation orientée prototype
- la programmation orientée composant

#### La programmation orientée classe 

Une classe est une définition abstraite de l'objet et donc l'objet est une instanciation d'une classe (on parle de typage statique). Une classe est statique, la dérivation d'une classe est possible grace à l'héritage 

#### La programmation orientée prototype

Un prototype est mutable, il permet d'avoir un héritage dynamique et donc un typage dynamique qui necessite une surconsommation de mémoire, même typescript, supposé ajouté du typage à javascript, ou encore n'est en faite qu'un moyen de controle lors de la transpilation (traduction du langage typescript vers javascript). 

Plus simplement, le prototype est une superclasse dont héritent tous les objets, pour ajouter une méthode il suffit d'utiliser prototype comme suit:

```
function voiture(){
    this.color;
    this.marque;
    this.vitesse;
}

voiture.prototype.accelerer() = function(){
    // ...
}
voiture.prototype.decelerer() = function(){
    // ...
})
```

#### La programmation orientée composant

Dans ce paradigme, l'approche est plus modulaire, il y a toujours de l'objet auquels ont y ajoute tout ce dont il a besoin pour devenir un élement réutilisable. Le développement d'une application consistera en l'assemblage de composants. Les connexions entre composants peuvent être résolues par de l'injection de dépendance.
Trois types de composants sont à connaitre: les composants techniques (utilitaire de manipulation des données, élements UI), les composants métiers (entité du domaine) et les composants applicatifs (pour le traitement interne d'une application)

### La programmation déclarative

La programmation déclarative consiste a déclarer les données du problèmes, puis demande au programme de les résoudres, nous allons revenir à plus de détails dans ce principe, mais par exemple vos pages web utilise de l'HTML, vous n'avez qu'a définir les élements de votre pages sans vous soucier de la façon avec laquelle il sera rendu (c'est le travail du moteur de rendu de votre navigateur).

> Pour information, les moteurs de rendu se décomposent en plusieurs familles de moteur de rendu dont Gecko, KHTML, Microsoft Edge. Les front-ends comprendront pourquoi on leur demande de tester la compatibilité de leur application sur plusieurs navigateurs. C'est pour vérifier que leur page est bien rendu par les bibliothèques de rendu et non les navigateurs. Par exemple il est inutile de tester sur "Firefox et Kompozer" ou de tester sur "Opera et Google Chrome", puisque chaque couple de navigateurs utilise le même moteur de rendu

Pour revenir à nos moutons, alors que la programmation impérative s'occupe du COMMENT, la programmation déclarative s'occupe du QUOI. Les 4 grands dérivés sont:
- la programmation descriptive
- la programmation logique
- la programmation par contraintes
- la programmation fonctionnelle

#### Programmation descriptive



#### la programmation logique



#### la programmation par contraintes



#### la programmation fonctionnelle

## Autres paradigmes

Les langages de programmation suivent tous au moins un des différents paradigmes recensés et qui ne se limite pas au trois paradigmes ci dessus présentés, d'autres existent comme:
- la programmation séquentielle
- la programmation concurrente
- la programmation générique
- la programmation logique
- la programmation réactive
- la programmation non-déterministe
- la programmation synchrone


