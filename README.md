# csi2532_playground
 
Lab 06  CSI2532 Uottawa 

Andie SAMADOULOUGOU 300209487

**Les fichiers SQL ont aussi été push dans GITHUB **

ANDIE SAMADOULOUGOU 
300209487
Lab6

1)	   
/*Lister les noms des artistes et leur lieu de naissances*/

**SELECT name,birthplace FROM artists;**


![Image of 1](https://github.com/AnderwanSAM/csi2532_playground/blob/lab06/lab6_1.png)
 
2)	   
/*Lister le title et le price de toutes les artworks après 1600.*/

**SELECT title, price 
FROM artworks
WHERE year >1600;**

![Image of 2](https://github.com/AnderwanSAM/csi2532_playground/blob/lab06/lab6_2.png)

 
3)	     

/*Lister le title et le type de toutes les artworks qui ont été peintes en
2000 ou peintes par Picasso.*/

**SELECT title, type 
FROM artworks
WHERE year =2000 OR artist_name ='Picasso';**

![Image of 3](https://github.com/AnderwanSAM/csi2532_playground/blob/lab06/lab6_3.png)
 
4)	    
/*Lister les name et birthplace de tous les artists nés entre 1880 et
1930. (ASTUCE: EXTRACT(YEAR FROM dateofbirth) vous donne
l'année à partir d'un attribut DATE)*/

**SELECT name, birthplace 
FROM artists 
WHERE (EXTRACT(YEAR FROM dateofbirth)) BETWEEN 1880 AND 1930;**

 ![Image of 4](https://github.com/AnderwanSAM/csi2532_playground/blob/lab06/lab6_4.png)

5)	  
/*. Lister les name et le country de naissance de tous les artists dont le
style de peinture est Modern, Baroque or Renaissance. (ASTUCE:
utilisez le mot-clé IN).*/


**SELECT name, birthplace
FROM artists
WHERE style IN ('Modern','Baroque','Renaissance');**

 ![Image of 5](https://github.com/AnderwanSAM/csi2532_playground/blob/lab06/lab6_5.png)


6)	    

/*
Lister tous les détails des artworks dans la base de données, triés
par title*/

**SELECT * 
FROM artworks
ORDER BY title;**

![Image of 6](https://github.com/AnderwanSAM/csi2532_playground/blob/lab06/lab6_06.png)
 

7 ) 
/*Lister les name et les customer ids de tous les customers qui aiment Picasso*/

**SELECT name, customer_id 
FROM customers AS s , likeartists AS T  
WHERE s.id = T.customer_id AND T.artist_name = 'Picasso';**

![Image of 7](https://github.com/AnderwanSAM/csi2532_playground/blob/lab06/lab6_7.png)


8)	.Lister les name de tous les customers qui aiment les artistes de style Renaissance et dont le price est supérieur à 30000

**WITH artists_name(artist_name) as (SELECT name FROM artists WHERE style = 'Renaissance'),
artists_fan(customer_idd) as (SELECT customer_id FROM likeartists,artists_name WHERE likeartists.artist_name  = artists_name.artist_name)
SELECT name
FROM customers ,artists_fan
WHERE id = artists_fan.customer_idd AND amount > 30000;**

![Image of 8](https://github.com/AnderwanSAM/csi2532_playground/blob/lab06/lab6_8.png)

 


 
