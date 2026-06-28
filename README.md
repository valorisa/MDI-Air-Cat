# L'Autonomie du MDI CAT — Moteur à air comprimé (2003)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/valorisa/mdi-air-cat/blob/main/notebook/mdi_air_cat_analysis.ipynb)

**Une analyse pédagogique du rapport de l'École des Mines de Paris (octobre 2003).**

---

## Le pitch

En 2003, la société MDI promettait un véhicule "zéro émission" fonctionnant à l'air comprimé. Ce projet reproduit les calculs du rapport original, les confronte à la physique moderne, et révèle pourquoi on ne croise pas de voitures à air comprimé dans nos rues.

## Ce que vous trouverez ici

- 🔬 **Modèle thermodynamique simple** (gaz parfait) vs **modèle réel** (gaz supercritique avec CoolProp)
- 🚗 **Comparaison des autonomies** à vitesse constante et en cycle urbain
- 🔥 **Le twist** : pourquoi MDI a dû ajouter un brûleur diesel
- 📊 **Simulation dynamique** pas-à-pas du cycle urbain CEE (195 secondes)
- 📉 **Benchmark 2026** : air comprimé vs batteries LFP vs hydrogène vs diesel
- 🏛️ **Autopsie historique** : que sont devenus MDI et Tata Motors ?

## Pour exécuter le notebook

Cliquez sur le badge Colab ci-dessus. Aucune installation locale requise.

## Résultats clés

| Scénario | Autonomie |
|----------|-----------|
| Gaz parfait (20 km/h) | 73,8 km |
| Gaz réel (20 km/h) | 105,3 km |
| Cycle urbain (sans accessoires) | 47 km |
| Cycle urbain (avec accessoires 300W) | 40 km |
| Cycle urbain + brûleur diesel (100°C) | 53 km |

## Licence

- **Code** : MIT
- **Texte et analyse** : CC BY-NC 4.0

---

*"La physique est impitoyable. L'air comprimé n'est pas un carburant, c'est un accumulateur très faible."*
