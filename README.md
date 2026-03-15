# Tutoriels d’analyse de graphes et réseaux probabilistes

Ce dépôt regroupe une série de notebooks pédagogiques consacrés à la **reconstruction**, l’**analyse** et la **visualisation** de réseaux probabilistes (Bayesian Networks) à partir de données réelles. Ces travaux ont été réalisés en collaboration avec **Serigne Bassirou Ndiaye**.

L’objectif est d’explorer plusieurs approches classiques de l’inférence de graphes, d’en comparer les performances et d’illustrer leurs applications sur des jeux de données variés (assurance, données génomiques COSMIC).


## 🎯 Objectifs du projet

- Comprendre les principes des réseaux bayésiens.  
- Appliquer différentes méthodes de reconstruction :  
  - **Hill-Climbing** (score-based)  
  - **PC Algorithm** (constraint-based)  
  - **ARACNE** (information mutuelle)  
  - **MIIC** (méthode informationnelle robuste)  
- Comparer les performances via TP / FP / FN, précision, rappel, F-score.  
- Visualiser les graphes avec **igraph** et **qgraph**.  
- Interpréter les structures obtenues (clusters, hubs, dépendances causales).  


## 📁 Contenu du dépôt

```
graph-analysis-tutorials/
├── README.md
├── notebooks/
│   ├── graph_reconstruction.ipynb (reconstruction du réseau “insurance” avec Hill-Climbing, PC et ARACNE)
│   ├── hill_climbing.ipynb (reconstruction du réseau COSMIC avec Hill-Climbing)
    └── PC_MIIC.ipynb (reconstruction du réseau COSMIC avec PC et MIIC)
```


## 🧠 Méthodes étudiées

### **Hill-Climbing (score-based)**
- Optimisation du score BIC.  
- Reconstruction dirigée.  
- Analyse des erreurs (TP, FP, FN).  

### **PC Algorithm (constraint-based)**
- Tests d’indépendance conditionnelle.  
- Squelettes non orientés puis orientation partielle.  
- Sensibilité au seuil α.  

### **ARACNE**
- Basé sur l’information mutuelle.  
- Graphe non orienté, parcimonieux.  

### **MIIC**
- Méthode robuste basée sur l’information mutuelle conditionnelle.  
- Détection de dépendances complexes.  
- Analyse stricte vs standard.  


## 📈 Visualisation et analyse

Les notebooks incluent :

- Graphes orientés et non orientés  
- Mise en évidence des faux positifs / faux négatifs  
- Identification des hubs (degree, betweenness)  
- Analyse mutation ↔ expression (COSMIC)  
- Rôle de la ploïdie dans les réseaux biologiques  


## 🛠️ Technologies utilisées

- **R**  
- bnlearn  
- pcalg  
- miic  
- igraph  
- qgraph  


## 👥 Collaboration

Projet réalisé en binôme :  
- **Lyse NDIFO**  
- **Serigne Bassirou Ndiaye**


## 📚 Références

- Documentation *bnlearn*  
- Documentation *pcalg*  
- Documentation *miic*  
- Dataset COSMIC (mutation, expression, ploïdie)  


