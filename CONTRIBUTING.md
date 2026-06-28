# Contribuer au projet MDI CAT

Merci de t'intéresser à ce projet pédagogique. Voici les règles pour contribuer.

## Ce qui est bienvenu

- 🐛 **Corrections de bugs** : si un calcul ne correspond pas au PDF ou si une
  équation est mal transcrite, ouvre une issue avec la page et le tableau de
  référence.
- 📚 **Améliorations pédagogiques** : reformulation d'un passage, ajout d'une
  analogie, correction d'une faute de frappe.
- 🔬 **Extensions** : simulation avec récupération d'énergie au freinage (>13 %),
  modèle de température ambiante variable, benchmark mis à jour. Une branche
  `feature/extensions` est ouverte pour ces contributions.

## Ce qui n'est PAS bienvenu

- ❌ **Curve fitting** : toute PR qui modifie les constantes du PDF (rendement
  isentropique 85 %, pertes d'air 2 %, efficacité échangeurs 50 %) dans le seul
  but de "faire coller" les chiffres sera rejetée sans discussion.
- ❌ **Suppression des avertissements** : les notes sur les limites du modèle
  (gaz parfait, fallback CoolProp/NIST, valeurs interpolées) sont essentielles
  à l'honnêteté pédagogique du projet.
- ❌ **Réécriture de l'histoire** : l'autopsie de MDI et Tata Motors doit rester
  factuelle et documentée. Toute affirmation non sourcée sera retirée.

## Règle d'or

> **Les constantes du PDF sont figées. Les écarts entre notre modèle et le PDF
> sont documentés, pas masqués.**

## Comment contribuer

1. Fork le dépôt.
2. Crée une branche explicite :
   ```bash
   git checkout -b fix/calcul-puissance-acceleration
   # ou
   git checkout -b feature/recuperation-freinage
   ```
3. Teste ton notebook en local ou sur Colab de bout en bout
   (*Exécution → Exécuter toutes les cellules*).
4. Ouvre une Pull Request avec :
   - ce que tu as changé et pourquoi ;
   - la référence au tableau ou à la figure du PDF si applicable ;
   - une capture d'écran ou un extrait de sortie si tu modifies un calcul.

## Environnement de développement

```bash
git clone https://github.com/VOTRE_USERNAME/mdi-air-cat.git
cd mdi-air-cat
pip install -r requirements.txt
jupyter notebook notebook/mdi_air_cat_analysis.ipynb
```

## Licence

- Code : MIT.
- Texte et analyse : CC BY-NC 4.0 (citation obligatoire, usage commercial
  interdit sans accord).2. Crée une branche : `git checkout -b feature/ma-contribution`
3. Teste ton notebook en local ou sur Colab
4. Ouvre une Pull Request avec une description claire de ce que tu as changé et pourquoi

## Licence

- Code : MIT
- Texte/analyse : CC BY-NC 4.0 (citation obligatoire)
