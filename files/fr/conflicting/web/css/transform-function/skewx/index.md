---
title: skewY()
slug: conflicting/Web/CSS/transform-function/skewX
translation_of: Web/CSS/transform-function/skewY()
original_slug: Web/CSS/transform-function/skewY()
browser-compat: css.types.transform-function.skewY
---
{{CSSRef}}

La fonction **`skewY()`** permet d'opérer une distorsion verticale en étirant chaque point de l'élément d'un certain angle dans la direction verticale. Pour cela, on augmente l'ordonnée d'un élément d'une valeur proportionnelle à l'angle donné et à la distance de l'origine. Plus le point est éloigné de l'origine et loin de l'axe, plus le décalage obtenu sera important.

{{EmbedInteractiveExample("pages/css/function-skewY.html")}}

La valeur obtenue par cette fonction est de type [`<transform-function>`](/fr/docs/Web/CSS/transform-function).

## Syntaxe

```css
skewY(a)
```

### Valeurs

- `a`
  - : Une valeur de type [`<angle>`](/fr/docs/Web/CSS/angle) qui représente l'angle avec lequel appliquer la distorsion selon l'axe des ordonnées (axe vertical).

<table class="standard-table">
  <thead>
    <tr>
      <th scope="col">Coordonnées cartésiennes sur ℝ<sup>2</sup></th>
      <th scope="col">Coordonnées homogènes sur ℝℙ<sup>2</sup></th>
      <th scope="col">Coordonnées cartésiennes sur ℝ<sup>3</sup></th>
      <th scope="col">Coordonnées homogènes sur ℝℙ<sup>3</sup></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td colspan="1" rowspan="2">
        <math
          ><mfenced
            ><mtable
              ><mtr>1<mtd>0</mtd></mtr
              ><mtr>tan(ax)<mtd>1</mtd></mtr></mtable
            ></mfenced
          ></math
        >
      </td>
      <td>
        <math
          ><mfenced
            ><mtable
              ><mtr>1<mtd>0</mtd><mtd>0</mtd></mtr
              ><mtr>tan(ax)<mtd>1</mtd><mtd>0</mtd></mtr
              ><mtr><mtd>0</mtd><mtd>0</mtd><mtd>1</mtd></mtr></mtable
            ></mfenced
          ></math
        >
      </td>
      <td colspan="1" rowspan="2">
        <math
          ><mfenced
            ><mtable
              ><mtr>1<mtd>0</mtd><mtd>0</mtd></mtr
              ><mtr>tan(ax)<mtd>1</mtd><mtd>0</mtd></mtr
              ><mtr><mtd>0</mtd><mtd>0</mtd><mtd>1</mtd></mtr></mtable
            ></mfenced
          ></math
        >
      </td>
      <td colspan="1" rowspan="2">
        <math
          ><mfenced
            ><mtable
              ><mtr>1<mtd>0</mtd><mtd>0</mtd><mtd>0</mtd></mtr
              ><mtr>tan(ax)<mtd>1</mtd><mtd>0</mtd><mtd>0</mtd></mtr
              ><mtr><mtd>0</mtd><mtd>0</mtd><mtd>1</mtd><mtd>0</mtd></mtr
              ><mtr
                ><mtd>0</mtd><mtd>0</mtd><mtd>0</mtd><mtd>1</mtd></mtr
              ></mtable
            ></mfenced
          ></math
        >
      </td>
    </tr>
    <tr>
      <td><code>[1 tan(a) 0 1 0 0]</code></td>
    </tr>
  </tbody>
</table>

## Exemples

### HTML

```html
<div>Normal</div>
<div class="skewed">Distordu</div>
```

### CSS

```css
div {
  width: 80px;
  height: 80px;
  background-color: skyblue;
}

.skewed {
  transform: skewY(40deg);
  background-color: pink;
}
```

### Résultat

{{EmbedLiveSample("Exemples","100%","250")}}

## Specifications

{{Specifications}}

## Compatibilité des navigateurs

{{Compat}}

## Voir aussi

- [`transform`](/fr/docs/Web/CSS/transform)
- [`<transform-function>`](/fr/docs/Web/CSS/transform-function)
