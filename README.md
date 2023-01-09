<!-- Preview = Ctrl + Maj + V on VsCode-->


# Méthodes JavaScript (Array)
#### Comment choisir la méthode la plus approprié pour un tableau
* ##### Exercice 1: Doubler chaque élément de mon tableau. 


>const someArr = [1,2,3,4,5];

```bash
const doubleArr = someArr.map(e => e * 2)
console.log(doubleArr)

## Résultat attendu: 
### Tableau de même longueur mais différent -> méthode map().
```

*********
* ##### Exercice 2: Afficher les éléments pair/impair de mon tableau. 

```bash
const evenArr = someArr.filter(e => e % 2 == 0)
const oddArr = someArr.filter(e => e % 2 !== 0)
console.log(evenArr)
console.log(oddArr)

## Résultat attendu: 
### Mon tableau de sortie est plus petit en longueur | méthode filter().
```


*********
* ##### Exercice 3: Afficher les valeurs max/min. 

```bash
const maxValueArr = someArr.reduce((max, e) => Math.max(max, e))
const minValueArr = someArr.reduce((max, e) => Math.min(max, e))

console.log(maxValueArr)
console.log(minValueArr)

## Résultat attendu:
### Mon tableau de sortie est une valeur | méthode reduce().
```

*********
* ##### Exercice 4: Obtenir la somme des valeurs de mon tableau. 

```bash
const sumValueArr = someArr.reduce((sum, e) => sum + e)
console.log(sumValueArr)

## Résultat attendu:
### Mon tableau de sortie est une valeur | méthode reduce() .
```

*********
* ##### Exercice 5: Retourner si un élément de mon tableau est pair. 

```bash
const isOddValueArr = someArr.filter(e => e % 2 != 0).length != 0
console.log(isOddValueArr)

## Résultat attendu:
### Mon tableau de sortie est plus petit en longueur -> filter().
```

