# R111

## Bonnes pratiques CSS globales

### Points généraux

- Opter pour des tailles de polices fluides (de préférence en rem), éviter les tailles de police de taille fixe (px ou pt) car inaccessible aux personnes nécessitant d’agrandir les contenus textuels.
- Éviter d’écraser une règle par une autre.
- La règle `!important` doit être éradiquée si possible du fait de son poids extrêmement important (certaines parties des styles peuvent toutefois exceptionnellement employer à juste titre `!important`).
- Durant la phase de développement l'intégration se fait sur plusieurs fichiers CSS (composants, layout, etc.) que l'on rassemble (@import) dans un fichier unique.
- Les fichiers CSS doivent être minifiés pour économiser du poids de chargement.
- Toujours préciser quelle(s) propriété(s) doit être animée dans une transition ou animation.
- Éviter d’animer des propriétés autres que transform ou opacity ou filter (ou alors ajouter la propriété will-change au cas par cas).

**Remarque sur l'ordre des déclarations**
Les déclarations au sein d'une règle CSS sont ordonnées de façon à faire apparaître les propriétés importantes en tête de liste.

Voici l'ordre dans lequel nous déclarons nos propriétés :

- **Propriété display** : tout ce qui affecte le rendu par défaut de l’élément
- **Positionnement** : tout ce qui détermine la position de l’élément
- **Modèle de boîte** : tout ce qui influe sur les dimensions de l’élément
- **Typographie** : tout ce qui détermine les caractéristiques de la police de caractères
- **Effets Viusels & Graphiques**
- **Transformations et transitions**

La démarche de réordonnement est manuelle, en se servant de cette liste comme référence.

Ref
[Alsacreation](https://github.com/alsacreations/guidelines/blob/master/Guidelines-CSS.md)

https://www.alsacreations.com/outils/guidelines/Guidelines-CSS.md
[CUBE]()

## Outils

### Place Holder

- http://picsum.photos
- https://www.pexels.com
- https://i.pravatar.cc/{size}
- http://lorempixel.com/400/200
- https://doodleipsum.com/
- https://logoipsum.com/

Exemple d'utilisation

```html
https://picsum.photos/480/320/?random
```
