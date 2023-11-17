# Exemple Formulaire


```html
<!DOCTYPE html>
<html>
<head>
    <title>Formulaire d'inscription</title>
</head>
<body>

<h2>Formulaire d'inscription</h2>

<form action="/submit_form" method="post">
    <fieldset>
        <legend>Informations personnelles:</legend>

        <label for="nom">Nom:</label><br>
        <input type="text" id="nom" name="nom" required><br>

        <label for="email">Email:</label><br>
        <input type="email" id="email" name="email" required><br>

        <label for="mdp">Mot de passe:</label><br>
        <input type="password" id="mdp" name="mdp" minlength="6" required><br>

        <label for="age">Age:</label><br>
        <input type="number" id="age" name="age"><br>

        <label>Sexe:</label><br>
        <input type="radio" id="feminin" name="sexe" value="feminin">
        <label for="feminin">Féminin</label><br>
        <input type="radio" id="masculin" name="sexe" value="masculin">
        <label for="masculin">Masculin</label><br>

        <label for="bio">Biographie:</label><br>
        <textarea id="bio" name="bio" rows="4" cols="50"></textarea><br>

        <input type="checkbox" id="newsletter" name="newsletter" value="oui">
        <label for="newsletter">S'abonner à la newsletter</label><br>

        <button type="submit">S'inscrire</button>
    </fieldset>
</form>

</body>
</html>
```

### Explications :

- **`<fieldset>` et `<legend>`** : Utilisés pour grouper les éléments du formulaire et ajouter un titre à ce groupe.
- **`<label>`** : Fournit des étiquettes textuelles pour chaque champ de formulaire pour une meilleure accessibilité.
- **`<input>`** : Différents types d'`input` sont utilisés ici, y compris `text`, `email`, `password`, `number`, `radio`, et `checkbox`.
- **`<textarea>`** : Permet aux utilisateurs d'entrer un texte multi-lignes.
- **`<button>`** : Un bouton pour soumettre le formulaire.

### Points à noter :

- L'attribut `action` du formulaire doit être remplacé par l'URL du serveur qui traitera les données du formulaire.
- L'attribut `method` est défini sur `post`, ce qui est approprié pour l'envoi de données sensibles comme les mots de passe.
- Les champs `required` et `minlength` dans les inputs assurent une validation basique côté client.

Ce formulaire est un exemple de base. Vous pouvez l'étendre ou le modifier en fonction des besoins spécifiques de votre application.
