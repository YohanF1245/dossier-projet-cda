# Pourquoi une Base de Données PostgreSQL?

| Stat                       | MySQL                             | PostgreSQL                                      |
| -------------------------- | --------------------------------- | ----------------------------------------------- |
| GH stars                   | 10.9k                             | 16.2k                                           |
| FLast commit               | 2 months ago                      | 10 minutes ago                                  |
| Fork                       | 3.9k                              | 4.6k                                            |
| Architecture               | Relationnel                       | Relationnel & objet                             |
| Prix                       | Certaines fonctionnalité payantes | Totalment gratuit                               |
| Performance                | Rapide pour des bdd simples       | Plus performant sur des gros volumes de données |
| Language SQL               | Compatibilité restreinte          | Compatibilité accrue                            |
| Stack overflow survey 2023 | 41.09%                            | 45.55%                                          |
| Licence                    | PostgreSQL (semblable à MIT)      | GPL                                             |
| Transaction ACID           | OUI                               | OUI                                             |
| Support des extensions     | +                                 | +++ |

Pour l'application le choix de postgreSQL s'avère rationnel en raison de sa popularité, de sa scalabité, et de sa robustesse.<br>
PostgreSQL respecte les standards SQL , qui lui permet de construire des requêtes plus complexes et avancées. <br>
De plus postgreSQL est sous license open source ce qui permet plus de flexibilité dans l'utilisation et garanti la totale gratuité pour l'utilisation.<br>
Le système etant complexe car composé de plus bots allant interragir de manière concurrentielle avec la base de données, postgreSQL aura un avantage de performance sur MySQL grace à sa meilleur gestion des transactions concurrentes.<br>
Les données de Discord sont au format JSON, postgreSQL gérant le format JSON nativement il sera plus performant que MySQL dans le traitement de ces données.

## Benchmark de Performance (source: bytebase.com)

| Opération                  | MySQL                             | PostgreSQL                                      |
| -------------------------- | --------------------------------- | ----------------------------------------------- |
| Insertion simple           | Plus rapide (+15%)                | Base de référence                               |
| Insertion en batch         | Plus lent (-20%)                  | Base de référence                               |
| Lecture simple             | Similaire                         | Similaire                                       |
| Lecture avec JOIN          | Plus lent (-10%)                  | Base de référence                               |
| UPDATE avec index          | Plus rapide (+5%)                 | Base de référence                               |
| DELETE en masse            | Plus lent (-25%)                  | Base de référence                               |
| Requêtes complexes         | Plus lent (-30%)                  | Base de référence                               |
| Performances sous charge   | Dégradation plus rapide           | Meilleure stabilité                             |
| Utilisation mémoire        | Plus efficace (+20%)              | Base de référence                               |
| Utilisation CPU           | Plus efficace (+10%)              | Base de référence                               |