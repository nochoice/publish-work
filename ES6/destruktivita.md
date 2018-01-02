# Destruktivita v Javascripte (ES6) [Javascript destructure]

T�to nov� vlastnost jazyka vyu��vam najcastej�ie. A je aj jednou y najjednoduch��ch. Pomocou nej m�te mo�nost *vybrat* premenn�, ktor� sa nach�dzaj� v `objektoch` alebo `poli`.

```javascript
const osoba = {
	meno: 'J�n',
	priezvisko: 'Polka',
	vek: 36
};
let {meno, priezvisko} = osoba;

console.log(meno);
// <--- 'J�n'
console.log(priezvisko);
// <--- 'Polka'
```