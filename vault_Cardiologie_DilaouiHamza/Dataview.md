# Dashboard – Cardiologie

La note permet de centralisée l’ensemble des contenus du Vault .Elle permet une meilleure navigation grâce aux liens entre les dossiers . Le tableau en-dessous est généré avec le plugin dataview , il montre comment le vault est organisé.

```dataview
TABLE file.link AS "Note", file.folder AS "Dossier"
FROM "1-Anatomie" OR "2-Physiologie" OR "3-Pathologies_cardio" OR "4-Cas_cliniques" OR "5-Traitements"
SORT file.folder ASC
```
