# C-Exemple-Base-De-Donn-es
Travaux d'initiation à la communication entre une application Windows Forms développée sous visual Studio et une base de données SQL 




HOWTO:

Vous devez disposer d'un serveur local sur lequel ajouter la base de données comcli (Wamp fait tout à fait l'affaire).

Au démarrage de l'application, vous serez invité à remplir les zones de texte nécessaires à la communication à la base de donées comcli. Les zones de texte sont préremplies avec les informations nécessaires pour une connexion à la base avec les paramètres par défaut. Si vous ne changez rien au comportement initial de Wamp, vous n'avez qu'une chose à modifier:
L'application dispose de deux modes, à choisir dans la liste déroulante "Mode" de la fenêtre principale.

Le mode Administration permet de gérer une des trois tables "client", "commande" ou "produit". Par défaut, le chanmp "Table", indiquant la table à modifier, est rempli avec la valeur "client". Si vous souhaitez modifier une des autres tables, il vous faudra changer cette zone de texte. En cliquant ensuite sur "connexion", il vous sera possible de consulter, de modifier, d'ajouter, ou de supprimer une entrée de la table sélectionnée.

Le mode Factures permet de consulter la liste des commandes passées pour un utilisateur sélectionné. Un bouton "détail clients" permet à l'utilisateur d'accéder à la liste des clients et de leurs informations, dans le cas où il souhaiterai consulter ses données avant de consulter ou modifier/ajouter ses commandes.
Une fois un client sélectionné, l'utilisateur a accès à la liste des commandes passées par celui-ci. Il peut alors les modifier (ou en créer une nouvelle) en cliquand sur le bouton "générer/modifier une facture". La fenêtre s'agrandit alors. L'utilisateur peut sélectionner un produit dans la nouvelle liste, modifier la quantité à ajouter, et cliquer sur la flèche vers le haut pour ajouter ce produit à la commande en cours. En sélectionnant un produit dans la liste de déails, et en cliquant sur la flèche du bas, il peut retirer ce produit de la liste.


TODO:

  General:
Commenter le code !
Refactorer le code
Améliorer le Howto
Améliorer l'interface utilisateur (embellir)

  Factures:
Améliorer l'interface utilisateur (plus de retours utilisateur, plus de demandes de confirmation)
Améliorer la gestion de la date de commande (peut être source d'erreurs)
Permettre d'ajouter plus d'un produit déjà sélectionné sans devoir retirer ce produit de la liste pour ensuite le remettre
Baisser (localement) la quantité en stock d'un produit ajouté à la liste, pour éviter de créer par exemple deux commandes dont la quantité cumulée d'un produit est supérieure à la quantité en stock de ce produit.

