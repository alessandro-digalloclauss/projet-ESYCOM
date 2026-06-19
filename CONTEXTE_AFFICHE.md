# Contexte projet — Affiche "AUTOPSIE CLR" (Bilan carbone ESYCOM 2024)

> Fichier de passation destiné à une autre IA (ou un autre contributeur).
> But : permettre d'apporter des améliorations à **l'affiche du projet étudiant** sans repartir de zéro.
> Dernière mise à jour : 2026-06-19.

---

## 1. Le projet en bref

- **Type** : projet étudiant (Le Jour des Projets), promo E3S, ESIEE Paris.
- **Sujet** : "AUTOPSIE CLR — Autopsie climat du laboratoire de recherche ESYCOM".
  Analyse de l'empreinte carbone **2024** du laboratoire ESYCOM (CNRS) et modélisation
  des leviers d'action pour atteindre la trajectoire de réduction **CNRS 2030 (−50 %)**.
- **Auteurs** : LAMARQUE Amélie, DAUTHIEU Laure, DI GALLO CLAUSS Alessandro, CARCANADE Rosa, LOCCISANO Constance.
- **Tuteur** : HERVÉ Armande.
- **Sources des données** : GES-1point5 / Labos 1point5, ADEME Base Carbone.

## 2. Les deux livrables (NE PAS CONFONDRE)

1. **L'affiche** = le poster A0/A1 à présenter (fait sur un outil de design type Canva/PowerPoint).
   👉 **C'est ici que les améliorations sont attendues.** Ce n'est PAS un fichier de ce repo,
   c'est un visuel image. Les corrections doivent être reportées à la main dans l'outil de design.
2. **`bilan_carbone_esycom2024_multilabos_v4.html`** = une page web interactive séparée
   (simulateur, graphiques Chart.js). **C'est le modèle de calcul qui fait FOI.**
   Les chiffres de l'affiche doivent toujours être alignés sur ce fichier.

## 3. Données de référence (source de vérité = le HTML)

### Total et intensité
- **Total GES 2024 = 385,5 tCO₂eq** (et non 385,6 — vérifier l'affiche).
- **Intensité = 7,49 tCO₂eq / ETP** (ETP = Équivalent Temps Plein ; labo = **51,5 ETP**).
  ⚠️ Écrire **"/ETP"** et non "/pers" (terme officiel Labos 1point5).
- Équivalences : ≈ **214 allers-retours Paris–New York en avion** (385,5 ÷ ~1,8 t/AR). ✓ vérifié.

### Répartition par poste 2024 (le camembert — VÉRIFIÉ COHÉRENT)
| Poste | tCO₂e | % |
|---|---|---|
| Achats & consommables | 235,0 | 61,0 % |
| Missions professionnelles | 85,2 | 22,1 % |
| Énergie (élec + chauffage) | 26,0 | 6,7 % |
| Construction & infrastructure | 20,5 | 5,3 % |
| Domicile-travail | 12,8 | 3,3 % |
| Numérique & IT | 6,0 | 1,6 % |
| **TOTAL** | **385,5** | 100 % |

### Évolution pluriannuelle
- 2022 : 285 t (4,38 t/ETP, 65 ETP) — 2023 : 414 t (7,02 t/ETP, 59 ETP) — 2024 : 385,5 t (7,49 t/ETP, 51,5 ETP).
- Objectif CNRS 2030 (−50 %) → cible ≈ **143 tCO₂e**.

### Benchmark / personne (graphe horizontal du HTML)
Objectif Paris 2030 : 0,8 — Moy. nationale (~200 labos) : 2,1 — LRP 2023 : 4,61 —
Pprime 2024 : 4,85 — LAAS 2023 : 7,0 — **ESYCOM 2024 : 7,49**.
→ Message fort : ESYCOM est ~3,5× la moyenne nationale (à savoir expliquer = labo "achats lourds").

### Plan d'action (chiffres de l'affiche)
- **Achats (235 t = 61 %)** : mutualiser commandes, reconditionné, regrouper livraisons,
  codification NACRES. Potentiel **−60 à −100 tCO₂e/an**.
- **Missions (85 t = 22 %)** : train obligatoire <6h, visioconférence, quota carbone
  (plafond strict ≈ 2 tCO₂e/an/ETP). Potentiel **−30 à −50 tCO₂e/an**.
- **Énergie (26 t)** : capteurs de présence + LED, thermostat 19 °C, électricité verte.
- **Mobilités / domicile (12,8 t)** : remboursement Navigo, forfait mobilités durables, télétravail 2 j/sem.

## 4. État de la relecture (déjà fait)

- ✅ Camembert : valeurs et % **vérifiés cohérents** avec le HTML.
- ✅ Équivalence "214 A/R Paris–New York" : **plausible**.
- ⚠️ **À vérifier sur l'affiche** : le grand chiffre total affiche-t-il **385,5** ou **385,6** ?
  (la somme exacte = 385,5).
- ⚠️ **"7.49 TCO₂EQ/PERS"** → remplacer par **"/ETP"**.
- ⚠️ **"ET UNE SURFACE DE ___ M²"** → champ de surface vide à compléter (ou retirer).

## 5. Pistes d'amélioration suggérées (pour la prochaine IA)

### Cohérence / rigueur
1. Harmoniser le total (385,5) et l'unité d'intensité (/ETP) partout.
2. Compléter ou supprimer la mention "surface en m²".
3. Ajouter une **mention de la méthode** (incertitude des facteurs d'émission, périmètre scopes 1/2/3)
   — un correcteur appréciera.

### Lisibilité / design
4. Hiérarchie visuelle : le message clé ("61 % = achats, pas l'énergie") devrait être le plus visible.
5. Vérifier le contraste des libellés clairs sur fond foncé (accessibilité).
6. Uniformiser la typo des nombres (virgule décimale FR partout : 385,5 / 7,49).

### Storytelling
7. Angle recommandé pour l'oral : *"On croit qu'un labo se décarbone en éteignant les lumières,
   mais 61 % vient des achats."* → relie directement bilan ↔ plan d'action.
8. Rendre explicite le lien trajectoire actuelle (385 t) → cible 2030 (143 t) et le "gap" à combler.

## 6. Garde-fous pour toute modification

- **Toujours** revérifier qu'une nouvelle valeur sur l'affiche existe dans
  `bilan_carbone_esycom2024_multilabos_v4.html` (objets `P_DATA` ~ligne 1858, et le doughnut ~ligne 1284).
- Ne jamais "inventer" un chiffre : si une donnée manque (ex : surface m²), la demander, pas l'estimer.
- Les % du camembert sont calculés sur **385,5** (cf. `c.raw/385.5*100` dans le HTML).
