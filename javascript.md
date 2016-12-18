---
layout: page
title: Javascript
subtitle: Protože statické stránky jsou nuda
---

Javascript je klientský skriptovací jazyk. To znamená, že veškerý kód probíhá na straně klienta (webového prohlížeče). To nám dovoluje manipulovat s HTML tagy, měnit jejich vzhled a obsah, přidávat efekty a mnoho dalšího.

Může se vyskytovat v různých formách. Nejběžnější formou je ve vlastním souboru s příponou .js. Může být také součástí HTML dokumentu jako obsah tagu <script>. Poslední možnou formou je inline jako atribut HTML tagu.

Jelikož čistý JS není příliš „pěkný“ na psaní, vzniklo mnoho dalších knihoven a frameworků, jako je jQuery, Angular, nebo čím dál více populární Vue JS, které mají za cíl usnadnit práci a také přidávají mnoho běžně používaných funkcí.

Níže je ukázka, jak můžeme pomocí Javascriptu vytáhnout z DOM element a dynamicky změnit jeho obsah.

```html
<script type=“text/javascript“>

/* Toto je JS komentář*/
// Toto je jednořádkový komentář


// Vytáhneme si náš element
var el = document.getElementById(„myspan“);

// A změníme jeho obsah
el.innerHTML = „sometext“;

</script>
```