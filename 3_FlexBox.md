# Bootstrap Partie  : LES POSITIONNEMENTS 

## Les grilles

### Créer une grille

```html
<html>
<!-- Dans la grille ci-dessous les deux éléments finissent par être l'un en-dessous de l'autre -->
<div class="row">
    <div class="col-md-4 col-sm-6">
        <div class="bg-danger p-4"></div>
    </div>
    <div class="col-md-4 col-sm-6">
        <div class="bg-info p-4"></div>
    </div>
</div>
 
<!-- Dans la grille ci-dessous l'élément prend toute la largeur -->
<div class="row">
    <div class="col">
        <div class="bg-secondary p-4"></div>
    </div>
</div>
</html>
```

### Prioriser nos éléments

On utilise pour ça la classe .order- suivi de la position que l'on veut donner à notre élément.  
Cette classe s'utilise sur la colonne. On peut également utiliser les breakpoints pour dire à un élément sa position en fonction de la taille du navigateur.  

### Décaler d'un certains nombre

On peut décaler d'un certains nombre de colonnes nos éléments vers la droite. Pour ça nous utilisons la classe .offset- suivi de 1 à 11 en fonction du nombre de colonnes que nous voulons.  
On peut également utiliser les breakpoints pour dire à un élément le nombre de colonnes qu'il décalera en fonction de la taille du navigateur.  

### Espacer les éléments

Pour espacer, nous allons utiliser ce que nous appelons des gouttières. On peut les utiliser de trois manières différentes:  

g- - Pour un espacement de toutes les côtés  

gx- - Pour un espacement du côté gauche et droite (horizontal)  

gy- - Pour un espacement du côté haut et bas (vertical)  

On associe ensuite un nombre entre 0 à 5 (aucun espace avec 0, énormément avec 5).  

### Aligner verticalement

Nous pouvons utiliser la classe .align-self-center et .align-self-end sur les colonnes que nous voulons aligner verticalement. Si nous souhaitons aligner tous les éléments d'une ligne au centre, nous pouvons utiliser .align-items-center et .align-items-end sur la classe .row.    

## Flexbox et Bootstrap

### Utiliser Flexbox

```html
<html>
<div class="d-flex">
 
</div>
</html>
```

### Donner une direction

```html
<html>
<div class="d-flex flex-row">
 
</div>
 
<!--
    On a également
    
    - flex-row-reverse
    - flex-column
    - flex-column-reverse
-->
</html>
```

### Aligner les éléments

On peut utiliser la propriété justify-content: start avec la classe .justify-content-start sur le container (.d-flex).  
Toutes les valeurs sont acceptées : end, center, between, around, evenly.  

Nous pouvons utiliser aussi la propriété align-items: center avec la classe .align-items-center et il en est de même avec .align-self-center si nous voulons centrer non pas tous les éléments mais un seul élément.  
Toutes les valeurs sont acceptées : start, end, baseline, stretch.  

### Donner des proportions identiques

Il est possible de donner des proportions identiques, comme avec flex-grow: 1 grâce à la classe .flex-grow-1.  

### Wrapper des éléments

Pour wrapper des éléments, on peut utiliser .flex-wrap ou .flex-wrap-reverse.  
La classe .flex-nowrap vient annuler l'effet.  

### Désigner un ordre

On peut désigner un ordre avec la classe .order- qui va de 1 à 5.  
