---
layout: page
title: HTML
subtitle: Dávám textovým dokumentům značky
---

Základním stavebním kamenem každého webu je HTML. Poznáme ho jednoduše pomocí zobáčků, ve kterých jsou tagy.

```html
<!-- Toto je HTML komentář -->
<a href="http://jaknaweb.thinky.cz/html" class="odkaz">Jak na Web</a>
```

### Komentář
Komentáře slouží pro programátory k zápisu užitečných informací, většinou pro zpřehlednění zdrojového kódu. Prohližeče ho ignorují.

### Otevírací tag
Primárním elementem HTML kódu jsou otevírací tagy. Mnoho z nich má své vlastnosti a chování, například `<a>` znamená anchor, neboli kotva. Existují však i tagy bez vlastního významu. Těmi jsou například `<div>` a `<span>`. Jejich vlastnosti se poté definují pomocí CSS, a chování většinou Javascriptem. Může obsahovat atributy.

### Atributy
Většina tagů může mít atributy, ale nemusí. Ty dávají tagům přidanou informační hodnotu. Pomocí atributů class nebo id lze například v CSS a JS dohledat daný element. Hodně atributů má hodnotu, ale jsou i takové, které hodnotu nemají. Jedním z nich je například `disabled`.

### Uzavírací tag
Většina tagů musí být uzavřena pomocí uzavíracího tagu, aby bylo zřejmé, kde obsah daného tagu končí. Existují ale i tzv. samouzavírací tagy, které nemají obsah. Přiklady jsou `<br />`, `<img />`.