# Gabarit UdeM (science politique)

Ce répertoire fournit un gabarit Quarto pour les travaux et dissertations du departement de science politique de l'Université de Montreal. Il applique les exigences materielles (marges, interligne, police, pagination, titres, bibliographie).

## Prerequis

- Quarto installé: https://quarto.org/docs/get-started/
- Un moteur LaTeX 

## Utilisation rapide (via GitHub)

1. Ouvrez ce depot dans GitHub et cliquez sur **Fork**.
2. Dans votre fork, ouvrez `projet.qmd` et modifiez les variables LaTeX en haut du fichier:
   - `\titretravail`, `\auteur`, `\auteurid`, `\cours`, `\coursnumero`, `\professeur`, `\departement`, `\faculte`, `\lieu`
3. Remplacez le contenu du document par votre texte.
4. Generez le PDF:
   ```bash
   quarto render projet.qmd
   ```

## Utiliser le gabarit directement

Vous pouvez cloner le gabarit dans un nouveau dossier avec Quarto:

```bash
quarto use template githubusername/gabarit_udem
```

Puis editez `projet.qmd` et compilez:

```bash
quarto render projet.qmd
```

## Structure du depot

- `projet.qmd`: gabarit principal
- `references.bib`: bibliographie (à adapter)
- `img/UdeM_CoA.png`: logo (si requis par votre professeur)

## Remarques importantes

- Le gabarit est en `pdflatex` avec une police Times open source (newtx). C'est robuste pour la plupart des installations.
- La page de titre n'est pas numerotee; la premiere page de texte commence a 1 (non affichee), puis la numerotation apparait en haut a droite.
- L'introduction ne doit pas avoir de titre; commencez le texte directement avant le premier titre de section.

Bon travail.
