Sprint n°2: Voir le readme du projet + réalisation d'un controller qui permet à l'admin de gérer les comptes liés à l'application du jumeau numérique. Cette gestion concerne 2 statuts possibles pour un compte: administrateur et utilisateur. La seule différence entre ces 2 statuts est que l'administrateur doit s'occuper, en plus, de la gestion des comptes.
Cependant, ce controller n'est pas visible sur l'application puisque, après découverte, nous avons pris la décision de partir sur un bundle (paquet) nommé easyadmin, qui comme mon controller, s'occupe de la gestion des comptes. C'est Benoit qui s'est occupé d'intégrer ce bundle à l'application mais nous avons laissé mon controller comme plan B. Ce bundle donne des fonctionnalités qui sont parfaitement en rapport avec ce que nous voulions et c'est aussi pour cela que symfony est un très bon framework car il offre des outils permettant d'avoir un rendu complètement cohérent et performant rendant la vie du développeur plus facile.



Sprint n°3:

Elaboration d'un serveur en javascript qui va servir de remplacement au robot grâce à la bibliothèque socket.io et au framework nodejs grâce auquel nous pouvons exécuter le fichier javascript à l'origine du serveur. A ce serveur sera connecté un ou plusieurs clients (qui seront avertis lorsqu'un nouveau client se connecte au serveur du robot) qui ont alors 2 solutions : 
    - le serveur demande au client la saisie des valeurs d'angles pour chacun des axes du robot (attention: le serveur ne fait que        demander les valeurs. C'est pourquoi le serveur va enregistrer ces valeurs et va les envoyer comme si c'était lui qui était à l'origine de ces valeurs. Pour l'envoi, que je n'ai pas encore fait, je vais essayer de partir sur un stockage des données envoyées par le serveur dans un fichier qui sera ensuite travaillé par Brice (lire les valeurs dans ce fichier)
    - le serveur envoie des valeurs aléatoires au client à travers, comme la 1ère solution, un stockage des données dans un fichier qui sera ensuite traité par Brice. 

Je suis sur un problème actuellement concernant la 1ère soltuion qui consiste, pour le client, à ne pas envoyer les valeurs d'angles qui sont vides ou égales à null car par rapport au code du serveur, ce dernier va stocker toutes les valeurs envoyées par le client. Cependant, comme j'ai mis une boucle for concernant les valeurs saisies par le client, c'est la dernière valeur correcte saisie par le client qui est visible et stockée par le serveur. Ainsi, si je n'arrive pas à corriger ce problème, j'essaierais de travailler sur l'issue avec laquelle le serveur pourrait envoyer la dernière saisie qu'il voit et qu'il a stocké.
Une fois ce problème réglé, je me pencherais sur l'envoie de données au client.

Pour voir le schéma looping_jumeau.loo, il faut utiliser le logiciel que vous allez récupérer ici https://www.looping-mcd.fr
