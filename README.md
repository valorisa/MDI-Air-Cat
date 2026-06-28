# L'Autonomie du MDI CAT — Moteur à air comprimé (2003)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/VOTRE_USERNAME/mdi-air-cat/blob/main/notebook/mdi_air_cat_analysis.ipynb)
[![License: MIT](https://img.shields.io/badge/Code-MIT-blue.svg)](LICENSE)
[![License: CC BY-NC 4.0](https://img.shields.io/badge/Texte-CC%20BY--NC%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc/4.0/)

**Une analyse pédagogique du rapport de l'École des Mines de Paris (octobre 2003).**

---

## Le pitch

En 2003, la société MDI (Motor Development International) promettait un véhicule
"zéro émission" fonctionnant à l'air comprimé. Ce projet reproduit les calculs du
rapport original d'Adeline Fabre et Jacky Mochel, les confronte à la physique
moderne, et révèle pourquoi on ne croise pas de voitures à air comprimé dans nos rues.

## Ce que vous trouverez ici

- 🔬 **Modèle thermodynamique simple** (gaz parfait) vs **modèle réel** (fluide
  supercritique avec CoolProp).
- 🚗 **Comparaison des autonomies** à vitesse constante et en cycle urbain CEE.
- 🔥 **Le twist** : pourquoi MDI a dû ajouter un brûleur diesel.
- 📊 **Simulation dynamique** pas-à-pas du cycle urbain (195 secondes, machine
  à états pour les 3 étages de détente).
- 📉 **Benchmark 2026** : air comprimé vs batteries LFP vs hydrogène vs diesel.
- 🏛️ **Autopsie historique** : le rachat par Tata Motors (2007) et l'abandon du projet.

## Résultats clés

| Scénario | Autonomie |
|----------|-----------|
| Gaz parfait, 20 km/h (vitesse constante) | 73,8 km |
| Gaz réel, 20 km/h (vitesse constante) | 105,3 km |
| Cycle urbain CEE (sans accessoires) | 47,3 km |
| Cycle urbain CEE (avec accessoires 300 W) | 40,3 km |
| Cycle urbain CEE + récupération 13 % | 42,2 km |
| Cycle urbain + brûleur diesel à 80 °C | 56 km |

*Source : Tableau 6 et Tableau 10 du rapport original (Fabre & Mochel, 2003).*

## Pour exécuter le notebook

Cliquez sur le badge **Open In Colab** ci-dessus. Aucune installation locale
requise — les dépendances s'installent automatiquement en première cellule.

**Vous n'avez jamais codé ?** Dans Colab : *Exécution → Exécuter toutes les
cellules*. Lisez les commentaires Markdown entre les cellules de code.

### En local

```bash
git clone https://github.com/VOTRE_USERNAME/mdi-air-cat.git
cd mdi-air-cat
pip install -r requirements.txt
jupyter notebook notebook/mdi_air_cat_analysis.ipynb
```

## Structure du dépôt

```
mdi-air-cat/
├── README.md           — ce fichier
├── CONTRIBUTING.md     — règles de contribution
├── LICENSE             — MIT (code) / CC BY-NC 4.0 (texte)
├── requirements.txt    — dépendances Python
├── .gitignore
└── notebook/
    └── mdi_air_cat_analysis.ipynb
```

## Conclusions clés

1. **L'air comprimé n'est pas un carburant** — c'est un accumulateur à très
   faible densité énergétique : 0,1 MJ/L contre 0,9 MJ/L pour une batterie LFP
   et 35 MJ/L pour le diesel.
2. **La physique est impitoyable** : en hiver, de nuit, sous la pluie,
   l'autonomie descend sous 30 km.
3. **Le "zéro émission" était un mythe** : pour atteindre des autonomies
   acceptables, MDI a dû ajouter un brûleur diesel — transformant le véhicule en
   hybride pneumatique-diesel.

## Autopsie historique

MDI a signé un accord de licence avec Tata Motors en 2007 pour produire le
véhicule en Inde. Après plusieurs reports successifs et l'absence de produit
commercialisable, Tata a abandonné le partenariat. MDI continue d'exister mais
n'a jamais livré un seul véhicule à air comprimé à un client final.

## Références

- Fabre A., Mochel J. (2003). *Évaluation de l'autonomie d'un véhicule CAT
  utilisant la technologie MDI*. École des Mines de Paris, Centre Énergétique,
  Armines. Encadré par J. Benouali et R. El Chammas.
- Benouali J., Clodic D. (2003). *Étude préalable du moteur 34p01-4*, Centre
  d'Énergétique, École des Mines de Paris.

## Licence

- **Code** : MIT — réutilisation libre, attribution appréciée.
- **Texte et analyse** : CC BY-NC 4.0 — citation obligatoire, usage commercial
  interdit sans accord.

---

*"La physique est impitoyable. L'air comprimé n'est pas un carburant,
c'est un accumulateur très faible."*
