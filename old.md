# Anticiper la production d'énergies renouvelables et améliorer l'optimisation du mix énergétique.

## Table des Matières
- [Introduction](#introduction)
- [Sujet choisit](#sujet-choisit)
- [Membres de l'équipe et leurs compétences](#membres-de-léquipe-et-leurs-compétences)
- [Problématique](#problématique)
- [Approche et méthodologie](#approche-et-méthodologie)
  - [Analyse des données météorologiques](#analyse-des-données-météorologiques)
  - [Analyse des données de consommation et production Eco2mix et des jours TEMPO](#analyse-des-données-de-consommation-et-production-eco2mix-et-des-jours-tempo)
  - [Préparation des données pour la modélisation](#préparation-des-données-pour-la-modélisation)
  - [Développement d'un modèle prédictif](#développement-dun-modèle-prédictif)
- [Usagers pressentis et bénéfices](#usagers-pressentis-et-bénéfices)
- [Architecture technique](#architecture-technique)
- [Résultats et analyses](#résultats-et-analyses)
- [Conclusion et perspectives futures](#conclusion-et-perspectives-futures)
- [Annexes](#annexes)


## Introduction
### Hackathon data.gouv.fr - météo france
Le Hackathon Météo est un événement de deux jours complets (8 et 9 avril 2024) consacré à la valorisation des données publiques météorologiques. Il réunira tous types de profils pour répondre à des défis liés à la thématique météorologique.

Il est organisé par la Direction interministérielle du numérique et Météo-France.

L'objectif du hackathon sera de faciliter l'accès et la réutilisation des données publiques météorologiques.

### Sujet choisit
**Anticiper la production d'énergies renouvelables et améliorer l'optimisation du mix énergétique.**

### Membres de l'équipe et leurs compétences
- **Mathieu NICOLLE (@mnicolle)** : Expert en Python, compétences en Data Engineering.
- **Antoine T (@Antoine T)** : Data Scientist, spécialisé en Python.
- **Frederic LAGNIEZ (@Frederic_LAGNIEZ)** : Data Scientist, maîtrise Python.
- **Samuel LITZLER (@Samuel Litzler)** : Développeur fullstack web et géomaticien.
- **Thibaut CASSARD (@ThibautC)** : Data Scientist, spécialisé en analyse numérique et Python.
- **Matthieu Colin (@Matthieu Colin)** : Data Scientist, compétences en Python, cloud et data sciences.
- **Robin Locatelli (@Robin)** : Inscrit dans l’équipe mais non présent - compétences non spécifiées.

## Problématique
- [ ] A détailler

Notre équipe se concentre sur des solutions spécifiques pour anticiper les variations de la capacité de production d'énergies renouvelables en utilisant les données météorologiques.
## Approche et méthodologie
Notre équipe se focalise sur l'élaboration de stratégies pour anticiper les variations de la capacité de production d'énergies renouvelables en se basant sur les données météorologiques et la consommation énergétique historique.

### **Étapes Clés :**

#### **Analyse des données météorologiques**
Utilisation des prévisions météo du modèle ARPEGE, avec une attention particulière sur les prévisions du flux solaire moyen, de la vitesse du vent moyen et des températures moyennes annuelles en France.

Le but étant d’avoir des indicateurs de ces prévisions par jour.

#### **Analyse des données de consommation et production Eco2mix et des jours TEMPO**
Formatage des données de consommation et production énergétique fournies par RTE, incluant les consommations réelles et les prévisions.

- [ ] détail des indicateurs
- [ ] détail du calcul de l'analyse + ressource

Le tableau final pour chaque jour inclut les indicateurs suivants :
- Nature
- Date
- Heures
- Consommation
- Prévision J-1
- Prévision J
- Fioul
- Charbon
- Gaz
- Nucléaire
- Éolien
- Solaire
- Hydraulique
- Pompage
- Bioénergies
- Échanges physiques
- Taux de CO2
- Échanges commerciaux
- Stockage batterie
- Déstockage batterie
- Type de jour TEMPO


#### **Préparation des données pour la modélisation**
Concaténation des données météorologiques et de consommation énergétique pour créer un ensemble unifié utilisé pour le développement d'un modèle prédictif.
Cette étape vise également à analyser les caractéristiques des jours TEMPO, particulièrement les jours TEMPO rouge, qui surviennent principalement en hiver (de septembre à mars). La compréhension de ces jours permettra de prédire leur occurrence.

Les données agrégées pour la période “été” pourront servir à d'autres analyses.

#### **Développement d'un modèle prédictif**
Mise en place d'un modèle exploitant l'ensemble de données consolidé pour anticiper les situations de stress énergétique, y compris la prédiction des jours TEMPO rouge, tout en tenant compte des divers facteurs influençant la consommation et la production énergétique (achat d’électricité, plus de production carbonée car déficit possible …)

## Usagers pressentis et bénéfices
- [ ] détailler plus les usagers cible + essayer d'avoir cas concret ?
- [ ] Mettre cette partie avant la partie approche et méthodologie

- Usagers : Utilisateurs de contrats TEMPO et particuliers équipés en installations électriques.
- Horizon 2050 : Contribuer à la restructuration du réseau énergétique pour améliorer sa résilience et son efficacité -> on a eu une réflexion sur les contrats TEMPO qui ne sont adaptés qu’aux jours froids sauf qu’avec le changement climatique et l’achat massif de climatisation, il est possible que la tendance évolue vers les jours de forte chaleur.
- Éducation et sensibilisation : Les données et les prédictions générées pourraient servir à des campagnes d'éducation du public sur l'utilisation de l'énergie et l'importance de la transition énergétique.
- Autres ? On aura un historique annuel par jour pour entraîner des possibles modèles de prédictions ?

## Architecture technique
- Description de l'architecture technique du projet, incluant les outils, les technologies utilisées, et la structure des données.

## Résultats et analyses

- [ ] Présentation des résultats obtenus.
- [ ] Analyses des performances du modèle et interprétation des données.

## Conclusion et perspectives futures
- [ ] Synthèse des accomplissements et réflexion sur les objectifs atteints.
- [ ] Discussion sur les perspectives futures et les améliorations potentielles.

## Annexes
- [ ] Documents supplémentaires, codes sources, références, ou tout autre matériel d'appui.
