# Notas-Node-

notas de curso

# Ciclo de eventos de node

Primero se crea una funcion `main()`, se registran las funciones de arriba hacia abajo (no se ejecutan), luego se saltan los bloques de las funciones y se continuá en las siguientes lineas de códigos, consta de una pila de procesos, un area de Node apis, y una cola de callbacks.

# Const vs Let vs var

- no utilizar variables var, siempre empezar con variables const y si se considera cambiar a let

- las variables const son más ligeras que let

# Template strings:

Es común el uso de backticks` (ctrl + alt + } `` )` para almacenar y concatenar strings incluso en varias lineas de código, siempre se devuelve un string

```javascript
const normal = nombre + ' ' + real;`
` const template = `${nombre} ${real}`;
```

ambas variables son iguales

# Desestructuración de objetos

La desestructuración de objetos puede ayudarnos para obtener datos de objetos, arreglos y variables en general de manera especifica, omitiendo datos que no necesitemos en el momento o incluso cambiandole el valor que se les tiene asignado al momento de la declaración.

```javascript
const deadpool = {
	nombre: 'Wade',
	apellido: 'Winston',
	poder: 'regeneracion',

	getNombre() {
		return `${this.nombre} ${this.apellido} ${this.poder}`;
	},
};

/* const nombre = deadpool.nombre;
const apellido = deadpool.apellido;
const poder = deadpool.poder; */

function imprimeHeroe({ nombre, apellido, poder, edad = 0 }) {
	console.log(nombre, apellido, poder, edad);
}

/* imprimeHeroe(deadpool); */

const heroes = ['Deadpool', 'Superman', 'Batman'];

/* const h1 = heroes[0];
const h2 = heroes[1];
const h3 = heroes[2]; */

const [, , h3] = heroes;

console.log(h3);
```
