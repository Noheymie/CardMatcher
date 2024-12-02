# CardMatcher 

## Objectif
Dans le cadre de notre 2ème année d'ingénierie, nous avons eu la tâche de créer une interface permettant de reconnaître des cartes de jeu présentées face à la caméra. Il a ainsi fallu inclure un retour du flux vidéo issu de la webcam, une gestion de la base de données de cartes de jeu, un algorithme SIFT de reconnaissance de caractéristiques, et enfin un taux de correspondance pour le résultat.

De plus ce projet a été réalisé en plusieurs étapes ("sprints") dans un contexte de méthodologie agile, avec un suivi du Product Owner.

## Utilisation
Il existe 2 modes d'utilisation de l'interface.

***Apprentissage***:
* Le mode Apprentissage vous permet de créer votre propre base de données de cartes.
* Placer une carte à jouer dans le rectangle vert et appuyer sur _Apprentissage_.
* Il est demander de nommer la carte, veuillez suivre la norme suivante : {numéro de la carte}{couleur de la carte}, avec Coeur = C, Carreau = D, Trèfle = T, Pique = P, Ace = A, Roi = K, Reine = Q, Valet = V (exemple : le roi de carreau sera **RD** et le 8 de trèfle sera **8T**).
* La carte choisie est maintenant enregistrée dans le dossier Apprentissage, qui constitue votre base de données personnelle. Les cartes enregstrées ne seront pas supprimées après arrêt du programme. De plus, si une ancienne carte possède déjà le nom choisi pour une nouvelle carte, l'ancienne sera écrasée.

***Test*** :
* En mode test vous pourrez tester la fonctionnalité de reconnaissance de cartes.
* Commencez par choisir une base de données à l’aide du bouton _Select Database_. Cette dernière pourra être une base de données existante que vous avez téléchargé, ou par défaut la base de données Apprentissage que vous avez alimenté.
* Placez une carte dans le rectangle rouge et appuyez sur _Test_.
* Suite à cela, à droite de l’écran s’affiche la carte la plus proche de celle que vous venez de tester d'après l'algorithme SIFT, ainsi qu’un taux de correspondance.
* Dans le dossier Test vous retrouverez l’image de la carte que vous avez testé.
* Dans le dossier TestResult vous retrouverez la comparaison de cette carte à toutes celles de la base de données choisie, pour observer comment l'algorithme SIFT trouve les correspondances.

## Elements techniques
HTML/CSS, Java, OpenCV, MVC, SCRUM, SIFT

## Equipe Image2
Niama Amtoun, Noémie Gerard, Orson Lento, Mathilde Raby, Nicolás Pérez Burbano

