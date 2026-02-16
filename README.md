# medicaments-ruptures-france-2017-2026
Analyse des événements de disponibilité des médicaments en France (2014–2026) – Power BI
# Analyse des tensions d’approvisionnement des médicaments en France (2014–2026)

## Contexte
Depuis 2017, la France connaît une augmentation des ruptures et tensions d’approvisionnement en médicaments.  
Ce projet analyse les données ouvertes de data.gouv.fr afin d’identifier les tendances, les médicaments et les laboratoires les plus impactés.

## Objectifs
- Analyser l’évolution des événements de disponibilité
- Identifier les types d’événements dominants
- Analyser les laboratoires les plus concernés
- Mettre en évidence les tendances temporelles

## Source des données
- data.gouv.fr – Données ouvertes sur la disponibilité des médicaments
- Période : 2014–2026
- Format : txt

## Outils utilisés
- Power BI
- Power Query
- DAX
- Excel

## Analyses réalisées
- Évolution annuelle des ruptures et tensions
- Répartition par type d’événement
- Top 10 des laboratoires les plus impactés
- Analyse des remises à disposition et arrêts de commercialisation

## Aperçu du dashboard & analyses

### B)les laboratoires qui ont subi des évenements

### 1)Dashborad Synthètique

![Synthese](screenshot/Synthese_evenement.png)

**Analyse :**
On observe une augmentation progressive des tensions d’approvisionnement à partir de 2019, 
avec un pic marqué après 2020, suggérant un impact des perturbations de la chaîne logistique.

---

### 2)Top 10 des laboratoires fabriquant le plus grand nombre de spécialités
![Top 10 des laboratoires au plus gros portefeuille](screenshot/Top_10_des_laboratoires_fabricants.png)

**Analyse :**
Une concentration importante des événements est observée chez un nombre limité de laboratoires,
ce qui indique un risque systémique lié à certains acteurs clés du marché.

---

### 3)Répartition par type d’événement
### Rupture de stock
![Rupture_de_stock](screenshot/Rupture_de_stock.png)

**Analyse :**
Les tensions d’approvisionnement représentent la majorité des événements, tandis que les
arrêts de commercialisation restent minoritaires.

