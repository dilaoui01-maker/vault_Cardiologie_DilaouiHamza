# Documentation, Vault Cardiologie

## 1. Organisation du Vault
Le Vault est structuré par dossiers thématiques :

1. **Anatomie** : notes sur le cœur, les vaisseaux, le myocarde et le système coronaire  
2. **Physiologie** : cycle cardiaque, conduction électrique, pression artérielle  
3. **Pathologies_cardiovasculaire** : hypertension, insuffisance cardiaque, infarctus, troubles du rythme  
4. **Cas_cliniques** : exemple de patient avec ces pathologies ainsi que les traitements  
5. **Traitements** : IEC, ARA2, bêtabloquants, anticoagulants
---

## 2. Plugins
- **CSS** : utilisation de couleurs, titres, mise en page  
- **Advanced Slides** : pour créer la présentation avec des diapositives 
- **Canvas** : création de schéma pour faciliter la comprehension du contenu du vault 
- **Dataview** : extraction dynamique et création d'un tableau des notes importantes 
- **Templates** : notes standardisées pour homogénéiser la mise en forme  
- **Lien interne** :  les notes sont interconnectées  

---

## 3. Dataview
Une note Dataview liste les notes par thème grâce au plugin Dataview . Le bloc de dataview utilisé est :

```dataview
TABLE file.link AS "Note", file.folder AS "Dossier", file.tags AS "Tags"
FROM #anatomie OR #physiologie OR #pathologie OR #cas_clinique OR #traitement
SORT file.folder ASC
