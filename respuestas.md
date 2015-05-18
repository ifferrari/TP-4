# RESPUESTAS #


1.  La primera expresión inicializa dichas variables `nl y nc en 0`. La coma es un operador binario, que  establece el orden de evaluación a la expresión, definiendo una susceptibilidad de evaluación de izquierda a derecha, a diferencia de la mayoría de los distintos operadores. 
Otra expresión equivalente existente puede ser la asociatividad de expresiones, en este caso sería: `nl=nc=0`. Esta expresión, genera una particularidad en la forma de evaluar expresiones, pudiendo realizar cambios en el sistema dándole mayor eficiencia, llamado efecto de lado.
1.  Los paréntesis puntúan la expresión y permite su evaluación. Si no son aplicados, no se podría evaluar la expresión, y en este caso, no se ejecutaría el `EOF`.
1.  La semántica en la primera etapa de la sentencia, evalua la expresión if e invoca a `FEOF` mediante stdin negándolo, pidiendo que su resultado sea distinto de 0. En la segunda etapa, Si dicho resultado es verdadero, pide invocar a `PERROR`, con el mensaje “"No se pudo seguir leyendo de la entrada debido a un error".
La pragmática de dicha sentencia es definir si la lectura del flujo finalizó con Error o no.
1. La función `PERROR` imprime un mensaje(argumento) de error  por stderror (salida estándar), permitiendo a un operador observar si hay error en el flujo de salida.
1. Puede ser reemplazada por: `ferror(stdin)`. La semántica de `feof` es que cuando se produce el fin del flujo de forma correcta devuelve verdadero. `ferror`, por el contrario, devuelve verdadero cuando el flujo termina con error. Las expresiones `!feof(stdin)` y `ferror(stdin)` no son mutuamente excluyentes ya que no indica el `EOF` hasta terminar de leer el flujo.
1. No corresponde respuesta.	
1. No corresponde respuesta.
1. El formato  `%.1f` establece la impresión de un float con precisión de 1 carácter.
1. Se explica un *casteo* para que la expresión se evalúe mediante un float y tenga mayor precisión el resultado.
1. No funciona correctamente para una entrada de flujo vacía.
1.  No es precisa ya que cuenta el dato `'\n'` en el ciclo y no considera la inicialización en 0 de las variables `nl y nc`.
1. Se debería imprimir la salida de valores de las variables` nl y nc` aumentadas en 1 luego de su inicialización en 0.
