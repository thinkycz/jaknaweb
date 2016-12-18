---
layout: page
title: SQL
subtitle: Poslouchají mě jen databáze
---

Doposud jsme se bavili o webových stránkách, které jsou buď statické, či dynamické, ale bez uživatelských dat. Co když budeme chtít uložit nějaké informace, například o zákazníkovi v našem eshopu? K tomu nám poslouží databáze a SQL.

SQL je zkratka od Structured Query Language a jak již sám název napovídá, nejedná se o programovací jazyk, nýbrž o jazyk dotazovací. Ten se od programovacích jazyků liší tím, že nepíšeme „jak“ se daný úkol má provést, pouze určíme „co“ chceme provést.

Mějme následující tabulku v databázi:

|ID|Jmeno|Prijmeni|Vek|
|:---:|:---:|:---:|:---:|
|1|Leo|Hrách|23|
|2|Anna|Velká|12|
|3|Petr|Hruška|18|
|4|Tom|Veselý|20|

Název této tabulky je „Studenti“.

Tímto dotazem vybereme všechny záznamy:

```sql
SELECT * FROM Studenti;
```

A takto můžeme zjistit průměrný věk všech studentů:

```sql
SELECT avg(Vek) FROM Studenti;
```

Můžeme si všimnout, že jsme nemuseli definovat, jak se počítá průměrný věk (sečtením věku všech studentů a následným vydělením počtem studentů), pouze jsme se dotázali na průměr věků v tabulce.

Dále si můžeme všimnout, že nepsaným pravidlem v SQL je, že se píše VELKÝMI písmeny.

Existuje mnoho druhů SQL databází, nejrozšířenější jsou MySQL, Oracle, MS SQL Server, Sqlite, MariaDB. A ačkoliv existují drobné odlišnosti v jednotlivých platformách, jedno mají ale společné. Všechny používají jako dotazovací jazyk právě jazyk SQL.