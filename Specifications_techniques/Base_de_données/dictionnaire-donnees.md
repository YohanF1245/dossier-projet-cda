# Dictionnaire de données
### Introduction

Un dictionnaire de données est un référentiel de métadonnées qui fournit le contexte nécessaire à la compréhension d'une base de données. Il offre des informations essentielles sur la structure et l'organisation des données, facilitant ainsi leur gestion. Cet outil est crucial pour les administrateurs et les utilisateurs, car il leur permet d'interpréter et d'exploiter efficacement les données.

| Entité   | Attribut      | Type de Données | Longueur | Contraintes | Description                                  | Exemple                                |
| -------- | ------------- | --------------- | -------- | ----------- | -------------------------------------------- | -------------------------------------- |
| Users    | user_sf_id    | BYTE            | 18       | PRIMARY KEY | Identifiant unique de l'utilisateur          | 123456789012345678                     |
| Roles    | role_sf_id    | BYTE            | 18       | PRIMARY KEY | Identifiant unique du rôle                   | 234567890123456789                     |
|          | role_name     | VARCHAR         | 50       | -           | Nom du rôle                                  | "Admin"                                |
| Channels | channel_sf_id | BYTE            | 18       | PRIMARY KEY | Identifiant unique du canal                  | 345678901234567890                     |
|          | channel_name  | VARCHAR         | 50       | -           | Nom du canal                                 | "Email"                                |
|          | channel_type  | INT             | -        | -           | Type de canal aud niveau de l'api discord(message, forum, etc...) | 1                                      |
| Promos   | promo_id      | UUID            | -        | PRIMARY KEY | Identifiant unique de la promotion           | "550e8400-e29b-41d4-a716-446655440000" |
|          | promo_name    | VARCHAR         | 50       | -           | Nom de la promotion                          | "Promo Été 2023"                       |
|          |               |                 |          |             |                                              |                                        |