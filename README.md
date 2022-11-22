# Notas-Node-

notas de curso

# Ciclo de eventos de node

Primero se crea una funcion `main()`, se registran las funciones de arriba hacia abajo (no se ejecutan), luego se saltan los bloques de las funciones y se continuá en las siguientes lineas de códigos, consta de una pila de procesos, un area de Node apis, y una cola de callbacks.

# Const vs Let vs var

- no utilizar variables var, siempre empezar con variables const y si se considera cambiar a let

- las variables const son más ligeras que let

# Template strings :tw-1f50c:

Es común el uso de backticks` (ctrl + alt + } `` )` para almacenar y concatenar strings incluso en varias lineas de código, siempre se devuelve un string

`const normal = nombre + ' ' + real;`
` const template = ``${nombre} ${real}``; `//solo es una backtick ``

ambas variables son iguales
