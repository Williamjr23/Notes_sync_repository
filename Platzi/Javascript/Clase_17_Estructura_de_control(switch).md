# Switch

nos va a permiitir decidir que codigo ejecutar de acuerdo a multiples condiciones 


Cuando tenes muchos ```if``` que hacen referencia a la misma entrada se puede utilizar mejor ```switch```en lugar de llenar todo nuestro cógio de ```if```s y esa es una forma de darte cuenta que puedes aplicar esta estructura 

Forma de utlizarse:

```js 
switch (signo) {
	case 'aries':
	console.log('Prepárese, ya que sus conocimientos se convertirán en la base para la realización de esos nuevos proyectos. Procure pensar bien antes de realizar algún movimiento.')
	break
}
```
> se declara ```swtch ()``` y entre los paréntesis vamos a poner la varable que queremos utilizar

> La parte ```case``` signifca "caso" y hace referencia a que dependiendo que casos tengamos se hará tal cosa 

>Por ultmo hay que saber que el codigo segun sea el caso se va a ejecutar hasta que encuentre un ```break```

otro caso especial del switch es el ```default:``` que significa que si ninguna de las condiciones se cumple entonces se reproduce lo que se tenga preestablecido en default como