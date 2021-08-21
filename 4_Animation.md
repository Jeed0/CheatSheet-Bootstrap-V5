# Bootstrap Partie 4 : Les composants d'animation

## Les barres de navigation responsives

```html
<html>
<nav class="navbar navbar-dark bg-dark navbar-expand-md">
    <div class="container">
        <div class="navbar-brand">
            Smoosh
        </div>
        <!-- Le bouton s'affichera en petit écran -->
        <button class="navbar-toggler" data-bs-toggle="collapse" data-bs-target="#monMenuDeroulant">
            <span class="navbar-toggler-icon"></span>
        </button>
 
        <div class="collapse navbar-collapse" id="monMenuDeroulant">
            <ul class="navbar-nav">
                <li class="nav-item">
                    <a href="#" class="nav-link active">Accueil</a>
                </li>
                <li class="nav-item">
                    <a href="#" class="nav-link">Contact</a>
                    </li>
                </ul>
        </div>
    </div>
</nav>
</html>
```

## Les carrousels

```html
<html>
<!-- Créer un carousel -->
<div id="monPetitCarrousel" class="carousel slide carousel-fade" data-bs-ride="carousel">
 
    <!-- Indicateurs -->
    <ul class="carousel-indicators">
        <li data-bs-target="#monPetitCarrousel" data-bs-slide-to="0" class="active"></li>
        <li data-bs-target="#monPetitCarrousel" data-bs-slide-to="1"></li>
    </ul>
 
    <!-- Contenu du carousel -->
    <div class="carousel-inner">
 
        <!-- Premier slide -->
        <div class="carousel-item active" data-bs-interval="1000">
            <img src="https://cdn.pixabay.com/photo/2016/04/09/02/09/please-include-your-comments-1317308_640.jpg"
                    class="w-100 d-block" alt="Japon">
            
            <!-- Description -->
            <div class="carousel-caption">
                <h5>Le printemps arrive !</h5>
                <p>Les fleurs de cerisiers éclosent dans tout le Japon.</p>
            </div>
        </div>
 
        <!-- Deuxième slide -->
        <div class="carousel-item">
            <img src="https://cdn.pixabay.com/photo/2017/01/28/02/24/japan-2014616_640.jpg"
                    class="w-100 d-block" alt="Japon">
            
            <!-- Description -->
        </div>
 
    </div>
 
    <!-- Controles -->
    <a class="carousel-control-prev" href="#monPetitCarrousel" data-bs-slide="prev">
        <span class="carousel-control-prev-icon"></span>
        <span class="sr-only">Précédent</span>
    </a>
    <a class="carousel-control-next" href="#monPetitCarrousel" data-bs-slide="next">
        <span class="carousel-control-next-icon"></span>
        <span class="sr-only">Suivant</span>
    </a>
    
</div>
</html>
```

## Les listes déroulantes

```html
<html>
<!-- Dropdown (liste déroulante) -->
<div class="dropdown m-3">
    <!-- Bouton -->
    <button id="monBoutonBleu" class="btn btn-primary dropdown-toggle" type="button" data-bs-toggle="dropdown">
        Je suis un menu
    </button>
 
    <!-- Les éléments du menu -->
    <ul class="dropdown-menu" aria-labbeledby="monBoutonBleu">
        <li><a class="dropdown-item" href="#">Action</a></li>
        <li><a class="dropdown-item" href="#">Action</a></li>
        <li><a class="dropdown-item" href="#">Action</a></li>
    </ul>
</div>
 
<!-- Liste déroulant et bouton collés -->
<div class="btn-group m-3 dropup">
    <button type="button" class="btn btn-primary">J'aime</button>
    <button type="button" class="btn btn-primary dropdown-toggle dropdown-toggle-split" data-bs-toggle="dropdown" id="mesOptions">
        <span class="sr-only">Options</span>
    </button>
    <ul class="dropdown-menu" aria-labbeledby="mesOptions">
        <li><a class="dropdown-item" href="#">Action</a></li>
        <li><a class="dropdown-item" href="#">Action</a></li>
        <li><a class="dropdown-item" href="#">Action</a></li>
    </ul>
</div>
</html>
```

## Les fenêtres modales

```html
<html>
<!-- Modale -->
<button type="button" class="btn btn-danger" data-bs-toggle="modal" data-bs-target="#supprimer">
    Supprimer mon compte
</button>
 
<div class="modal fade" id="supprimer" data-bs-backdrop="static">
    <div class="modal-dialog modal-dialog-centered">
        <div class="modal-content">
 
            <!-- Header -->
            <div class="modal-header">
                <h5 class="modal-title">Supprimer mon compte</h5>
                <button type="button" class="btn-close" data-bs-dismiss="modal">
                    <span>&times;</span>
                </button>
            </div>
 
            <!-- Body -->
            <div class="modal-body">
                <p class="m-0">Etes-vous sûr de vous ? C'est très dangereux.</p>
            </div>
 
            <!-- Footer -->
            <div class="modal-footer">
                <button type="button" class="btn btn-outline-secondary" data-bs-dismiss="modal">Fermer</button>
                <button type="button" class="btn btn-danger">Supprimer</button>
            </div>
 
        </div>
    </div>
</div>
</html>
```

## Les infobulles

```html
<html>
<button type="button" class="btn btn-info" data-bs-toggle="tooltip" data-bs-placement="bottom" title="Ma première infobulle">
    Action
</button>
 
<script>
    var tooltipTriggerList = [].slice.call(document.querySelectorAll('[data-bs-toggle="tooltip"]'))
    var tooltipList = tooltipTriggerList.map(function (tooltipTriggerEl) {
        return new bootstrap.Tooltip(tooltipTriggerEl)
    })
</script>
</html>
```

## Les popovers

```html
<html>
<button type="button" class="btn btn-secondary" data-bs-toggle="popover" data-bs-placement="bottom" data-bs-content="Fonctionnalité non créée">
    Fonctionnalité
</button>
 
<script>
    var popoverTriggerList = [].slice.call(document.querySelectorAll('[data-bs-toggle="popover"]'))
    var popoverList = popoverTriggerList.map(function (popoverTriggerEl) {
        return new bootstrap.Popover(popoverTriggerEl)
    })
</script>
</html>
```

## Les "Scrollspy"

Pour espionner le scroll des utilisateurs, nous avons besoin d'ajouter l'attribut data-bs-spy et data-bs-target sur la balise body.

```html
<html>
<body data-bs-spy="scroll" data-bs-target="#menu">
 
</body>
</html>
```

La cible doit toujours être une balise nav qui utilise la classe navbar. Il ne reste qu'à ajouter vos ancres et Bootstrap gérera tout.

## Les spinners

```html
<html>
<!-- Démonstration A -->
<div class="spinner-border text-primary">
    <span class="visually-hidden">Chargement</span>
</div>
 
<!-- Démonstration B -->
<div class="spinner-grow text-primary">
    <span class="visually-hidden">Chargement</span>
</div>
 
<!-- Démonstration C -->
<button type="button" class="btn btn-primary">
    Modifier
    <span class="spinner-border spinner-border-sm"></span>
</button>
</html>
```
