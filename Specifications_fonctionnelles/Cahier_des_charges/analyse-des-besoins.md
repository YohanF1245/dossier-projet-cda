# Analyse du Besoin

Après entretien avec le client, nous avons pu dégager les spécifications fonctionnelles nécessaires au bon fonctionnement du bot.
Le bot Discord "Signature" a pour vocation de fluidifier la communication pour les échanges liés à l'émargement. Les oublis de signatures présentant un réel risque de manque à gagner financier et entraînant une surcharge administrative, il est primordial d'apporter une solution visant à réduire les risques d'oublis.
Les principaux utilisateurs finaux amenés à manipuler le bot sont les formateurs, les apprenants et les chargés de projets.
Diverses contraintes s'opposent à nous, à commencer par les API des outils externes d'émargement inaccessibles. L'environnement Discord propose lui aussi son lot de contraintes liées aux possibilités restreintes de l'API Discord

## Processus métier

Discord est l'outil de communication sélectionné par les centres Simplon Hauts-de-France. Il est utilisé par tout le personnel et les apprenants.
Il y a deux solutions d'émargement selon si la formation est financée par la région (SoWeSign) ou non (NetYparéo).
Il y a une disparité dans les systèmes d'exploitation : en grande majorité Mac ou Linux, Windows dans une plus faible proportion.
Le groupe Simplon se scinde en plusieurs groupes par région. Les méthodes de fonctionnement peuvent légèrement différer d'une région à l'autre. L'utilisation d'un Discord communautaire est une méthode propre à la région Hauts-de-France, et la gestion des outils d'émargement est commune à toutes les régions.

## Exigences non fonctionnelles :
- L'utilisation du bot doit être la plus accessible possible pour les utilisateurs.  
- Les actions doivent nécessiter le moins de clics possibles.  
- Le bot doit permettre de centraliser au maximum les opérations.  
- Le bot doit être efficace pour notifier les parties concernées, sans pour autant devenir trop oppressant.
- Le bot doit journaliser toutes les opérations (pour les statistiques et le débogage).  
- Le bot doit être capable de gérer automatiquement les nouvelles promos.  
- Le bot doit être capable de gérer automatiquement les nouvelles formations.  
- Le bot doit accorder le droit d'utiliser certaines commandes sous certaines conditions (exemple : le vote uniquement pour les rôles apprenant ET type de promo).   
- **Performance** : le bot doit être performant sur un serveur VPS avec une petite configuration matérielle.  
- Le bot doit créer les premiers messages de vote dans les canaux signature afin d'éviter les problèmes de performance.

## La Problèmatique
Le rappel de la signature est peu intuitif : 
- le coach doit rechercher dans une longue liste de noms pour rappeler un apprenant à l'ordre. 
- le coach peut oublier de lancer le code de la signature.
- les apprenants oublient de signer.

<table>
    <tr>
        <td>Problématiques</td>
        <td>Problèmes</td>
        <td>Conséquences</td>
    </tr>
    <tr>
        <td rowspan="5">Oubli de signatures</td>
        <td>Rattrapages</td>
        <td>Perte de temps</td>
    </tr>
    <tr>
        <td>Absence injustifiée</td>
        <td>Perte de rémunération</td>
    </tr>
    <tr>
        <td>Remise en cause du sérieux de Simplon</td>
        <td>Perte de financements</td>
    </tr>
    <tr>
        <td>Difficulté à cibler les apprenants</td>
        <td>Perte de temps <br> Risque d'oublis</td>
    </tr>
    <tr>
        <td>Demander un envoi de signature au formateur</td>
        <td>Perte de temps <br> Risque d'oublis</td>
    </tr>
    <tr>
        <td rowspan="2">Outils de signatures externes</td>
        <td>Outils différents</td>
        <td>Dispersion entre les plateformes</td>
    </tr>
    <tr>
        <td>Rappels officiels pas assez efficaces</td>
        <td>Surcharge de travail administratif</td>
    </tr>
</table>