
Javascript je bordel - a to je dobre

Javsascript nikdy nemaže staré features - nové verzie sú stále spatne kompatibilné. Prial by som si, keby sa to dalo vyčisť, ale ostať kompatibilmý má príliš veľa výhod.

Niektoré z nich sa pokúsim popísať v nasledujúcom texte.

1. Benefity spätnej kompatibility

- Je jedonduché prechádzať na novšie verzie jazyka. Príchodom ES6 všetky staré napísané riadky kódu fungovali.
-  Kód nie je potrebné verzovať. V prípade, že dovolíte označiť niečo za nové a iné zase za staré tak s adostanete do"
  - Prekladače (impretetory) budú musieť byť zložitejšie
  - Programátory si budú musieť dávať pozor na verzie
  - Už nemáte možnosť prehadzovať s kódom na rôzne miesta

2. Tipy ako si poradiť s narastajúcim JS
- Študovanie (vydelávanie) - nemusíte sa učiť staré konštrukcie. Je však dobré o nich vedieť a aspoň tušiť, čé sa za nimi skrýva
- Nechajte nech vám lintery pomôžu

3. Čistejší JS
Ak chcete aby váš kód ostal čo najčistejší tak môžete ignorovať nasledujúce 
- namiesto var používajte let a const
- function - používajte tzv. arrow funkcie
- Promisy - používajte async function
- Itrerovanie cez objekt. Lepšie je použiť Map()
- Cykly - for-in (vyhnúť sa vždy), for (vyhnúť sa ak je to možné). Používajte for-of
- arguments - použiť rest operátor ... (...args)
- Constructor functions - používajte class
