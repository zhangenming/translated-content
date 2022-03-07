---
title: ':-moz-broken'
slug: Web/CSS/:-moz-broken
tags:
  - CSS
  - Non-standard
  - Pseudo-classe
  - Reference
translation_of: Web/CSS/:-moz-broken
---
{{Non-standard_header}}{{CSSRef}}{{gecko_minversion_header("1.9")}}

La [p](/en-US/docs/Web/CSS)[seudo-class CSS](/fr/docs/Web/CSS/Pseudo-classes) `:-moz-broken` s'adapte aux éléments qui représentent des liens cassés vers des images.

Ce sélecteur est principalement destiné à être utilisé par les développeurs de thèmes.

## Syntaxe

    :-moz-broken

## Exemples

### HTML

```html
<img src="broken.jpg" alt="Cette image ne fonctionne pas. :-(">
```

### CSS

```css
:-moz-broken {
  background: bisque;
  padding: 8px;
}
```

### Résultat

{{EmbedLiveSample("Exemples")}}

## Voir aussi

- {{bug("11011")}}
- {{cssxref(":-moz-loading")}}, {{cssxref(":-moz-suppressed")}}, {{cssxref(":-moz-user-disabled")}}
