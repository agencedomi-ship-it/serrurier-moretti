# Site Moretti Serrurier

Site statique : LP principale + 7 LPs zone + 190 pages ville/arrondissement.

## Structure

```
/                              # LP generale (Moretti)
/paris                         # LP Paris (75)
/idf-petite-couronne           # LP IDF Petite Couronne (92/93/94)
/idf-grande-couronne           # LP IDF Grande Couronne (77/78/91/95)
/sud-est                       # LP Sud-Est (83/06)
/sud-ouest                     # LP Sud-Ouest (30/34)
/ouest                         # LP Ouest (44/56/85/35)
/bas-rhin                      # LP Bas-Rhin (67)
/serrurier-<ville>             # 190 pages dediees ville/arrondissement
```

## Publication GitHub Pages

1. Push ce dossier dans un repo GitHub
2. Settings > Pages > Source = main branch / root
3. Domaine custom : ajouter le fichier `CNAME` avec `www.serrurier-moretti.fr`
4. Configurer le DNS chez le registrar : CNAME `www` -> `<user>.github.io`

## Inventaire URLs

L'inventaire complet des 197 URLs est dans `Moretti.xlsx` feuille "Inventaire LPs".

## Assets

- `/photos/` : photos hero, equipe, vehicules, avatars
- `/logos/` : logos marques, assurances, plateformes

## Genere automatiquement

Ne pas editer manuellement les pages ville (`serrurier-*/index.html`) :
elles sont generees depuis le template via `outputs/generate_all.py`.
