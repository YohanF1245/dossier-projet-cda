# Introduction

- 1 [À propos de moi](#à-propos-de-moi)
- 2 [À propos du client](#à-propos-du-client)
- 3 [Le projet](#le-projet)

## À propos de moi.

Mon parcours professionnel a commencé avec l'obtention d'un diplôme de Technicien de Maintenance Informatique, où j'ai acquis une solide maîtrise des techniques de maintenance et de dépannage du matériel informatique, ainsi que des notions en réseau. Ce premier pas dans le domaine de l'informatique m'a permis de développer une base technique essentielle et une compréhension approfondie des infrastructures matérielles et des systèmes de réseaux.<br>

Cherchant toujours à élargir mes horizons et à approfondir mes compétences, j'ai ensuite entrepris un Diplôme d'Accès aux Études Universitaires (DAEU). Cette étape cruciale m'a ouvert la voie vers un Diplôme d'études universitaires scientifiques et techniques Informatique d'organisation et systèmes d'information (DEUST IOSI), où j'ai pu me plonger dans l'univers de la programmation. Cette formation m'a permis de découvrir ma passion pour le code et de renforcer mes compétences techniques.<br>

Autodidacte par nature, j'ai continuellement cherché à élargir mes connaissances et à perfectionner mes compétences en explorant diverses technologies. Je me suis ainsi familiarisé avec les technologies de backend et de frontend, ainsi qu'avec le développement d'applications desktop. Mon aisance avec les bases de données complète cette palette de compétences, me permettant d'aborder des projets complexes avec une vision globale et une expertise technique.<br>

Aujourd'hui, fort de ce parcours diversifié et enrichissant, je me fixe un nouvel objectif ambitieux : reprendre mes études dans le but d'obtenir un titre de Concepteur Développeur d'Applications. Cette nouvelle étape représente pour moi un défi stimulant, en phase avec mon aspiration constante à évoluer et à me perfectionner.<br>

Je suis animé par une grande détermination et une soif de challenge. Mon sérieux et mon engagement me poussent à toujours donner le meilleur de moi-même dans chaque projet que j'entreprends. Je crois fermement que chaque défi est une opportunité d'apprentissage et de croissance.<br>
<br>

## À propos du client.

Simplon est un réseau de fabriques numériques et inclusives, implanté en France et à l'international. Depuis 2013, plus de 30 000 apprenants ont été formés, dont 30 % de femmes et 46 % de personnes peu ou pas diplômées. En tant qu'entreprise sociale et solidaire, l'objectif de Simplon est de faire du numérique un levier d'inclusion, en révélant des talents sous-représentés dans le secteur digital et les métiers techniques. Simplon accompagne les organisations dans leur transformation numérique, en veillant à ce qu'elle soit inclusive. En parallèle, l'entreprise contribue également à la médiation numérique et à l'apprentissage créatif des technologies auprès des enfants.

## Le projet.

Le système se décompose comme suit :

- Une base de données qui contient les informations des utilisateurs (identité,promotion, formation, etc...)
- Un dashboard qui permet de visualiser les information concernant les bots et modifieur leur configuration
- Les bots qui permettent d'automatiser des tâches récurrentes liées à la gestion des promotions :
    - Un bot onboarding qui permet de créer des promotions et de les configurer
    - Un bot signature qui permet de rapidement prévenir les oublis d'émargement
    - Un bot feedback qui permet de collecter les retours des apprenants
    - Un bot community qui permet de gérer les partages de ressources




# Expression du besoin
La communication est la pierre angulaire du fonctionnement de toute organisation. Dans le cas de Simplon, s'assurer d'une communication fluide est crucial, aussi bien verticalement qu'horizontalement. La complexité de la circulation peut être résumée dans le schéma simplifié ci-dessous.
![image](/./assets/img/schema-communication.png)
Il est à noter que si la distance physique entre les divers centres de formation et entre les centres et les alumni paraît évidente, une autre distanciation apparaît avec les formations ouvertes à distance, ce qui renforce encore le besoin d'un système de communication béton.<br>
Le plan à long terme est de former une communauté dans le but de créer du mentorat entre alumni et apprenants et de créer un canal de recrutement pour les entreprises. Cela mettra de surcroît l'accent sur la collaboration et le partage qui sont des principes clés dans le monde du développement (l'un des meilleurs exemples est le principe de l'open source qui colle parfaitement au mindset des valeurs susnommées).<br>
Le choix d'une plate-forme de communication s'avère compliqué car il faut tenir compte de plusieurs critères. Discord, malgré ses défauts que nous détaillerons plus bas, a été le meilleur compromis pour sa gratuité, son agnosticisme de plate-forme ainsi que sa popularité.


