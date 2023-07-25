# CSS: The Very Basic

## 🎯 Unit Goals -- Things We'll Cover
- Create well-formatted HTML Tables
- Understand when and when not to use tables
- Explain the role of the form element
- Utilize a variety of form controls
- Define complex HTML forms
- Add HTML5 Form Validations
- Ensure accessibility of our forms


## 🙋 WHAT IS CSS?

CSS is a language for describing how
documents are presented visually - how they
are arranged and styled.

## 🙋 WHAT DOES IT STAND FOR?

CSS stands for Cascading Style Sheets. We'll
cover the "cascading" part in a bit; don't worry about it for now!

## 🙆 THERE'S A LOT!

CSS is very easy to get the hang of, but it can
be intimidating because of how many
properties we can manipulate.

## 📋 CSS RULES
(almost) everything you do in CSS

follows this basic pattern:
``` code
    selector {
        property: value;
    }
```

Make all `<h1>` elements purple
``` code
    h1 {
        color: purple;
    }
```

Make all image elements
100 pixels wide & 200 pixels tall
```code
    img {
        width: 100px;
        height: 200px;
    }
```

FANCIER!!

Select every other text input and give it a red border:
```code
    input[type="text"]:nth-of-type(2n) {
        border:2px solid red;
    }
```
----

## 🔎 So Many CSS Border Properties

### INLINE STYLES
You can write your styles directly inline on
each element, but this is NOT A GOOD IDEA
most of the time.

### THE `<STYLE>` ELEMENT
You can write your styles inside of a `<style>`
element. This is easy, but it makes it
impossible to share styles between
documents. Not recommended either.

### EXTERNAL STYLESHEET
Write your styles in a .css file, and then
include the using a `<link>` in the head of your
html document. **Recommended!**

## 📄 CSS Text Properties
- text-align
- font-weight
- text-decoration
- line-height
- letter-spacing

## 📏 Font Size

### Relative:
- EM
- REM
- VH
- %
- AND MORE!

### Absolute:
- PX
- PT
- CM
- IN
- MM
---

### Absolute Unit

**PX - BY FAR THE MOST
COMMONLY USED ABSOLUTE UNIT**

1px does not necessarily equal the width
of exactly one pixel!

Not recommended for responsive websites.

### em

**EM'S ARE RELATIVE UNITS**

With font-size, 1em equals the font-size
of the parent. 2em's is twice the font-
size of the parent, etc.

With other properties, 1em is equal to
the computed font-size of the element
itself.

### rem

**ROOT EMS**

Relative to the root html element's
font-size. Often easier to work with.

If the root font-size is 20px, 1 rem is
always 20px, 2rem is always 40px, etc.