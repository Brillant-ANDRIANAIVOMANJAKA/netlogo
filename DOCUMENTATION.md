# 📝 Documentation Technique : Simulation Épidémiologique Madagascar

## 1. ARCHITECTURE DU MODÈLE

Le modèle repose sur une approche **Système Multi-Agents (SMA)** couplée à un modèle compartimental **SIR** (Susceptible-Infectious-Recovered).

### 1.1 Types d'Agents (Breeds)
- **Humains (`humans`)** : Population cible de l'épidémie. Ils se déplacent entre les villages.
- **Vecteurs (`vectors`)** : Moustiques (Paludisme) ou Puces (Peste). Ils transmettent l'agent pathogène.
- **Villages (`villages`)** : Hubs de population servant de centres d'activité et de points d'origine/destination.

### 1.2 Environnement
- **Corridors de mobilité** : Réseau de routes (patches gris) reliant les villages. Les humains suivent préférentiellement ces chemins pour se déplacer, simulant ainsi les flux migratoires réels à Madagascar.

---

## 2. DYNAMIQUES COMPORTEMENTALES

### 2.1 Modèle de Mobilité Inter-Villages
Les humains utilisent une logique de destination :
1. Sélection d'un village cible aléatoire selon la `frequency-mobility`.
2. Navigation le long des corridors (recherche de patches de couleur grise).
3. Retour au comportement local une fois arrivé.

### 2.2 Cycle de Transmission SIR
- **Infection** : Un humain sain devient infecté s'il se trouve sur le même patch qu'un vecteur infecté (probabilité basée sur `transmission-rate`).
- **Infection des vecteurs** : Un vecteur sain devient porteur s'il pique un humain déjà infecté.
- **Évolution** : Après une période d'incubation, l'humain a une probabilité quotidienne de :
    - Mourir (`mortality-rate`).
    - Guérir et devenir immunisé (`recovery-chance`).

---

## 3. PARAMÈTRES ET VARIABLES

### 3.1 Sliders de l'Interface
| Paramètre | Description |
|-----------|-------------|
| `initial-human-pop` | Nombre d'individus au début de la simulation |
| `transmission-rate` | Probabilité de passage du pathogène lors d'un contact |
| `mortality-rate` | Risque de décès pour un individu infecté |
| `mobility-frequency` | Intensité des déplacements inter-villages |

---

## 4. ANALYSE ET STATISTIQUES

La simulation suit en temps réel :
- **Taux de prévalence** : Pourcentage de la population infectée.
- **Taux de létalité** : Nombre de décès total.
- **Courbe épidémique** : Visualisation de la progression temporelle (Plot SIR).

---

## 5. CONTEXTE HISTORIQUE
Inspiré par :
- **Épidémie de Peste 2017** : Propagation rapide via les axes de transport routier.
- **Paludisme Endémique** : Transmission saisonnière par vecteurs anophèles.

**Note** : Ce modèle est une simplification à visée pédagogique et de recherche conceptuelle.
