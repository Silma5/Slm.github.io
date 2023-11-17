# Introduction CSS
CSS, qui est l'acronyme de Cascading Style Sheets (Feuilles de style en cascade). CSS est un langage de feuille de style utilisé pour décrire la présentation d'un document écrit en HTML ou en XML (y compris des langages basés sur XML comme SVG). CSS décrit comment les éléments doivent être rendus à l'écran, sur du "papier",  ou sur d'autres médias.

## Fondamentaux de CSS

### 1. Syntaxe

- **Sélecteurs** : Identifient l'élément HTML à styliser. Exemples : `p`, `.classe`, `#id`.
- **Déclarations** : Paire propriété-valeur pour styliser le sélecteur. Exemple : `color: red;`.
- **Règles** : Sélecteur suivi d'une ou plusieurs déclarations entourées de `{}`.

  ```css
  p {
    color: red;
    font-size: 14px;
  }
  ```
```css
h1 {
    color: blue;
    font-size: 20px;
}
```


### 2. Ajout de CSS à HTML

- **Interne** : Utiliser `<style>` dans l'en-tête `<head>` du document HTML.
- **Externe** : Lier un fichier CSS externe avec `<link rel="stylesheet" href="style.css">`.
- **Inline** : Style directement dans un attribut `style` d'un élément HTML.

```html
<style>
    body {
        background-color: lightblue;
    }
</style>
```

```html
<link rel="stylesheet" href="styles.css">
```

```html
<p style="color: green;">Ceci est un paragraphe avec un style inline.</p>
```

### 3. Sélecteurs

- **Sélecteur d'élément** : Cible le nom de l'élément, ex : `p`, `div`.
- **Sélecteur de classe** : Cible la classe de l'élément, ex : `.ma-classe`.
- **Sélecteur d'ID** : Cible l'ID de l'élément, ex : `#mon-id`.
- **Sélecteurs avancés** : Combinateurs, pseudo-classes, pseudo-éléments, etc.

```css
p {
    font-size: 16px;
}
```

```css
.ma-classe {
    color: red;
}
```

```css
#mon-id {
    background-color: yellow;
}
```

### 4. Propriétés et Valeurs

- **Texte** : `color`, `font-family`, `font-size`, `text-align`, etc.
- **Boîte** : `margin`, `padding`, `border`, `width`, `height`.
- **Positionnement** : `position`, `top`, `right`, `bottom`, `left`, `float`, `display`.
- **Arrière-plan** : `background-color`, `background-image`, `background-position`.

```css
p {
    color: navy;
    font-family: Arial, sans-serif;
    text-align: center;
}
```

```css
.box {
    margin: 10px;
    padding: 20px;
    border: 1px solid black;
    width: 50%;
}
```

### 5. Box Model

- Tout élément HTML est considéré comme une boîte.
- Comprend `margin`, `border`, `padding`, et la `content area`.
```css
.box {
    width: 300px;
    padding: 10px;
    border: 5px solid gray;
    margin: 20px;
}
```

### 6. Positionnement et Layout

- **Positionnement** : `static`, `relative`, `absolute`, `fixed`, `sticky`.
- **Flexbox** : Système de layout unidimensionnel.
```css
.container {
    display: flex;
    justify-content: space-between;
}
```

- **Grid** : Système de layout bidimensionnel.
```css
.grid-container {
    display: grid;
    grid-template-columns: auto auto auto;
    gap: 10px;
}
```

### 7. Responsive Design

- **Media Queries** : Appliquer des styles en fonction de la taille de l'écran et d'autres caractéristiques de l'appareil.
```css
@media screen and (max-width: 600px) {
    body {
        background-color: lightpink;
    }
}
```


### 8. Animation et Transition

- **Transitions** : Changement doux d'une propriété à une autre.
```css
.box:hover {
    transition: background-color 0.5s ease;
    background-color: coral;
}
```

- **Animations** : Plus complexes, définies avec `@keyframes`.
```css
@keyframes example {
    from {background-color: red;}
    to {background-color: yellow;}
}

.box {
    animation-name: example;
    animation-duration: 4s;
}
```



