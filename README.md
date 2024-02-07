# Research_Lung

Dans le cadre de ma recherche dans mon cursus universitaire, je travaille sur la modélisation numérique de l'écoulement de l'air dans les voies respiratoires à l’aide de FreeFEM++ pour la modélisation numérique, Paraview pour l'analyse visuelle.

# Introduction

Le poumon humain possède une structure géométrique assez atypique, complexe. Dans le domaine de l'imagerie médicale, on rencontre des difficultés à visualiser l'ensemble du poumon. En effet, nous pouvons seulement apercevoir la haute partie du poumon. L'idée de la recherche est donc de proposer une approche afin de pouvoir visualiser la partie obscure de l'imagerie. 

Pour recréer au mieux la simulation du poumon humain dans la réalité, il y a plusieurs notions physique à prendre en compte, passant par du Navier-Stokes, au terme convectif sans oublier la rigidité du poumon au moment de l'expiration. Dans notre cas, nous travaillons aussi sur une pathologie choisi au préalable, l'asthme, afin de pouvoir tester notre simulation.

# Structure du GitHub

Pour voir l'évolution du projet, je divise le code en plusieurs section :

- **Navier-Stokes** : L'idée est de pouvoir comprendre comment fonctionne Navier-Stokes, comment le coder et comment la simulation réagit selon les différents cas.
- **Poumon_2D** : L'idée est de pouvoir faire le maillage du Poumon sur FreeFEM++.
- **EulerImplicit** : L'idée est de travailler sur la méthode du splitting via ImplicitEuler. 
- **Combinaison NS+EulerImplicit+Poumon** : L'idée est de pouvoir faire simuler dans un poumon rempli d'air avec toutes les contraintes qu'elle présente.
- **Terme convetif** : L'idée est de rajouter le terme convectif quand on est satisfait des résultats des versions précédentes.
- **Asthme** : L'idée est de pouvoir tester la simulation avec une pathologie dont un état de l'art a été effectué en amont.
