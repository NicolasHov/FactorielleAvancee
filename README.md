[![Build Status](https://travis-ci.org/simplon-promo-pe-1/FactorielleAvancee.svg?branch=init)](https://travis-ci.org/simplon-promo-pe-1/FactorielleAvancee)

# Factorielle Avancée

Base de code propice à l'écriture de tests unitaires et à la gestion d'exceptions

[Suite du TP Factorielle dédié à la découverte des tests unitaires](https://github.com/simplon-promo-pe-1/Factorielle)

## Contenu de l'exercice

1. Etape 1 :
  - Forker le dépôt
  - Mettre en place le build Travis et modifier le Readme en conséquence
  - Clôner son dépôt en local et importer le projet dans son environnement de développement
  - Améliorer le code en mettant en place une gestion d'exception :
    - Commencer par écrire un test visant à valider que pour l'entier 50, le calcul de la factorielle doit amener une exception de type *UnsupportedOperationException* (exception faisant partie du JDK)
    - Retoucher l'implémentation afin de faire passer le tests (on pourra notamment comparer fact(n) et fact(n-1) en estimant qu'il est anormal lorsque fact(n) < fact(n-1)
2. Etape 2 : remplacer l'usage de *UnsupportedOperationException* par votre propre exception (ex. *FactorielleUnavailableException*)
3. Etape 3 : simplifier votre code pour vous débarrasser des instructions *throws FactorielleUnavailableException* dans votre classe de test (indice : regarder les particularités des classes *IllegalArgumentException* et *UnsupportedOperationException*)
4. Etape 4 : écrire un programme avec sa méthode main permettant l'exécution du calcul de factorielle pour un argument
  - écrire une méthode *main* exploitant la première chaîne de caractères du tableau passé en paramètres, pour la convertir en entier et appeler sur une instance de *Factorielle* la méthode *calculer*
  - l'exécution du programme doit afficher dans la console :
    - "Cas passant pour " suivi du nombre fourni en paramètre et du résultat
    - "Cas d'erreur 1" si ce n'est pas un entier qui est fourni en paramètre
    - "Cas d'erreur 2" si l'exécution amène une exception de type *IllegalArgumentException*
    - "Cas d'erreur 3" si l'exécution amène une exception de type *FactorielleUnavailableException*
    - "Cas d'erreur 4" si aucun paramètre n'est fourni au programme
  - il est interdit de modifier la classe *Factorielle*
   
