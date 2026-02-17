# Medicaments-ruptures-france-2013-2026 
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

## Analyses réalisées
- Évolution annuelle des ruptures et tensions
- Répartition par type d’événement
- Top 5 des laboratoires les plus impactés
- Analyse des remises à disposition et arrêts de commercialisation

## Aperçu du dashboard & analyses

### A- les laboratoires qui ont subi des évenements

### 1) Dashborad Synthètique

![Synthese](screenshot/Synthese_evenement.png)

**Analyse :**
Sur la période allant de 2013 au début de l’année 2026, un total de 953 événements de disponibilité a été recensé. Ces événements concernent 142 laboratoires distincts, soit 21,2 % des 671 laboratoires présents dans le référentiel. L’année 2025 se distingue nettement comme la plus impactée, avec 580 événements, traduisant une forte dégradation de la disponibilité des médicaments sur cette période.

Les laboratoires les plus touchés en volume d’événements sont :

ARROW (66 événements),
VIATRIS SANTÉ (64),
EG LABO (58),
BIOGARAN (54),
TEVA SANTÉ (51),
suivis de SANDOZ (45).

Ces résultats soulignent une concentration des événements sur un nombre restreint d’acteurs, principalement positionnés sur le marché des médicaments génériques.

---

### 2) Répartition par type d’événement
### a) Rupture de stock
![Rupture_de_stock](screenshot/Rupture_de_stock.png)

**Analyse :**
Les ruptures de stock représentent 72 événements, soit 7,5 % de l’ensemble des événements observés entre 2013 et début 2026. Un pic marqué est observé en 2025, avec 34 ruptures de stock signalées, confirmant le caractère exceptionnel de cette année.

Les laboratoires les plus concernés sont :

-MYLAN (7 événements),
-BIOGARAN (6),
-TEVA SANTÉ (5),
-VIATRIS IRLANDE (4),
-LABORATOIRE DELBERT (3),
auxquels s’ajoutent 35 autres laboratoires touchés de manière plus ponctuelle.

Les ruptures attribuées à MYLAN peuvent être interprétées à la lumière de la disparition progressive de la marque au profit de VIATRIS depuis 2020, ce qui a pu générer des situations transitoires d’épuisement des stocks ou de requalification des titulaires.

