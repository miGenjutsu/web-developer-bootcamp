# CSS: The World of CSS Selectors

## 📋 CSS RULES
Everything you do in CSS
follows this basic pattern:
```bash
selector {
    property: value;
}

```

Make all `<h1>` elements purple
```bash
h1 {
    color: purple;
}
```

## ✨ FANCIER!

Select every other text input and give it a red border:
```bash
input[type="text"]:nth-of-type(2n){
    border:2px solid red;
}
```

## 📋 CSS RULES
#### 📌 ELEMENT SELECTOR: select everything
```bash
    * {
        color: black;
    }
```

#### 📌 ELEMENT SELECTOR: select all images

```bash
    img {
        width: 100px;
        height: 200px;
    }
```

#### 📌 SELECTOR LIST: select all h1s and h2s
```bash
    h1,h2 {
        color: magenta;
    }

```

#### 📌 CLASS SELCTOR: select elements with class of 'complete'
```bash
    .complete {
        color: green;
    }

```

#### 📌 ID SELECTOR: select the element with id of 'logout'
```bash
    #logout {
        color: orange;
        height: 200px;
    }
```

#### 📌 DESCENDANT SELECTOR: select all `<a>`'s that are nested inside an `<li>`
```bash
    li a {
        color: teal;
    }
```

#### 📌 ADJACENT SELECTOR: select only the paragraphs that are immediately preceded by and `<h1>`
```bash
h1 + p {
    color: red:
}
```

#### 📌 DIRECT CHILD: select only the `<li>`'s that are direct children of `<div>` element
```bash
    div > li {
        color: white;
    }

```

#### 📌 ATTRIBUTE SELECTOR: select all input elements where the type attribute is set to "text"
```bash
    input[type="text"] {
        width: 300px;
        color: yellow;
    }
```

----


## 🧑🏽‍🎓 Psuedo Classes

keyword added to a selector that
specifies a special state of the
selected element(s)
- :active
- :checked
- :first
- :first-child
- :hover
- :not()
- :nth-child()
- :nth-of-type()

## 📍 Psuedo Elements
Keyword added to a selector that lets
you style a particular part of
selected element(s)

- ::after
- ::before
- ::first-letter
- ::first-line
- ::selection
--------


## 🙋🏾 What happens when conflicting styles target the same elements?

### The Cascade
The order your styles are declared in
and linked to matters!
```bash
    h1 {
        color: red;
    }

    h1 {
        color: purple;
    }
```

📢 PURPLE WINS

## ⚡️ SPECIFICITY
Specificity is how the browser decides
which rules to apply when multiple
rules could apply to the same element.

It is a measure of how specific a
given selector is. The more specific
selector "wins"

#### 📌 Element Selector
```bash
    p {
        color: yellow;
    }
```

#### 📌 Element Selector + Element Selector
```bash
    section p {
        color: teal;
    }
```