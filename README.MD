#Lancer le projet : 
dans le dossier racine du projet <b>mvn clean install spring-boot:run</b> 


#Model :   
La classe <b>Poisson</b> représente l'ensemble des différents 'poissons' qui peuvent exister dans le projet. 
La classe <b>Espece</b> représente l'ensemble des especes qui regroupent différent poissons aux caractéristiques similaires
Chaque poisson appartient à une espece.

L'interface <b>ConsolePrintable</b> définies une méthode consolePrint(). Tout objet qui l'implémente peut être affiché dans la cosole par cette méthode. La classe Poisson et la classe Espece implémentent cette méthode.


#Routes :
get:
/poissons -> liste l'ensemble des poissons
/especes/{especeID}/poissons -> liste l'ensemble des poissons de l'espece {especeID}
/poissons/{poissonID}/espece -> donne l'espece du poisson dont l'id est {poissonID}
/especes -> liste l'ensemble des especes
/especes/{id} -> donne l'espece du poisson dont l'id est{id}


post:
/poissons -> permet de créer un poisson
/especes -> permet de créer une espece

delete:
/poissons/{id} -> permet de supprimer le poisson à l'id {id}
/especes/{id} -> permet de supprimer l'espece à l'id {id} et tous les poissons associés
