# 🦠 Simulation Propagation Épidémique Madagascar - Guide Rapide

## DÉMARRAGE EN 3 ÉTAPES

### 1️⃣ Prérequis
- Télécharger **NetLogo 7.0.4** : https://ccl.northwestern.edu/netlogo/

### 2️⃣ Lancer la simulation
1. Ouvrir `model.nlogo` dans NetLogo 7.0.4
2. Cliquer sur **SETUP**
3. Cliquer sur **GO**

### 3️⃣ Explorer
- Modifier les sliders (taux de transmission, mobilité, mortalité)
- Observer les graphiques SIR en temps réel
- Analyser l'impact des corridors de mobilité entre villages

---

## 📦 CONTENU DU PROJET

| Fichier | Description |
|---------|-------------|
| `simulation_epidemiologie.nlogox` | **Simulation complète NetLogo 7** (code + interface) |
| `DOCUMENTATION.md` | Documentation technique détaillée (architecture, algorithmes) |
| `PROTOCOLE_EXPERIMENTAL.md` | Protocole scientifique d'étude épidémiologique |
| `README.md` | Ce fichier (démarrage rapide) |

---

## 🎯 FONCTIONNALITÉS CLÉS

✅ **3 types d'agents** : Humains, Vecteurs (moustiques), Villages  
✅ **Modèle SIR** : Susceptible, Infecté, Rétabli/Mort  
✅ **Corridors de mobilité** : Déplacement réaliste entre hubs de population  
✅ **Transmission vectorielle** : Moustique -> Humain et Humain -> Moustique  
✅ **Monitors** : Suivi précis de la morbidité et mortalité  
✅ **Plots** : Courbes épidémiques dynamiques  

---

## 🎨 CODE COULEUR VISUEL

- 🔵 **Humain bleu** : Sain (Susceptible)
- 🔴 **Humain rouge** : Infecté (Infectious)
- 🟢 **Humain vert** : Guéri (Recovered)
- ⚪ **Humain gris** : Décédé (Dead)
- 🟡 **Moustique jaune** : Sain
- 🟠 **Moustique orange** : Porteur (Infecté)
- 🏠 **Maison blanche** : Village (Hub)
- 🛣️ **Patch gris** : Corridor de mobilité (Route)

---

## 🎓 USAGE ACADÉMIQUE

Ce projet est conçu pour :
- Étude des dynamiques de diffusion épidémique
- Analyse de l'impact de la mobilité géographique
- Modélisation des endémies à Madagascar (Peste, Paludisme)

**Bonne simulation ! 🦠🇲🇬**
