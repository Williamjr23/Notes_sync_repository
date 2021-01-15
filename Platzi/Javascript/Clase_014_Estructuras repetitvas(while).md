# Estructura "While"

> Nos va a permitr repetr un codgo hasta que se cumpla una condición 

Estructura:
```js
while () {
}
```

### Como funciona?
> El codigo que esté entre las llaves ```{}``` se va a repetir siempre que la condición especificada dentro de los parentesís ```()```se cumpla

Ejemplo:
```js
var willam = {
 nombre: 'Willam',
 apelldo: 'Castillo',
 edad: 18
}

var william = {

}

const INCREMENTO_PESO = 0.3
const DIAS_DEL_ANO - 365

const aumentarDePeso = persona => persona.peso += INCREMENTO_PESO
const adelgazar = persona => persona.peso -= INCREMENTO_PESO
const comeMucho = () => Math.random < 0.3
const realizaDeporte = () => Math.random < 0.4

var dias = 0

const META = willam.peso - 3

while (willam.peso > META) {
	if (comeMUcho()) {
		aumentarDePeso(william)
	}
	if (realizaDeporte()) {
		adelgazar(william)
	}
	dias += 1
}

console.log(`Pasaron ${dias} días hasta que ${william.nombre} adelgazó 3kg`)
```