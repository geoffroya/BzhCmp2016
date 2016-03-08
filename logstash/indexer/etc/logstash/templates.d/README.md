# Templates

Je propose 3 templates :
- **default-template.json** : le template par défaut
- **default-optimized-template.json** : Ce template d'analyze pas les champ de type string, sauf s'il s'appelle **detail**. Le principe est qu'on ne va pas faire de recherche full-text sur un niveau de log par exemple. Par contre l'analyse du **detail** du message est pertinente pour faire des recherche full-text dessus.
- **grokparsefailure-template.json** : les logs qui n'ont pas pu être parsés sont stockés dans un autre index. Ce template permet de réduire l'espace occupé par cet index en limitant les données analysées.

Les templates permettent également de configurer l'index au niveau sharding et réplication.
