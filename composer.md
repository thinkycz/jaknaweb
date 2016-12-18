---
layout: page
title: Composer
subtitle: Jsem rád když vývojáři spolupracují
---

Neustále výmýšlet kolo je nuda. Obzvláště pokud víme, že ho již někdo vynalezl. To samé platí s kódem. Nač psát jednu a tu samou funkcionalitu neustále dokola, když jí někdo již v minulosti napsal? Přesně k tomu slouží Composer.

Composer je nástroj pro správu balíčků a jejich závislostí (package manager) pro PHP projekty. Dovoluje nám definovat, jaké knihovny (kód třetích stran) náš projekt bude potřebovat, a také nám je nainstaluje, spolu se všemi závislostmi jednotlivých knihoven.

Composer je PHAR (PHP Archive) soubor, který je spustitelný v příkazové řádce. Pro jeho spuštění je nutno mít v projektu soubor composer.json, ve kterém máme nadefinované naše závislosti:

```json
{
    "require": {
        "php": ">=5.6.1",
        "laravel/framework": "5.3.*"
    }
}
```

Nyní již stačí zadat do terminálu:

```
composer install
```

Tímto nám Composer ověří, že máme správnou verzi PHP a také stáhne framework laravel a jeho závislosti do adresáře vendor.

### Autoloader
Jedna z nejlepších funkcí composeru je jeho autoloader. Za normálních okolností bychom museli každý další php soubor „zaregistrovat“ do našeho projektu tak, abychom s nimi mohli pracovat. To je velice obtížné vzhledem k tomu, že některé knihovny mají stovky až tisíce souborů.

Composer proto vytvořil v adresáři vendor soubor s názvem autoload.php. Nyní, vše co musíme udělat je načíst tento jeden soubor:

```php
require '/vendor/autoload.php';
```