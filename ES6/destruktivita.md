# Destruktivita v Javascripte (ES6) [Javascript destructure]

Túto novú vlastnosť jazyka využívam najcastejšie. A je aj jednou y najjednoduchších. Pomocou nej máte možnost *vybrat* premenné, ktoré sa nachádzajú v `objektoch` alebo `poliach`.

```javascript
const osoba = {
	meno: 'Ján',
	priezvisko: 'Polka',
	vek: 36,
	adresa: {
		ulica: 'Prekotna',
		cislo: 20,
		mesto: 'Brno'
	}
};

let {meno, priezvisko} = osoba;

console.log(meno);		// <--- 'Ján'
console.log(priezvisko);	// <--- 'Polka'
```

Ako máte možnosť vidieť, tak sa objekt rozobral na jeho 2 premenné. Pomocou ES5 by sa to riešilo následovne. 

```javascript
console.log(osoba.meno);	// <--- 'Ján'
console.log(osoba.priezvisko);	// <--- 'Polka'
```

Deštrukcia dáva možnosť aj premapovanie premenných na ich aliasy [meno -> name, priezvisko -> surname].

```javascript
let {meno: name, priezvisko: surname} = osoba;

console.log(name);	// <--- 'Ján'
console.log(surname);	// <--- 'Polka'
```

Samozrejmosťou je možnosť namapovania aj vnorených premenných

```javascript 
let {meno: name, adresa: {ulica: street}} = osoba;

console.log(name);	// <--- 'Ján'
console.log(street);	// <--- 'Prekotna'
```