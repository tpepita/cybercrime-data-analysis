# Criminal Data Mining Research | Analyse de données criminelles

**Python · WEKA · Data Mining · Interpretable Rules · Research**

> **Publication status / Statut de publication :** This repository package is a **private review draft**. Do not publish the `src/` scripts before confirming permission to redistribute research code from the original private GitLab project. / Cette archive est une **version de préparation privée** : ne publiez pas les scripts `src/` sans avoir confirmé l'autorisation de diffusion du code issu du GitLab privé.

## 🇫🇷 Présentation

Projet de recherche académique sur l'analyse de données relatives aux crimes et délits enregistrés en France, avec exploration de méthodes de fouille de données et de règles interprétables dans **WEKA**. Le dépôt de travail contient également des scripts **Python** permettant de lire et comparer les règles issues de **MODLEM** et **RandomTree** entre différentes années ou fichiers.

L'objectif des scripts est notamment de comparer des ensembles d'indices présents dans les règles et de mesurer leur similarité, avec ou sans prise en compte des classes, selon le script.

**Ma contribution :** développement des scripts Python de comparaison de règles (déclaration personnelle de Tyrone Paviot). Le travail scientifique et la publication sont collectifs ; les autres contributions ne sont pas revendiquées ici.

### Contenu technique
- `src/compar_modlem_index.py` : extraction et comparaison de règles MODLEM par indices.
- `src/compar_modlem_index_class.py` : comparaison des règles MODLEM tenant compte de la classe.
- `src/compar_randomTree.py` : comparaison de règles RandomTree tenant compte de la classe.
- `src/compar_randomTree_index.py` : comparaison RandomTree fondée sur les indices, indépendamment de la classe.

**Remarque :** Les scripts demandent des chemins de fichiers en entrée. L'archive de portfolio ne contient volontairement ni bases de données, ni exports complets de règles, ni vidéos, ni fichiers de présentation du projet collectif.

### Sources et référence scientifique
- Données d'origine (catalogue public) : [Crimes et délits enregistrés depuis 2012 – data.gouv.fr](https://www.data.gouv.fr/fr/datasets/crimes-et-delits-enregistres-par-les-services-de-gendarmerie-et-de-police-depuis-2012/)
- Publication scientifique collective : [Notice HAL](https://hal.science/hal-05500073/) · [Article PDF](https://www.lrde.epita.fr/dload/papers/meddouri.25.atelier.gast.pdf)
- Projet GitLab d'origine (accès éventuellement restreint) : [2024_cyber_criminality_1.0](https://gitlab.com/nidameddouri/2024_cyber_criminality_1.0)

### Exécution (après autorisation de publication)
```bash
python src/compar_modlem_index.py
python src/compar_modlem_index_class.py
python src/compar_randomTree.py
python src/compar_randomTree_index.py
```
Ces scripts utilisent la bibliothèque standard Python. Ils demandent des fichiers d'export WEKA au format attendu ; des tests reproductibles sur jeux de données d'exemple restent à ajouter.

---

## 🇬🇧 Overview

Academic research project studying recorded crime and offense data in France using **WEKA**, data mining and interpretable rules. The original project also includes **Python** scripts that parse and compare rule outputs from **MODLEM** and **RandomTree**, across files or years.

The scripts compare index sets in extracted rules and calculate similarity scores, optionally taking the predicted class into account.

**My contribution:** I developed the Python rule-comparison scripts (as stated by Tyrone Paviot). The research project and scientific publication are collaborative, and no claim is made over other contributors' work.

### Scripts
- `src/compar_modlem_index.py`: extract and compare MODLEM rules by index.
- `src/compar_modlem_index_class.py`: MODLEM comparisons incorporating class labels.
- `src/compar_randomTree.py`: compare RandomTree outputs incorporating class labels.
- `src/compar_randomTree_index.py`: compare RandomTree outputs by index only.

**Scope:** This draft excludes original datasets, complete generated results, research slides and videos. The scripts prompt for locally available input files in the expected format.

### References
- [French official data catalog](https://www.data.gouv.fr/fr/datasets/crimes-et-delits-enregistres-par-les-services-de-gendarmerie-et-de-police-depuis-2012/)
- [Collective research publication (HAL)](https://hal.science/hal-05500073/) · [Paper PDF](https://www.lrde.epita.fr/dload/papers/meddouri.25.atelier.gast.pdf)
- [Original research GitLab project](https://gitlab.com/nidameddouri/2024_cyber_criminality_1.0)

### Running the scripts (after permission is confirmed)
```bash
python src/compar_modlem_index.py
python src/compar_modlem_index_class.py
python src/compar_randomTree.py
python src/compar_randomTree_index.py
```
Only Python's standard library is imported by these four scripts. Reproducible demonstrations and tests with publishable sample data have not yet been added.

---

**Attribution / Crédits:** Scientific publication and methodology: original research authors and team, as identified in the linked publication. Python comparison scripts: Tyrone Paviot (author's statement). No open-source license has been assigned to this draft.
