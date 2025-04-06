# Damier CSS - Projet de Grille 10x10

## Description
Ce projet est un exercice de création d'un damier en CSS avec une grille de 10x10 (100 divs au total). L'objectif est d'afficher un motif spécifique où certains cubes sont colorés en `rgba(0, 0, 0, 0.5)` (noir semi-transparent) et les autres sont transparents. Le damier est conçu pour être responsive et s'adapter à un écran de 1920x1080px, avec 50 cubes visibles (10 colonnes × 5 lignes) et les 50 autres coupés via `overflow: hidden`.

Les cubes colorés sont : 1, 3, 5, 7, 9, 12, 14, 16, 18, 20, 21, 23, 25, 27, 29, 32, 34, 36, 38, 40, 41, 43, 45, 47, 49.

## Aperçu
Voici un aperçu du damier pour les 5 premières lignes (50 cubes) :

| 1  | 2  | 3  | 4  | 5  | 6  | 7  | 8  | 9  | 10 |
|----|----|----|----|----|----|----|----|----|----|
| N  |    | N  |    | N  |    | N  |    | N  |    |
|    | N  |    | N  |    | N  |    | N  |    | N  |
| N  |    | N  |    | N  |    | N  |    | N  |    |
|    | N  |    | N  |    | N  |    | N  |    | N  |
| N  |    | N  |    | N  |    | N  |    | N  |    |

(N = Noir, vide = Transparent)

## Prérequis
- Un navigateur web moderne (Chrome, Firefox, Edge, etc.).
- Aucun framework ou dépendance externe n’est requis, juste du HTML et CSS.

## Installation
1. Clonez ou téléchargez ce dépôt.
2. Ouvrez le fichier `index.html` dans votre navigateur.

## Structure du Projet
- `index.html` : Contient la structure HTML avec 100 divs.
- `styles.css` : Contient les styles CSS pour la grille et le damier.

## Utilisation
- La grille est définie avec `display: grid` et `grid-template-columns: repeat(10, minmax(10vw, 1fr))`.
- Seuls les cubes spécifiés sont colorés en `rgba(0, 0, 0, 0.5)`, les autres sont transparents.
- Les 50 derniers divs (51-100) sont masqués avec `overflow: hidden` pour s’adapter à un écran 1920x1080px.

## Personnalisation
Pour continuer le motif jusqu’à 100 divs (10 lignes), il suffit d’ajuster `grid-template-rows` à `repeat(10, minmax(10vw, 1fr))` et de retirer `overflow: hidden`. Voici les cubes colorés pour les lignes 6 à 10 :

- **Row 6 (51-60)** : 51, 53, 55, 57, 59
- **Row 7 (61-70)** : 62, 64, 66, 68, 70
- **Row 8 (71-80)** : 71, 73, 75, 77, 79
- **Row 9 (81-90)** : 82, 84, 86, 88, 90
- **Row 10 (91-100)** : 91, 93, 95, 97, 99

Ajoutez ces classes dans le CSS comme suit :

```css
.item-51, .item-53, .item-55, .item-57, .item-59,
.item-62, .item-64, .item-66, .item-68, .item-70,
.item-71, .item-73, .item-75, .item-77, .item-79,
.item-82, .item-84, .item-86, .item-88, .item-90,
.item-91, .item-93, .item-95, .item-97, .item-99 {
  background: rgba(0, 0, 0, 0.5);
}

``` javascript
  test ({
item: '1',
item-2: '2'
});
```
