# Bootstrap Partie 2 : LES COMPOSANTS

## Les composants CSS

### Les boutons

```html
<html>
<div class="btn-group-vertical">
    <button class="btn btn-primary">Bouton principal</button>
    <button class="btn btn-outline-primary">Bouton secondaire</button>
</div>
<button class="btn btn-primary btn-block" disabled>Lien</button>
</html>
```

### Les alertes

```html
<html>
<div class="alert alert-info">
    <h3 class="alert-heading">Bienvenue !</h3>
    Ceci est une notification et ceci un <a href="#" class="alert-link">lien</a>
</div>
</html>
```

### Les barres de navigation

```html
<html>
<nav class="navbar navbar-dark bg-dark navbar-expand">
    <div class="container">
        <div class="navbar-brand">
            Smoosh
        </div>
 
        <div class="collapse navbar-collapse">
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

### Les badges

```html
<html>
<h3>Les meilleurs restaurants de Paris <span class="badge bg-secondary">New</span></h3>
<button type="button" class="btn btn-primary">
    Demandes d'ami <span class="badge bg-dark">5</span>
</button>
</html>
```

### Les formulaires

```html
<html>
<form class="mt-5">
    <p>
        <label for="prenom" class="form-label">Prénom</label>
        <input type="text" name="prenom" id="prenom" class="form-control">
    </p>
 
    <p>
        <label for="pays" class="form-label">Pays</label>
        <select name="pays" id="pays" class="form-select">
            <option value="France">France</option>
            <option value="Suisse">Suisse</option>
            <option value="Congo">Congo</option>
        </select>
    </p>
 
    <p>
        <input type="file" name="fichier" class="form-control">
    </p>
 
    <p>
        <label for="email" class="form-label">Adresse email</label>
        <input type="email" name="email" id="email" readonly value="john@gmail.com" class="form-control-plaintext">
    </p>
 
    <p class="form-check">
        <input type="checkbox" name="mode_sombre" class="form-check-input" id="mode_sombre">
        <label for="mode_sombre" class="form-check-label">Mode sombre</label>
    </p>
 
    <p class="form-check form-switch">
        <input type="checkbox" name="mode_sombre" class="form-check-input" id="mode_sombre_pour_switch">
        <label for="mode_sombre_pour_switch" class="form-check-label">Mode sombre</label>
    </p>
</form>
</html>
```

### Regrouper ses champs de formulaire

```html
<html>
<p>
    <label for="email" class="form-label">Adresse email</label>
    <div class="input-group">
        <span class="input-group-text">
            https://www.youtube.com/watch?v=
        </span>
        <input type="email" name="email" id="email" class="form-control">
    </div>
</p>
 
<p>
    <div class="input-group">
        <span class="input-group-text">
            Vos motivations ?
        </span>
        <textarea class="form-control"></textarea>
    </div>
</p>
</html>
```

### Les cartes

```html
<html>
<div class="card">
    <!-- Image d'illustration -->
    <img src="https://cdn.pixabay.com/photo/2018/07/26/07/45/valais-3562988_640.jpg"
        class="card-img-top" alt="Montagnes">
 
    <!-- En-tête de la carte -->
    <div class="card-header">
        Destination
    </div>
 
    <!-- Corps -->
    <div class="card-body">
        <h5 class="card-title">Titre</h5>
        <h6 class="card-subtitle text-muted">Destination</h6>
        <p class="card-text">Ceci est un exemple de carte
            que Bootstrap nous permet de créer.
        </p>
        <a href="#" class="card-link">En savoir plus</a>
        <a href="#" class="card-link">Réserver</a>
    </div>
 
    <!-- Pied -->
    <div class="card-footer p-0">
        <ul class="list-group list-group-flush">
            <li class="list-group-item">Visiter les pyrénées</li>
            <li class="list-group-item">Visiter le jura</li>
        </ul>
    </div>
</div>
</html>
```

### Les barres de progression

```html
<html>
<div class="progress">
    <div class="progress-bar w-25">25%</div>
</div>
 
<div class="progress mt-1">
    <div class="progress-bar w-25">25%</div>
    <div class="progress-bar bg-success w-50">50%</div>
</div>
 
<div class="progress mt-1">
    <div class="progress-bar progress-bar-striped progress-bar-animated bg-dark w-75">25%</div>
</div>
</html>
```

### Les fils d'ariana

```html
<html>
<nav>
    <ul class="breadcrumb">
        <li class="breadcrumb-item">
            <a href="#">Accueil</a>
        </li>
        <li class="breadcrumb-item">
            <a href="#">Destination</a>
        </li>
        <li class="breadcrumb-item">
            <a href="#">Les pyrénées</a>
        </li>
    </ul>
</nav>
</html>
```
