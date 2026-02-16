# PRIMA – Exercice technique  
Ce dépôt contient ma proposition pour l’extraction et la normalisation d’informations issues de catalogues de manuscrits italiens.

## Objectifs
Transformer des descriptions textuelles hétérogènes en données structurées, réutilisables pour la recherche.

Cibles principales :
- Dates  
- Dimensions  
- Entités nommées (personnes, organisations)

## Méthode
Je combine trois approches complémentaires :

- **Regex / règles** → transparentes et contrôlables  
- **spaCy NER** → base statistique  
- **Extraction par LLM** → flexibilité sémantique  

Les cas incertains sont consignés pour expertise humaine plutôt que décidés automatiquement.

## Livrables
- `PRIMA_Exercice.ipynb` → pipeline, explications, évaluation  
- `entities_regex.csv`
- `entities_ner.csv`
- `entities_llm.csv`

## Évaluation
Les méthodes sont comparées à la vérité terrain à l’aide des métriques WER.
