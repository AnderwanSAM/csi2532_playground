# csi2532_playground
  
Lab04 


Probleme : 
 Une base de données universitaire contient
des informations sur les professeurs
(identifié par le numéro de sécurité sociale
ou SSN) et les cours (identifié par courseid).
Les professeurs donnent des cours; chacun
de les situations suivantes concernent
l'ensemble de relation teaches.


OBJECTIFS
‣ Transformez les diagrammes ER en
diagrammes relationnels.
‣ Gérer la structure de la base de
données avec SQL
‣ CREATE DATABASE / TABLE

Liens : 
1. Les professeurs peuvent enseigner le
même cours sur plusieurs semestres et seule
la plus récente doit être enregistrée.
https://github.com/AnderwanSAM/csi2532_playground/blob/lab04/csi2532_l4_1.png

3) Chaque professeur enseigne exactement
un cours (ni plus, ni moins).

https://github.com/AnderwanSAM/csi2532_playground/blob/lab04/ci2532_l4_3.png

5) Les professeurs peuvent enseigner le
même cours sur plusieurs semestres et
chaque doit être enregistrée.
https://github.com/AnderwanSAM/csi2532_playground/blob/lab04/csi2532_l4_5.png


6) Supposons maintenant que certains cours
puissent être enseignés conjointement par
une équipe de professeurs, mais il est
possible qu'aucun professeur dans une
équipe ne puisse enseigner le cours.
Modélisez cette situation en introduisant des
ensembles d'entités et des ensembles de
relations supplémentaires si nécessaire.
https://github.com/AnderwanSAM/csi2532_playground/blob/lab04/csi2532_l4_6.png



SQL pour chaque schema : 

1. Les professeurs peuvent enseigner le
même cours sur plusieurs semestres et seule
la plus récente doit être enregistrée.








3) Chaque professeur enseigne exactement
un cours (ni plus, ni moins).



5) Les professeurs peuvent enseigner le
même cours sur plusieurs semestres et
chaque doit être enregistrée.



6) Supposons maintenant que certains cours
puissent être enseignés conjointement par
une équipe de professeurs, mais il est
possible qu'aucun professeur dans une
équipe ne puisse enseigner le cours.
Modélisez cette situation en introduisant des
ensembles d'entités et des ensembles de
relations supplémentaires si nécessaire.








