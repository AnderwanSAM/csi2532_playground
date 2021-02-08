# csi2532_playground
 
Lab1 CSI2532 Uottawa 
Introduction à GIT 
Andie SAMADOULOUGOU 300209487

 
lab 2 CSI 2532 UOTTAWA 
Installation de Postgres 
Configuration d'environnement de developpement local 
Creation de base de donnees 
Manipulations basiques de la base de donnees (Requetes SQL simples)





lab 3 CSI 2532 Uottawa 

Dessin de diagrammes ER pour un systeme universitaire 
Cardinalite et relatons entre entites 

Probleme  : 
Une base de données universitaire contient
des informations sur les professeurs
(identifié par le numéro de sécurité sociale
ou SSN) et les cours (identifié par courseid).
Les professeurs donnent des cours; chacun
de les situations suivantes concernent
l'ensemble de relation teaches. 

Solutions : 

1) . Les professeurs peuvent enseigner le
même cours sur plusieurs semestres et seule
la plus récente doit être enregistrée
https://github.com/AnderwanSAM/csi2532_playground/blob/lab03/lab3_1.png

2) Chaque professeur doit enseigner un
cours
https://github.com/AnderwanSAM/csi2532_playground/blob/lab03/lab3_2.png

3) ) Chaque professeur enseigne exactement
un cours (ni plus, ni moins).
https://github.com/AnderwanSAM/csi2532_playground/blob/lab03/lab3_3.png

4) Chaque professeur enseigne exactement
un cours (ni plus, ni moins), et chaque cours
doit être enseigné par un professeur.
https://github.com/AnderwanSAM/csi2532_playground/blob/lab03/lab3_4.png

5) Les professeurs peuvent enseigner le
même cours sur plusieurs semestres et
chaque doit être enregistrée
https://github.com/AnderwanSAM/csi2532_playground/blob/lab03/lab3_5.png

6) ) Supposons maintenant que certains cours
puissent être enseignés conjointement par
une équipe de professeurs, mais il est
possible qu'aucun professeur dans une
équipe ne puisse enseigner le cours. 
https://github.com/AnderwanSAM/csi2532_playground/blob/lab03/lab3_6.png
