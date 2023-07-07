---
title: Etch-a-Sketch
picture: etch-a-sketch.png
last_commit: 02-13-2022
github_repository: https://github.com/Qwib-Qwib/Etch-a-Sketch
---

Une sorte "d'écran magique" surtout codé en JavaScript pur. Lorsque l'utilisateur passe sa souris sur le cadre, il laisse une trainée colorée. A chaque fois qu'il repasse sa souris sur une case colorée, la case s'assombrie de 10% jusqu'à devenir noire. L'utilisateur peut choisir le nombre de cases dans le cadre, ce qui a une influence sur la taille de chaque case, le cadre lui-même gardant la même dimension.

Petit problème que j'ai remarqué plus tard : toutes les cases ne deviennent pas complètement noires, certaines ne deviennent que *presque* noires. Je pense que cela à quelque chose à voir avec le fait que la division qui s'opère afin de calculer la nouvelle couleur donne parfois un float, ce qui rend le calcul imprécis au fil des assombrissements, un concept dont je n'avais pas conscience au moment de faire ce projet.

[Lien vers le projet en ligne](https://qwib-qwib.github.io/Etch-a-Sketch/)
