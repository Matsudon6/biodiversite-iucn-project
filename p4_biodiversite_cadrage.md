# Projet 4 — Biodiversité et espèces menacées

## Objectif

Analyser les facteurs de menace sur la biodiversité mondiale et produire des visualisations géographiques des espèces menacées.

---

## Sources de données

- **IUCN Red List**  
  - https://www.iucnredlist.org/resources/spatial-data-download
  - Login : matsudon6@gmail.com
  - password : iucnredlist6
  - Données : statuts de conservation, catégories de menace, répartition géographique (shapefiles)
  
- **Sources complémentaires (optionnel pour plus tard) :**
  - GBIF.org (données d'observations)
  - UNEP-WCMC (écosystèmes mondiaux)
  - OurWorldInData.org (indicateurs environnementaux globaux)

---

## Stack technique

- pandas
- geopandas
- shapely
- matplotlib / seaborn
- plotly / folium
- scikit-learn (si modélisation ultérieure)

---

## Questions exploratoires

- Répartition géographique des espèces menacées (cartes, heatmaps)
- Comparaison par continents / régions
- Analyse par groupes taxonomiques (mammifères, oiseaux, reptiles…)
- Identification des zones de forte vulnérabilité

---

## Étapes de travail

1. Téléchargement des données
2. Chargement des shapefiles en Python
3. Nettoyage des données et premières analyses descriptives
4. Visualisations géographiques interactives
5. (optionnel) Modélisation ou scoring de risque

---

## Sprint 1 (2 semaines)

| Étape | Deadline cible |
|-------|-----------------|
| Téléchargement & setup des données | d’ici 3-4 jours |
| Premiers chargements et EDA simple | sous 1 semaine |
| Premières cartes de visualisation | sous 10-14 jours |

---

## Actions en cours

- ✅ Choix du projet validé (12 juin 2025)
- 🔲 Téléchargement des shapefiles IUCN Red List
- 🔲 Setup environnement Python


# Phase 2 — Setup environnement Python

## 📁 Structure de projet recommandée

Créer les dossiers suivants dans ton projet local :

/Mon_Portfolio_DataScience/
    /Projet_4_Biodiversite/
        /data/
        /notebooks/
        /scripts/
        README.md
        requirements.txt

---

## 🐍 Création de l’environnement Python

1️⃣ Créer un environnement virtuel (optionnel mais conseillé) :

Sous Mac/Linux :

    python -m venv venv
    source venv/bin/activate

Sous Windows :

    python -m venv venv
    venv\Scripts\activate

2️⃣ Mettre à jour pip :

    pip install --upgrade pip

3️⃣ Installer les packages de base nécessaires :

    pip install pandas geopandas matplotlib seaborn plotly folium jupyter

4️⃣ (Facultatif mais conseillé) : créer un fichier requirements.txt pour documenter ton environnement :

    pip freeze > requirements.txt

---

## 🧪 Test de l’environnement

Lancer un Jupyter Notebook :

    jupyter notebook

Créer un notebook de test dans /notebooks/ :  
Ex : `test_geopandas.ipynb`

Et tester le chargement de geopandas :

```python
import geopandas as gpd

print(gpd.__version__)
