# Formulaire

### Balise `<form>`

- **Usage** : Sert de conteneur pour les éléments du formulaire.
- **Attributs importants** :
  - `action` : L'URL du serveur où les données du formulaire seront soumises.
  - `method` : Méthode HTTP pour l'envoi du formulaire (généralement `get` ou `post`).

  ```html
  <form action="url_de_traitement" method="post">
    <!-- Éléments de formulaire ici -->
  </form>
  ```

### Balise `<input>`

- **Usage** : Utilisée pour différents types de champs de saisie.
- **Types communs** :
  - `text` : Champ de texte standard.
  - `password` : Champ de mot de passe (les caractères sont masqués).
  - `submit` : Bouton pour soumettre le formulaire.
  - `radio` : Bouton radio (sélection unique parmi plusieurs choix).
  - `checkbox` : Case à cocher (sélections multiples possibles).
  - `file` : Téléversement de fichier.
  - `hidden` : Champ caché (pas visible par l'utilisateur, mais soumis avec le formulaire).
  - `email`, `tel`, `number` : Pour des saisies spécifiques (email, téléphone, nombre).

  ```html
  <input type="text" name="nom_utilisateur">
  <input type="password" name="mot_de_passe">
  ```

### Balise `<label>`

- **Usage** : Fournit une étiquette pour les éléments `input`.
- **Attribut important** :
  - `for` : Associe le label à un élément `input` spécifique (doit correspondre à l'ID de l'input).

  ```html
  <label for="nom_utilisateur">Nom d'utilisateur:</label>
  <input type="text" id="nom_utilisateur" name="nom_utilisateur">
  ```

### Balise `<textarea>`

- **Usage** : Champ de texte multi-lignes pour les saisies plus longues.
- **Attributs** : `name`, `rows`, `cols`.

  ```html
  <textarea name="message" rows="4" cols="50"></textarea>
  ```

### Balise `<select>` et `<option>`

- **Usage** : Crée une liste déroulante.
- **`<select>`** : Définit la liste déroulante.
- **`<option>`** : Définit les choix individuels dans la liste.

  ```html
  <select name="pays">
    <option value="france">France</option>
    <option value="espagne">Espagne</option>
    <!-- Autres options -->
  </select>
  ```

### Balise `<button>`

- **Usage** : Bouton personnalisable pour soumettre le formulaire ou d'autres interactions.
- **Attributs** : `type` (par exemple, `submit`, `reset`, `button`), `name`.

  ```html
  <button type="submit">Envoyer</button>
  ```

### Balise `<fieldset>` et `<legend>`

- **Usage** : Groupe plusieurs contrôles de formulaire et ajoute une légende.
- **`<fieldset>`** : Conteneur pour grouper les éléments.
- **`<legend>`** : Titre pour le groupe de champs.

  ```html
  <fieldset>
    <legend>Informations personnelles</legend>
    <!-- Éléments de formulaire ici -->
  </fieldset>
  ```

### Autres éléments

- **Attributs de formulaire courants** : `placeholder` (texte d'indication), `required` (champ obligatoire), `autofocus` (focus automatique), `value` (valeur par défaut).

