# Projet de Clustering : Segmentation de Clients

Ce projet utilise des techniques de Machine Learning non supervisé pour segmenter une base de données clients en groupes distincts et homogènes. L'objectif est de découvrir des structures cachées dans les données pour permettre un ciblage marketing plus efficace.

L'analyse est menée à l'aide de l'algorithme **K-Means** pour le clustering, et les résultats sont visualisés en 2D grâce à des techniques de réduction de dimension comme la **PCA** et le **t-SNE**.

---

##  Contexte et Objectifs

En marketing, comprendre les différents types de clients est fondamental. Ce projet vise à :

1.  **Identifier des segments de clients** basés sur leurs caractéristiques démographiques et comportementales (âge, profession, dépenses, etc.).
2.  **Appliquer un prétraitement rigoureux** des données, une étape cruciale pour les algorithmes basés sur la distance.
3.  **Déterminer le nombre optimal de clusters** à l'aide de la méthode du coude (Elbow Method).
4.  **Visualiser les clusters** de manière intuitive pour faciliter leur interprétation.
5.  **Créer des "personas" business** pour chaque segment afin de guider les stratégies marketing.

---

##  Technologies et Librairies

- **Langage :** Python 3.9+
- **Analyse de données :** Pandas, NumPy
- **Machine Learning :** Scikit-learn (KMeans, StandardScaler, PCA, TSNE)
- **Analyse exploratoire :** Jupyter Lab
- **Visualisation :** Matplotlib, Seaborn

---

## Installation et Lancement de l'Analyse

Suivez ces étapes pour reproduire l'analyse sur votre machine.

### 1. Prérequis

- Avoir [Git](https://git-scm.com/) et [Python](https://www.python.org/downloads/) (version 3.9+) installés.

### 2. Cloner le Dépôt

```bash
git clone https://github.com/ton-nom-utilisateur/segmentation-clients-clustering.git
cd Customer_Clustering
```

### 3. Créer l'Environnement et Installer les Dépendances

```bash      
    # Créer un environnement virtuel
    python -m venv venv

    # Activer l'environnement
    # Sur Windows : 
    venv\Scripts\activate
    # Sur macOS/Linux : 
    source venv/bin/activate

    # Installer les librairies
    pip install -r requirements.txt
```
    

### 4. Lancer Jupyter Lab

Pour explorer le notebook contenant l'analyse complète :
 ```bash     
    jupyter lab
```


Naviguez ensuite vers le dossier notebooks/ et ouvrez Custom_Segmentation.ipynb.
Résultats : **Les 4 Segments de Clients**

L'analyse a révélé 4 segments de clients distincts et pertinents :

| Persona	Profil | Démographique | Comportement d'Achat & Profession |
|-----------|-----------|-----------|
| 1. Le Cœur du Marché (Professionnels Variés) | Âge moyen (47 ans), mariés, diplômés. | Dépenses moyennes. Professions très diverses (Ingénieurs, Cadres...). |
| 2. Les Jeunes à Potentiel (Secteur Santé) | Très jeunes (27 ans), célibataires, vivent en famille. | Dépenses très faibles. Forte concentration dans la santé. |
| 3. Les Avocats Seniors | Le plus âgé (76 ans), mariés. | Dépenses élevées. 100% sont avocats. |
| 4. Les Personnes au Foyer | Milieu de vie (38 ans), principalement des femmes mariées. | Dépenses contrôlées. 100% sont des "Homemakers". |
 	

**Visualisation des Clusters (avec t-SNE)**

La visualisation avec t-SNE a confirmé l'existence de ces 4 groupes bien séparés, prouvant la pertinence de la segmentation.

**Conclusion**

Ce projet démontre comment le clustering peut transformer des données brutes en intelligence stratégique, permettant à une entreprise de personnaliser ses actions marketing et d'optimiser ses ressources.