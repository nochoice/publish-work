# Destruktivita v Javascripte (ES6) [Javascript destructure]

Túto novú vlastnosť jazyka využívam najcastejšie. A je aj jednou y najjednoduchších. Pomocou nej máte možnost *vybrat* premenné, ktoré sa nachádzajú v `objektoch` alebo `poli`.

```javascript
const osoba = {
	meno: 'Ján',
	priezvisko: 'Polka',
	vek: 36
};

let {meno, priezvisko} = osoba;

console.log(meno);		// <--- 'Ján'
console.log(priezvisko);	// <--- 'Polka'
```