---
title: Mastermind sur terminal
picture: mastermind.png
last_commit: 10-10-2022
github_repository: https://github.com/Qwib-Qwib/mastermind
---

Le jeu de société Mastermind, entièrement codé en pur Ruby, jouable sur terminal. Deux joueurs s'opposent, humains ou ordinateurs : l'un choisit un code secret composé de quatre pions colorés, l'autre à 12 essais pour tenter de deviner la couleur et l'emplacement de chaque pion, en ne recevant que de vagues indices sur chacun de ses choix.
L'ordinateur se base sur [l'algorithme de Knuth](https://www.cs.uni.edu/~wallingf/teaching/cs3530/resources/knuth-mastermind.pdf) afin de deviner les codes. Cet algorithme a pour but de deviner le code avec 100% de certitude en pas plus de 5 coups. Pour cela, l'ordinateur va donner la priorité à la destruction des champs du possible, plutôt que tenter le coup ayant la meilleur chance de gagner à un tour donné : mieux vaut proposer un coup qui est sûr d'être perdant de manière immédiate, mais qui va grandement nettoyer le set de coups possibles pour les prochains tours, que d'en tenter un qui à une chance incertaine d'être le bon et qui n'avancera guère plus le joueur s'il s'avère être effectivement mauvais.
C'est l'un des projets les plus intéressants sur lesquels j'ai travaillé, et mon immplémentation est perfectible, notamment en matière d'UI. Je trouve notamment la pause et l'invitation à presser une touche entre chaque action assez maladroite, et je pense qu'il y a moyen de faire plus simple d'un point de vue de récupération d'input en associant chaque couleur avec un indice plutôt qu'en obligeant le joueur à retaper sa proposition entière. Cependant, je trouve le résultat assez épatant, étant donné que j'ai codé ce projet assez tôt dans mon apprentissage, à une époque où je ne connaissais pas le pattern MVC ou Rails ! J'aimerais repasser dessus à un moment et faire quelque chose de plus propre, si je trouve le temps.
