# Cifrado Cesar

## Problema:
*Crea una web que pida, por medio de un prompt(), una frase al usuario y devuelva el mismo mensaje encriptado según el algoritmo de Cifrado César con el parámetro de desplazamiento de 33 espacios hacia la derecha.*

Por ejemplo:

+ Texto original: ABCDEFGHIJKLMNOPQRSTUVWXYZ
+ Texto codificado: HIJKLMNOPQRSTUVWXYZABCDEFG 

### Pseudocodigo
##### Esto comineza con un proceso, que preguntará al usuario *"¿Qué deseas hacer, cifrar 1 o descifrar 2?"*. Al ingresar los datos por medio del teclado, se epxresan las desiciones. 
Si es 1 se llamará a la función "cipher", por otro lado podría ser 2 donde correra la función "decipher".

La función cipher desarrolla la variable "sentence" la cuál preguntará por medio de un prompt * "¿Qué frase quieres cifrar?" *. Entonces se utilizará:

+ string.charCodeAt() con el que se obtendrá el código ASCII de la frase.
+ A través de la formula (x - 65 + 33 + 26)%26 + 65, se designará la posición de desplazamiento, según el problema debe ser 33.
+ Finalmente con String.fromCharCode() se pasará el número de la posición a letra.

##### Como se mencionaba anteriormente existe la posibilidad que el usuario quiciera decifrar. Esto se desarrolla con la variable position la que pregunta por medio de un prompt *"¿Qué frase quieres decifrar"*. Entonces:

+ Se aplica la formula (x - 33 + 26) % 26 para decifrar.
+ Luego la formula (x - 65 + 33)%26 + 65, aplicando el desplazamiento de la posición.
+ Luego string.charCodeAt () para saber el código ASCII.
+ String.fromCharCode() para pasar la posición a letra.


Finalmente se mencionará al usuario a través de un "alert" que no debe utilizar espacios en blanco o números.
 	 
 	 