---
layout: page
title: PHP
subtitle: Server je pro mě domov
---

Počínaje touto kapitolou se budeme věnovat serverovým technologiím. Ty se liší od klientských tím, že kód běží na vzdáleném serveru, kde se vygeneruje odpověď, která se vrátí klientovi.

Odpovědí je obvykle HTML stránka, ale může jí být také JSON, XML, nebo jakýkoliv jiný HTTP ContentType. Klientem je pak webový prohlížeč, nebo jakákoliv jiná aplikace posílající HTTP Request.

```php
<?php
   echo 'Ja jsem PHP';
?>
```

### Základní skladba
PHP se může vyskytovat jak v rámci HTML souboru, tak i jako samostatný soubor PHP. Vždy začíná značkou <?php a končí ?>, ale koncová značka se doporučuje psát pouze u inline zápisu. Jednotlivé funkce se zakončují středníkem.

### Proměnné, konstanty, pole
Úplným základem každého programovacího jazyka jsou proměnné. Umožňují nám si někam zapsat nějakou hodnotu, a přiřadit jí název, pomocí kterého se k dané hodnotě opět dostaneme. V PHP se proměnné deklarují takto:

```php
$proměnná = 5; //definice
$proměnná = 6; //změna hodnoty

const konstanta = 10;

$pole = [1, 3, 3];
$pole[1] = 2; //změna hodnoty
//pole je nyní [1, 2, 3]
```

Všimněme si, že každá proměnná začíná znakem pro dolar. Konstanta je pak proměnná, které nemůžeme v budoucnu změnit hodnotu.
Pole je jednoduše řečeno proměnná, která má naopak více hodnot. K hodnotám v poli se dostaneme pomocí indexu. Indexy začínají od nuly.

### Operátory
S jedním operátorem jsme se již setkali na předchozí stránce. Byl to operátor přiřazení, který proměnné přiřadil hodnotu. Dalšími operátory v PHP jsou např.:

```php
//aritmeticke + - * / %
$soucet = 1 + 1;

//porovnavaci == > >= < <= <> ===
$jeVetsi = 1 > 2; //false

//logicke && || !
$plati = $podminka1 && !$podminka2;

//konkatenace .
$veta = ‘ahoj‘ . ‘jak se vede‘;
```

### Řídící struktury
Pokud budeme chtít provést nějaké operace pouze za určitých podmínek, či provést stejnou operaci mnohokrát za sebou, budeme muset použít řídící struktury. Těmi jsou např. `if`, `switch`, `for`, `foreach`, `while`...

```php
if($cislo > 0) {
   echo ‘Cislo je kladne‘;
} else {
   echo ‘Cislo je zaporne ci nula‘;
}
```

### Funkce
Představme si objekt, který má vstup a výstup. Vstupem může být například číslo, a výstupem jiné číslo. Tomuto objektu, který něco dělá, se v programování říká funkce. Můžeme ji zapsat takto:

```php
function odmocnina($cislo) {
   return sqrt($cislo);
}
```

Naše funkce v tomto případě se jmenuje odmocnina, a přijímá jedno číslo, a jejím výstupem je odmocnina z daného čísla. Naše funkce není příliš užitečná, jelikož jsme pouze „obalili“ funkci `sqrt()`, přičemž její funkcionalita je stále stejná.
Funkce `sqrt()` je jednou ze základních funkcí jazyka PHP. Seznam všech dostupných funkcí můžete najít v oficiální dokumentaci.

### Objektově orientované PHP
PHP je objektově orientovaný jazyk. Podporuje třídy, dědičnost, polymorfismus, zapouzdřenost a mnoho dalších vlastností.
Jelikož by OOP vyšlo na samostatnou knížku, v naši základní příručce se OOP nebudeme věnovat.