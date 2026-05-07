# 🧪 Protocole Expérimental : Étude de la Propagation Épidémique

## 1. PROBLÉMATIQUE
Comment la structure des corridors de mobilité et la densité des vecteurs influencent-elles la vitesse de propagation et le bilan final d'une épidémie à Madagascar ?

---

## 2. HYPOTHÈSES SCIENTIFIQUES
- **H1** : Une augmentation de 20% de la mobilité inter-villages réduit le temps nécessaire pour atteindre le pic épidémique de 40%.
- **H2** : Les villages situés au croisement de plusieurs corridors (hubs) présentent un taux d'infection cumulé plus élevé que les villages isolés.
- **H3** : En l'absence de corridors, l'épidémie reste localisée et s'éteint spontanément (extinction stochastique).

---

## 3. VARIABLES DE L'EXPÉRIENCE

### 3.1 Variables Indépendantes (Facteurs)
- **Mobilité (`mobility-frequency`)** : [0, 5, 10, 20, 50]
- **Taux de transmission (`transmission-rate`)** : [5%, 15%, 30%]
- **Densité de vecteurs** : Ratio 1:2 et 1:5 par rapport aux humains.

### 3.2 Variables Dépendantes (Réponses)
- **Durée de l'épidémie** : Nombre de ticks jusqu'à 0 infectés.
- **Taux de mortalité final** : (Total morts / Population initiale) * 100.
- **Temps du Pic** : Tick où le nombre d'infectés est maximal.

---

## 4. PLAN D'EXPÉRIENCE (BEHAVIORSPACE)

### Expérience A : Impact de la Mobilité
- Fixer `transmission-rate` à 15%.
- Faire varier `mobility-frequency` de 0 à 100 par pas de 10.
- Répétitions : 30 simulations par palier pour assurer la validité statistique.

### Expérience B : Efficacité des Mesures de Confinement
- Comparer un scénario "Corridors ouverts" vs "Corridors bloqués" (simulation de quarantaine).

---

## 5. ANALYSE DES RÉSULTATS ATTENDUS
Les données extraites en CSV seront analysées pour identifier des corrélations non-linéaires entre la connectivité géographique et la résilience du système de santé local.

---

## 6. RÉFÉRENCES
- Modèle SIR (Kermack & McKendrick, 1927).
- Rapports OMS sur la Peste à Madagascar (2017).
