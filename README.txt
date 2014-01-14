Télécharger des émissions en mp3 des archives de France Culture.

Utilisation:

# Première utilisation: télécharger la liste des programmes
$fcult update

# Afficher les programmes disponibles
$fcult list
000 Le 5 à 7
001 A voix nue
002 Affaires étrangères
003 Atelier de Création Radiophonique
004 L'Atelier de la création
...

# Afficher les émissions du programme Affaires Etrangères
$fcult list 2
000. 2013-02-02 Les nouvelles figures de la guerre
001. 2013-02-09 Tunisie et Egypte : les deux révolutions dévoyées
002. 2013-02-16 La diplomatie vaticane
...

# Télécharger l'émission Tunisie et Egypte du programme Affaires Etrangers
fcult get 2 1
....

# Mettre à jour les émissions d'Affaires Etrangères
fcult update 2


Ce script est écrit en Perl et nécéssite les modules CPAN suivants:
    - LWP::Simple
    - URI::Escape
    - HTML::Entities
    - File::Spec
    - Storable

Ce script a été conçu pour fonctionner sous Linux, et stocke des données dans
~/.fcult afin d'éviter de devoir retélécharger les listes de programmes et 
d'émissions.

Copyright (c) Martijn van der Kwast 2013 <martijn@vdkwast.com>

Ce programme peut-être distribué selon les conditions de la license
artistique perl (http://dev.perl.org/licenses/artistic.html)

