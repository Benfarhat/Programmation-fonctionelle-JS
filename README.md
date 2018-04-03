# Introduction à la programmation fonctionnelle 

## Paradigme de programmation

Un développeur informatique comme pour tout autre profession, est la pour satisfaire un besoin et pour atteindre ce besoin il faut résoudre un certain nombre de problèmes. 
Par analogie, le besoin est la destination ou vous voulez vous rendre, et le développeur n'est rien d'autre que le chauffeur. Il y a plusieurs facon de faire, certains choisirons le chemin le plus court, le plus logique a leur sens et qui sera éventuellement parsemer d'embuches, d'autres préfèreront le chemin le plus long mais avec le moins d'obstacles. 
Les différentes `approches` possible permettant de résoudre vos problèmes pour satisfaire un besoin, ce sont les paradigmes. En programmation, il existe trois grandes familles de paradigme à savoir:

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