### Tension d'approvissionnement
![Tension](screenshot/Tension_d'approvisionnement.png)

**Analyse :**
Les tensions d’approvisionnement représentent la majorité des événements, tandis que les
arrêts de commercialisation restent minoritaires.

### Remise à disposition 
![Remise à disposition](screenshot/Remise_a_disposition.png)

**Analyse :**
Les tensions d’approvisionnement représentent la majorité des événements, tandis que les
arrêts de commercialisation restent minoritaires.

### Arrêt de commercialisation
![Arret de commercialisation](screenshot/Arret_de_commercialisation.png)

**Analyse :**
Les tensions d’approvisionnement représentent la majorité des événements, tandis que les
arrêts de commercialisation restent minoritaires.

### 4)Évolution des événements et prévision
![Évolution](screenshot/evolution_evenements.png)

**Analyse :**
On observe une augmentation progressive des tensions d’approvisionnement à partir de 2019, 
avec un pic marqué après 2020, suggérant un impact des perturbations de la chaîne logistique.

### B)les laboratoires sans évenement
### Synthèse des Non_événements
![Synthese_de_non_evenement](screenshot/Synthese_de_non_evenement.png)

**Analyse :**
On observe une augmentation progressive des tensions d’approvisionnement à partir de 2019, 
avec un pic marqué après 2020, suggérant un impact des perturbations de la chaîne logistique.

### 1)Suspension d'autorisation
![Autorisation suspendue](screenshot/Autorisation_suspendue.png)

**Analyse :**
On observe une augmentation progressive des tensions d’approvisionnement à partir de 2019, 
avec un pic marqué après 2020, suggérant un impact des perturbations de la chaîne logistique.

---
### Retraits d'autorisation
![Autorisation retiree](screenshot/Autorisation_retiree.png)

**Analyse :**
On observe une augmentation progressive des tensions d’approvisionnement à partir de 2019, 
avec un pic marqué après 2020, suggérant un impact des perturbations de la chaîne logistique.

---
### Archivage d'autorisation
![Autorisation_archivee](screenshot/Autorisation_archivee.png)

**Analyse :**
On observe une augmentation progressive des tensions d’approvisionnement à partir de 2019, 
avec un pic marqué après 2020, suggérant un impact des perturbations de la chaîne logistique.

---
### Autorisation actives
![Autorisations_actives](screenshot/Autorisations_actives.png)

**Analyse :**
On observe une augmentation progressive des tensions d’approvisionnement à partir de 2019, 
avec un pic marqué après 2020, suggérant un impact des perturbations de la chaîne logistique.---
### Abrogation d'autorisation
![Autorisations_abrogées](screenshot/Autorisations_abrogées.png)

**Analyse :**
On observe une augmentation progressive des tensions d’approvisionnement à partir de 2019, 
avec un pic marqué après 2020, suggérant un impact des perturbations de la chaîne logistique.

---
### Prédiction
![Visuels_prédiction](screenshot/Visuels_prédiction.png)

**Analyse :**
🔎 Lecture globale du dashboard

Ce tableau de bord analyse les événements de disponibilité des médicaments en France (ruptures, arrêts, tensions…) selon le statut AMM, le temps et les laboratoires titulaires, avec une approche à la fois descriptive et prédictive.

1️⃣ Nombre de laboratoires sans événement par statut AMM (graphique en cascade – en haut à gauche)
Ce que l’on observe
- La majorité des laboratoires sans événement concernent des médicaments à autorisation active.
- Les statuts abrogée, archivée, retirée ou suspendue contribuent marginalement.
- Le total montre qu’un volume important de titulaires n’a jamais déclaré d’événement.

### Interprétation métier
Les médicaments encore actifs sont globalement bien maîtrisés.
Les statuts non actifs concentrent peu de laboratoires → soit parce qu’ils sont peu nombreux, soit parce qu’ils ne génèrent plus d’événements.

### Insight clé
L’absence d’événements est fortement corrélée à un statut AMM actif, ce qui suggère une meilleure stabilité réglementaire et logistique.

2️⃣ Nombre d’événements par année et statut AMM (courbe – en haut à droite)
L'on peut voir:
- Une quasi-absence d’événements avant 2020.
- Une forte hausse à partir de 2021, avec un pic très marqué en 2024–2025, principalement sur les autorisations actives.
- Une chute brutale en 2026 (car année en cours donc incomplète).

### Interprétation métier
Effet post-crise (COVID, tensions logistiques, matières premières, dépendance aux API).
Les médicaments actifs sont les plus exposés, car ils sont les plus consommés.

### Insight clé
Le risque de rupture est devenu structurel et récent, concentré sur les AMM actives, ce qui justifie une approche prédictive plutôt que seulement descriptive.

3️⃣ Nombre total de spécialités vs nombre d’événements par titulaire AMM (nuage de points – en bas à gauche)
Ce que l’on observe

Corrélation positive : plus un laboratoire a de spécialités, plus il a d’événements.
Mais la relation n’est pas parfaitement linéaire : certains labos avec peu de spécialités ont beaucoup d’événements; d’autres très gros portefeuilles restent relativement stables

### Interprétation métier
La taille du portefeuille à lui seul n’explique pas tout. Des facteurs internes (organisation, sites de production, dépendance fournisseurs) joueraient un rôle.

### Insight clé
Le risque d’événement dépend à la fois du volume de spécialités et de la qualité de la chaîne d’approvisionnement du laboratoire.

4️⃣ Nombre d’événements vs événements par spécialité (nuage de points – en bas à droite)
L’on observe une forte concentration des points en bas à gauche : peu d’événements, donc faible taux d’événements par spécialité.
Quelques outliers avec beaucoup d’événements, mais un ratio événement/spécialité parfois faible

### Interprétation métier
Les gros laboratoires absorbent mieux les événements (effet dilution du au large portefeuille).
Les petits portefeuilles avec plusieurs événements sont à haut risque.

### Insight clé
Le ratio événement/spécialité est un meilleur indicateur de risque que le nombre brut d’événements.

5️⃣ Commentaire prédictif 

Ces visualisations justifient l’utilisation d’un modèle de loi de Poisson, car :
les événements sont discrets
rares
indépendants
observés sur une période donnée

Il etait ensuite judicieux de :
la probabilité d’au moins une rupture par DCI ou laboratoire
le nombre attendu d’événements à 3 ou 6 mois
identifier les DCI à risque élevé

---
## 🔍 Principaux insights
- Augmentation significative des tensions après 2020
- Concentration des événements chez certains laboratoires
- Les remises à disposition 

## 🚀 Améliorations possibles
- Modèle de prévision des tensions
- Croisement avec données ANSM
- Classification par classe thérapeutique

## 👤 Auteur
Georgy Djounda – Data Analyst / Pharmacien
