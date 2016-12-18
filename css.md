---
layout: page
title: CSS
subtitle: Mám rád barvy, efekty a layout
---

Kaskádové styly, neboli Cascade Stylesheet slouží k definování rozložení a celkového vzhledu HTML dokumentu. Její syntaxe je velice jednoduchá.

```css
/* Toto je CSS komentář */
#selektor {
   vlastnost1: hodnota1;
   vlastnost2: hodnota2;
}
```

### Komentář
Stejně jako u HTML, i CSS má komentáře. Značí se ovšem jinou sekvencí znaků, to bude platit i později u dalších jazyků. Každý má svůj vlastní způsob psaní komentářů.

### Selektor
Selektor je označení, kterého HTML elementu se daný blok vlastností týká. Může se jednat o HTML tag, jeho třídu `.class`, `#ID`, pseudotřídu `:hover`, či jakýkoliv jiný HTML atribut `[title=jaknaweb]`.

### Vlastnosti
Vlastnosti, jak název již napovídá, definují jednotlivou vlastnost kterou budeme chtít upravit. Vlastnosti se kaskádově dědí z rodičovské třídy na potomky - proto kaskádové styly. Povolené vlastnosti závisí na použité verzi CSS a jejich seznam najdete v oficiální dokumentaci. Nutno podotknout, že ne všechny prohlížeče podporují všechny atributy, a některé jsou specifické pro jednotlivé prohlížeče.

### Hodnota
Říká, jak má daná vlastnost vypadat. Pokud je vlastností barva (color), hodnotou může být například `black`, ale také funkce `rgba(0, 0, 0, 0)` nebo hexadecimální kód barvy `#ffffff`. 