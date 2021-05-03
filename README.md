# Projet-MOSH-Szuter-Leydier

# Introduction

Ce projet s’inscrit dans l’UF « Du capteur au banc de test » de la spécialité 4GP à l’INSA Toulouse. 
L’objectif est la réalisation d’un capteur de déformation à base graphite, à l’aide d’un module Arduino. Pour ce faire, nous avons recouvert la surface d’une tranche de papier avec une géométrie définie d’une couche de graphite à sa surface. Les avantages d’un tel capteur sont sa simplicité, son cout relativement faible et une bonne mobilité grâce à sa légèreté.

# Description du phénomène physique

La couche de graphite que nous déposons à l’aide d’un critérium sur la surface du papier possède des propriétés électriques (conductivité électrique et résistance) variable en fonction de sa géométrie. En effet, le graphite peut être représenté comme un réseau de nanoparticules séparées par une distance définie dans le réseau caractéristique. Lorsque nous allons appliquer une contrainte mécanique sur le papier, nous allons déformer la couche de graphite et ainsi modifier la distance entre les nanoparticules. Nous allons avoir une variation de la conductivité électrique et donc de la résistance de notre couche de graphite. A l’aide de ce phénomène, nous pouvons réaliser une jauge de contrainte.

# De Kitcad à la fabrication du PCB shield (perceuse)

Les plans de notre shield ont été fait sur le logiciel Kitcad.
Visualisation 2D
Visualisation 3D

# Fabrication 

Notre shield, partie recouvrant l’Arduino où nous allons placer nos composants et nos modules a été faite dans le bâtiment du GP à l’aide de Catherine Crouzet. Notre modèle du shield en 2D est imprimé sur un papier calque. Nous le plaçons sur une plaque d’epoxy recouverte d’une fine couche de cuivre que nous allons insoler aux UV pendant environ 5 minutes. Par la suite, nous mettons l’ensemble dans un révélateur qui va enlever la partie insolée. La plaquette d'epoxy est ensuite déposée dans un bain de perchlorure de fer pour la gravure, pendant environ 5 minutes également. Le cuivre non protégé par la résine a été retiré, ce qui permet d'obtenir le PCB modélisé. Enfin, on applique de l'acétone sur la plaquette afin d'ôter les dernières traces de résine résiduelle.



# Perçage : 

A l’aide d’une perceuse situé au GP, nous avons fais les trous sur le PCB permettant de placer nos composants. Ils ont un diamètre de 1mm pour notre AOP et les différents modules externes (Bluetooth , encodeur rotatoire et écran OLED)  et un diamètre de 0,8 mm pour les resistances et condensateurs .

# Code Arduino

Le programme arduino permet à la l’aide de bibliothèques spécifiques permet de contrôler un encodeur rotatoire et un écran OLED positionnés sur le shield.

# Application APK et module bluetooth

Notre application APK a été faite sur le site MIT application inventor. Elle a pour but de se connecter au module bluetooth directement relié au Shield pour récupérer facilement la valeur de résistance du capteur sur notre téléphone