### b) Tension d'approvissionnement
![Tensions](screenshot/Tension_d'approvisionnement.png)

**Analyse :**
Les tensions d’approvisionnement constituent une part majeure des événements recensés, avec 418 occurrences, soit 43,82 % du total. Elles concernent 82 laboratoires sur la période 2021–2026, traduisant une problématique récente mais persistante. L’année 2024 apparaît comme la plus critique, avec 148 tensions signalées.

Les laboratoires les plus affectés sont :

-ARROW (30),
-EG LABO (29),
-VIATRIS SANTÉ (27),
-ZENTIVA SANTÉ (23),
-BIOGARAN (22).

Ces résultats confirment le rôle central des génériqueurs dans les situations de tension, probablement en lien avec des chaînes d’approvisionnement fortement internationalisées.

### c) Remise à disposition 
![Remise à disposition](screenshot/Remise_a_disposition.png)

**Analyse:** 
Les remises à disposition représentent 422 événements, soit 44,23 % du total, constituant ainsi la catégorie la plus fréquente.

Elles concernent 82 laboratoires, dont principalement :

-ARROW (35),
-VIATRIS (34),
-EG LABO,
-GLAXOSMITHKLINE,
-TEVA SANTÉ (28),
-SANDOZ (27),
-BIOGARAN (21).

Ce volume élevé de remises à disposition traduit une dynamique de sortie de crise, mais également une instabilité chronique, avec des alternances fréquentes entre tension, rupture et retour à une situation normale.

### d) Arrêt de commercialisation
![Arret de commercialisation](screenshot/Arret_de_commercialisation.png)

**Analyse :**
Un total de 42 arrêts de commercialisation a été recensé, soit 4,5 % des événements, impliquant 12 laboratoires. L’année 2025 concentre à elle seule 21 arrêts, ce qui constitue un niveau particulièrement élevé.

Les laboratoires les plus concernés sont :

-IBSA PHARMA (12 spécialités),
-Assistance Publique – Hôpitaux de Paris (9),
-PFIZER (4),
-BIOGARAN (2),
-SANOFI WINTHROP (2).

Ces arrêts peuvent refléter des choix stratégiques, des contraintes industrielles, ou une rentabilité insuffisante de certaines spécialités.
### e) Evenements orphelins
![Evenements Orphelins](screenshot/Evenements_orphelins.png)

**Analyse :**
Un nombre limité d’événements (19) n’a pu être rattaché ni à un titulaire d’AMM, ni à une spécialité médicamenteuse du référentiel CIS utilisé.

Ces événements s’expliquent principalement par :

-des évolutions du référentiel (codes CIS obsolètes ou retirés),
-des décalages temporels entre les sources,
-ou des valeurs manquantes dans les données d’origine.

Compte tenu de leur faible volume et de leur impossibilité de rattachement fiable, ces événements ont été exclus de l’analyse principale.

**Conclusion partielle:**

L’analyse met en évidence une dégradation marquée de la disponibilité des médicaments à partir de 2021, culminant en 2025, année caractérisée par une augmentation significative des ruptures, des tensions d’approvisionnement et des arrêts de commercialisation.

Les événements se concentrent sur un nombre restreint de laboratoires, majoritairement des génériqueurs, soulignant une vulnérabilité structurelle des chaînes d’approvisionnement pour ces acteurs.

Les événements orphelins, bien que marginaux en volume, sont intégrés aux données globales mais ne peuvent pas être ventilés selon les dimensions analytiques en raison de limites du référentiel CIS. Leur présence n’altère pas les tendances observées et témoigne des enjeux classiques de synchronisation et d’évolution des référentiels dans les analyses longitudinales.

Dans l’ensemble, les résultats obtenus offrent une vision robuste et cohérente des dynamiques de disponibilité des médicaments sur la période étudiée.



### B-les laboratoires sans évenement
L'absence d'événement peut être perçu comme une situation de normalité. Mais, nous avons jugé utile d'approfondir l'etude en consultant également les évenements dr la table de dimension DIM INFO MEDICAMENTS à titre descriptif pour en tirer quelques éléments d'analyse

### Synthèse des Non_événements
![Synthese_de_non_evenement](screenshot/Synthese_de_non_evenement.png)

**Analyse :**
Sur une période allant de 2013 au début 2026, près de 15.000 spécialités (DCI) reparties entre 529 laboratoire n'ont subi aucun événement. Le laboratoire BOIRON, 868 DCI dispose du plus gros portefeuille représentant 5,86% de tous les médicaments normo-distribués. Il est suivi dans ce top 5 par les laboratoires BIOGARAN (765,5,1%), VIATRIS SANTE(733, 4,95%), ARROW GENERIQUES(707, 4,77%) et EG LABO (612, 4,13%)

### 1)Autorisation actives
![Autorisations_actives](screenshot/Autorisations_actives.png)

## Analyse :
### Insight 1 — La stabilité est concentrée chez les grands génériqueurs
Sur plus de 15.000 spécialités, 14.000 stables sont repartis dans 501 laboratoires, soit 74,6% de tous les laboratoires de cette étude. 
Les laboratoires comme Biogaran, Viatris, Sandoz, Teva, Zentiva concentrent :un grand nombre de DCI, sans aucun événement déclaré. Cela suggère :une maîtrise industrielle et logistique, une robustesse des chaînes d’approvisionnement, une capacité à absorber la demande sans rupture

### Insight 2 — La majorité des DCI sans événement sont sous AMM active
Le filtre montre que la stabilité concerne surtout : des médicaments toujours commercialisés, donc réellement exposés au marché. L’absence d’événement n’est pas liée à l’inactivité réglementaire, mais à une vraie performance.

### Insight 3 — Un indicateur de “non-risque” exploitable
Cette analyse permet :
d’identifier les zones de faible risque, de servir de baseline pour comparer avec : DCI à risque élevé, titulaires plus instables

---
### 2)Suspension d'autorisation
![Autorisation suspendue](screenshot/Autorisation_suspendue.png)

**Analyse :**
Il y a aucours de la période d'étude 6 suspensions d'autorisation, touchant principalement 4 laboratoires principalement EG LABO, ZENTIVA, PFIZER
Ce faible pourcentage de suspension d'autorisation suggère une bonne maitrise des événements aucours du cycle de vie d'un médicament: etudes de stabilité, pharmacovigilance et la maitrise des affaires réglementaires

---
### 3)Retraits d'autorisation
![Autorisation retiree](screenshot/Autorisation_retiree.png)

**Analyse :**
7 Laboratoires ont vu leur autorisation retirée, les laboratoires majoritairement touchés sont ADVANZ PHARMA, MELISANA PHARMA et ZANBON FRANCE.
Ce chiffre conforte l'analyse portée sur les suspension d'autorisation des laboratoire: Une maîtrise du cycle de vie du médicament et des événements y liés

---
### 4)Archivage d'autorisation
![Autorisation_archivee](screenshot/Autorisation_archivee.png)

**Analyse :**
Ce dashboard présente les DCI n’ayant jamais fait l’objet d’un événement, associées à des AMM archivées, réparties par titulaire AMM

**Indicateurs clés** :
197 DCI sans événement, 70 laboratoires concernés, une répartition beaucoup plus fragmentée que pour les AMM actives

### Insights clés
### Insight 1 — Une stabilité résiduelle et dispersée
Contrairement aux AMM actives, aucun laboratoire ne concentre une part dominante, la majorité des titulaires ne possèdent que 1 à 3 DCI sans événement
👉 Cela reflète une stabilité résiduelle, liée à l’historique plutôt qu’à une stratégie active.

### Insight 2 — Différence structurelle avec les AMM actives
Les volumes sont nettement plus faibles (197 vs 14 000),Le nombre de laboratoires est aussi réduit (70 vs 501)
👉 Les AMM archivées jouent un rôle marginal dans la disponibilité actuelle du marché.

### Insight 3 — Faible enjeu opérationnel immédiat
Ces DCI ne sont plus activement commercialisées, n’impactent pas directement la continuité des soins. Elles doivent être exclues ou pondérées dans les modèles prédictifs.

### Limites et précautions méthodologiques
Les DCI associées à des AMM archivées présentent un faible intérêt prédictif en matière de rupture, leur statut limitant leur exposition réelle au marché.

---

### 5)Abrogation d'autorisation
![Autorisations_abrogées](screenshot/Autorisations_abrogées.png)

**Analyse :**
Ce dashboard présente les DCI n’ayant jamais fait l’objet d’un événement et associées à des autorisations de mise sur le marché abrogées, réparties par titulaire AMM.
## Indicateurs clés : ##
762 DCI sans événement, 134 laboratoires concernés. Une répartition hétérogène, avec une faible concentration par titulaire

### Insights clés
### Insight 1 — Un volume intermédiaire mais sans enjeu opérationnel actuel
Comparé aux autres statuts bien inférieur aux AMM actives, supérieur aux AMM archivées
👉 Cela reflète un historique réglementaire, plus qu’une performance actuelle.

### Insight 2 — Dispersion marquée des titulaires
Aucun laboratoire ne domine fortement, les parts individuelles restent faibles, beaucoup de titulaires n’ont que quelques DCI sans événement
👉 Contrairement aux AMM actives, il n’existe pas ici de leaders de stabilité.

### Insight 3 — Faible valeur prédictive
Les AMM abrogées ne sont plus exposées au marché, ne contribuent pas à la continuité des soins
👉 Leur inclusion dans un modèle prédictif biaiserait l’analyse.

---
### C -Prédiction
![Visuels_prédiction](screenshot/Visuels_prédiction.png)

**Analyse :**
🔎 Lecture globale du dashboard

Ce tableau de bord analyse les événements de disponibilité des médicaments en France (ruptures, arrêts, tensions…) selon le statut AMM, le temps et les laboratoires titulaires, avec une approche à la fois descriptive et prédictive.

## 1) Nombre de laboratoires sans événement par statut AMM (graphique en cascade – en haut à gauche)
Ce que l’on observe
- La majorité des laboratoires sans événement concernent des médicaments à autorisation active.
- Les statuts abrogée, archivée, retirée ou suspendue contribuent marginalement.
- Le total montre qu’un volume important de titulaires n’a jamais déclaré d’événement.

### Interprétation métier
Les médicaments encore actifs sont globalement bien maîtrisés.
Les statuts non actifs concentrent peu de laboratoires → soit parce qu’ils sont peu nombreux, soit parce qu’ils ne génèrent plus d’événements.

### Insight clé
L’absence d’événements est fortement corrélée à un statut AMM actif, ce qui suggère une meilleure stabilité réglementaire et logistique.

## 2) Nombre d’événements par année et statut AMM (courbe – en haut à droite)
L'on peut voir:
- Une quasi-absence d’événements avant 2020.
- Une forte hausse à partir de 2021, avec un pic très marqué en 2024–2025, principalement sur les autorisations actives.
- Une chute brutale en 2026 (car année en cours donc incomplète).

### Interprétation métier
Effet post-crise (COVID, tensions logistiques, matières premières, dépendance aux API).
Les médicaments actifs sont les plus exposés, car ils sont les plus consommés.

### Insight clé
Le risque de rupture est devenu structurel et récent, concentré sur les AMM actives, ce qui justifie une approche prédictive plutôt que seulement descriptive.

## 3) Nombre total de spécialités vs nombre d’événements par titulaire AMM (nuage de points – en bas à gauche)
Ce que l’on observe:
Corrélation positive : plus un laboratoire a de spécialités, plus il a d’événements.
Mais la relation n’est pas parfaitement linéaire : certains labos avec peu de spécialités ont beaucoup d’événements; d’autres très gros portefeuilles restent relativement stables

### Interprétation métier
La taille du portefeuille à lui seul n’explique pas tout. Des facteurs internes (organisation, sites de production, dépendance fournisseurs) joueraient un rôle.

### Insight clé
Le risque d’événement dépend à la fois du volume de spécialités et de la qualité de la chaîne d’approvisionnement du laboratoire.

## 4) Nombre d’événements vs événements par spécialité (nuage de points – en bas à droite)
L’on observe une forte concentration des points en bas à gauche : peu d’événements, donc faible taux d’événements par spécialité.
Quelques outliers avec beaucoup d’événements, mais un ratio événement/spécialité parfois faible

### Interprétation métier
Les gros laboratoires absorbent mieux les événements (effet dilution du au large portefeuille).
Les petits portefeuilles avec plusieurs événements sont à haut risque.

### Insight clé
Le ratio événement/spécialité est un meilleur indicateur de risque que le nombre brut d’événements.

## 5) Commentaire prédictif 

Ces visualisations justifient l’utilisation d’un modèle de loi de Poisson, car :
les événements sont discrets, rares, indépendants observés sur une période donnée
Il est judicieux pour la suite d'etudier :
-la probabilité d’au moins une rupture par DCI ou laboratoire
-le nombre attendu d’événements à 3 ou 6 mois
-identifier les DCI à risque élevé

---
## Principaux insights possibles en prédiction
- Augmentation significative des tensions après 2020
- Concentration des événements chez certains laboratoires
- Les remises à disposition 

## Améliorations possibles
- Modèle de prévision des tensions (Avec la loi poisson)
- Croisement avec données avec d'autres bases comme la FDA
- Classification par classe thérapeutique

## Conclusion générale

Cette étude met en évidence une lecture fine et structurée de la disponibilité des médicaments en France sur la période 2013 - début 2026, en dépassant une approche strictement événementielle pour intégrer également l’analyse des situations de normalité, c’est-à-dire l’absence d’événement.

L’analyse des événements déclarés montre une dégradation nette et récente de la situation, principalement à partir de 2021, avec un point culminant en 2024–2025. Les tensions d’approvisionnement et les ruptures de stock se concentrent sur un nombre limité de laboratoires, majoritairement des génériqueurs, traduisant une fragilité structurelle des chaînes d’approvisionnement, fortement exposées aux aléas industriels, logistiques et géopolitiques.

En parallèle, l’étude des non-événements apporte un éclairage complémentaire essentiel. Près de 15 000 spécialités, réparties entre 529 laboratoires, n’ont connu aucun événement sur la période étudiée. Cette stabilité concerne principalement des AMM actives, indiquant qu’il ne s’agit pas d’une absence artificielle d’événements liée à une inactivité réglementaire, mais bien d’une performance réelle en conditions de marché. Les grands génériqueurs concentrent une part importante de ces spécialités stables, suggérant une maîtrise industrielle et logistique et une capacité à absorber la demande sans générer de rupture.

L’analyse par statut d’AMM confirme des différences structurelles marquées :

les AMM actives concentrent à la fois la majorité des événements et la majorité des situations de stabilité, car elles sont pleinement exposées au marché ;

les AMM archivées, abrogées, retirées ou suspendues jouent un rôle marginal dans la disponibilité actuelle et présentent une faible valeur prédictive, justifiant leur exclusion ou leur pondération dans les modèles prospectifs.

Les analyses croisées par laboratoire et par spécialité montrent que la taille du portefeuille ne suffit pas à expliquer le risque. Le ratio événement par spécialité apparaît comme un indicateur plus pertinent que le volume brut d’événements, mettant en évidence des situations de vulnérabilité élevée chez certains acteurs à faible portefeuille, mais aussi des stratégies d’absorption efficaces chez les grands titulaires.

Enfin, les résultats obtenus justifient pleinement le recours à une approche prédictive, notamment via des modèles adaptés aux événements rares tels que la loi de Poisson. Une telle modélisation permettrait d’estimer la probabilité d’occurrence future des événements, d’identifier les DCI ou laboratoires à risque élevé et d’anticiper les tensions à court et moyen terme.

Dans son ensemble, cette étude propose une vision robuste, cohérente et exploitable de la disponibilité des médicaments, en articulant données historiques, analyse de la stabilité et perspectives prédictives. Elle constitue une base solide pour éclairer les décisions en matière de gestion des risques, de politique du médicament et de continuité des soins.

## Auteur
Georgy Djounda – Data Analyst / Pharmacien
