# Introduction à la programmation fonctionnelle 

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

C'est une méthodologie qui prend la relève sur la programmation impérative. Alors que cette dernière utilisait les variables globales et des sous-routines ()

Les langages de programmation suivent tous au moins un des différents paradigmes recensés et qui ne se limite pas au trois paradigmes ci dessus présentés, d'autres existent comme:
- la programmation séquentielle
- la programmation concurrente
- la programmation générique
- la programmation logique

Leur nombre n'est pas fini et à tout moment une personne peut trouver une nouvelle approche de développement et mettre en place un langage de programmation permettant de l'appliquer.

Javascript est un de langages appelés multi-paradigmes, puisqu'en effet il permet de faire

### programmation impérative
Si lors de notre programmation on impose les étapes que l'on doit "impérativement" faire pour résoudre nos problèmes, alors vous l'aurez compris, on parle de programmation impérative. C'est ce qui a notre sens, semble le plus naturel, mais n'est pas forcément la meilleure approche à utiliser.


Mais il y en a d'autres comme:
- la programmation séquentielle
- la programmation concurrente
- la programmation générique
- la programmation logique