# Application en Python 🎮

## 📎 **Résumé** 📎:

le but du projet est de faire un code qui permette de controller un robot avec une interface fait avec designer cette interface devait possédé des boutton pour ce déplacer et tirer ainsi qu'un boutton pour passer le robot en mode automatique, un sprite qui pointe vers la direction du robot 

## 🎮 **Contexte** 🎮 : 

Le code fourni est une application utilisant la bibliothèque PyQt5 pour créer une interface graphique. L'application permet de contrôler un agent dans une arène virtuelle. L'agent est représenté par un sprite de Pikachu et peut se déplacer, tirer et changer d'orientation. L'agent communique avec un serveur distant en utilisant la bibliothèque j2l.pytactx.agent.

Le code utilise un modèle de programmation basé sur des événements. Lorsqu'une touche est enfoncée, une fonction correspondante est appelée pour effectuer une action spécifique, comme le déplacement de l'agent ou le tir. L'agent est également mis à jour périodiquement en interagissant avec le serveur distant pour récupérer son état actuel, tel que la vie et les munitions.

L'interface graphique comprend des éléments tels qu'une barre de vie, une barre de munitions, des étiquettes pour afficher le pseudo de l'agent et l'arène, ainsi qu'une image représentant le sprite de Pikachu qui change en fonction de l'orientation de l'agent.

Avant d'utiliser l'application, l'utilisateur doit remplir un formulaire avec un pseudo, le nom de l'arène et un mot de passe. Une fois le formulaire validé, une connexion est établie avec le serveur distant, et l'agent est créé et associé à cette connexion.

L'application prend également en charge un mode automatique activable par une touche spécifique, où l'agent peut se déplacer et agir de manière autonome sans intervention de l'utilisateur.

## 💻 **User Story** 💻 :

En tant qu'utilisateur, je souhaite pouvoir contrôler un agent dans une arène virtuelle en utilisant une interface graphique conviviale.

## 🔧 **Critères d'acceptation** 🔧 :

Je dois pouvoir saisir mon pseudo, le nom de l'arène et un mot de passe dans un formulaire.
Après avoir validé le formulaire, je veux être connecté au serveur distant et créer mon agent.
Je veux voir un sprite de Pikachu représentant mon agent dans l'interface graphique.
Je veux pouvoir déplacer mon agent vers le haut, le bas, la gauche et la droite en utilisant les touches du clavier.
Je veux pouvoir changer l'orientation de mon agent en appuyant sur des touches spécifiques.
Je veux voir une barre de vie et une barre de munitions pour mon agent, afin de connaître son état actuel.
Je veux que l'image du sprite de Pikachu change en fonction de l'orientation de mon agent.
Je veux pouvoir tirer en appuyant sur une touche spécifique et arrêter de tirer après un certain délai.
Je veux pouvoir activer un mode automatique où mon agent peut se déplacer et agir de manière autonome.
Je veux que l'interface graphique affiche mon pseudo et le nom de l'arène que j'ai spécifiés dans le formulaire.
Note : Les détails concernant les fonctionnalités spécifiques de l'agent, tels que la communication avec le serveur distant, la récupération des données d'état, et la lecture d'une mélodie en cas d'élimination d'un ennemi, ne sont pas inclus dans cette user story, car ils sont déjà implémentés dans le code fourni.

## 💽 **dépendance** 💽 :

PyQt5 : une bibliothèque pour la création d'interfaces graphiques en utilisant le framework Qt.
j2l.pytactx.agent : un module personnalisée spécifique au projet pour interagir avec le serveur distant et contrôler l'agent dans l'arène virtuelle.
