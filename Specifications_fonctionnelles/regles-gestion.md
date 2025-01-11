# Règles de gestion

## Configuration du bot
- Le système peut être ou en pause.
- L'état de pause peut être associé à une ou plusieurs promos.
- Le bot peut créer les messages à la demande.

## Rappeler à un formateur qu'il a oublié de faire signer
- Le message est lié à un channel de promo.
- Il y a un une liste selectionable contenant les formateurs liés a la promo.
- Un seul formateur peut être sélectionné à la fois.
- Un utilisateur doit patienter avant de pouvoir réutiliser la fontion.
- Il faut qu'un formateur soit sélectionner pour lancer le vote.
- Le bot envoie un message privé au formateur pour l'avertir qu'il doit autoriser les apprenants à signer.

## Prévenir les apprenants qu'ils peuvent signer
- Le message est lié à un channel de promo.
- Le message permet de notifier les apprenants qu'ils peuvent signer.
- Seul les formateurs et chargés de projets peuvent peuvent utiliser cette fonction.
- Le message est envoyé directement dans le fil de discussion signature.
- La promo est notifiée via un tag @.
- Le bot sauvegarde l'ID du message.
- Le message n'est utile que pendant que la signature est possible sur les plateformes externes.
- Le bot supprime le message quand il n'est plus utile.

## Rappeler à un apprenant qu'il a oublié de signer
- Le message est lié à un channel de promo.
- Le message contient la liste des apprenants liés a la promo.
- Seuls les formateurs peuvent interagir avec le message.
- Les formateurs peuvent selectionner un ou plusieurs apprenants.
- Il faut au moins un apprenant sélectionné pour valider le rappel.
- Les apprenants sélectionnés sont notifiés par message privé.

## Journalisation
- Le bot enregistre chaque fois qu'un utilisateur fait appel à lui dans un journal.
- Le journal écrit les informations de la manière suivante :
     À quelle date a été lancée la commande.
     Quel utilisateur a lancé la commande.
     Quelle commande a été utilisée.
     À quel utilisateur la commande est-elle destinée.

## Structuration de l'organisation
- Un formateur est lié à une ou plusieurs promotions.
- Une promotion est liée à un ou plusieurs formateurs.
- Un apprenant suit une formation à la fois.
- Une promotion regroupe plusieurs apprenants.
- Un apprenant appartient à une promotion.
- Une promotion a un chargé de projets.
- Un chargé de projets a une ou plusieurs promotions.
- Une formation peut être dispensée dans un ou plusieurs centres.
- Un centre peut proposer une ou plusieurs formations.

# Données nécessaires au bot
- Le bot a accès à la liste des formateurs.
- Le bot a accès à la liste des formations.
- Le bot a accès à la liste des promotions.
- Le bot a accès à la liste des apprenants.
- Le bot a accès à la liste des chargés de projets.
- Le bot a accès à l'ID Discord des utilisateurs.
- Le bot a accès à l'ID des canaux Discord des promotions.
- Le bot a accès à l'ID des fils Discord de signature.

