## HP50g Biblioteca para la asignatura Teoria de maquina / Sistemas mecanicos de la UNED

Esta es mi biblioteca personal que programe para la asignatura de "Sistemas mecanicos" publico su contenido por si a alguien le es de utilidad.

### Importante:

La biblioteca consiste de 4 programas mas adelante se explica su funcionamiento.

El programa de 4 barrras es el unico que no he desarrollado yo, credito al usuario Juange que lo publico (https://industrialesuned.es/index.php?topic=8370.msg154346#msg154346) el binario de este el foro (https://industrialesuned.es/index.php), la documentacion de la carpeta ./doc tambien es suya, de nuevo credito a su trabajo.

Dejo el el binario de la biblioteca y el editable, si encuentra algun fallo arreglelo, no me puedo comprometer a que los programas funcionen al gusto de todo el mundo.

### Directorios
./bin = binarios (el intalable esta aqui)
./doc = documentacion
./import = aqui hay una coipia del program utilizado para ovtener el codigo y el archivo origina importado
./origen = los binarios originales
./src = el archivo de biblioteca editable
./test = los codigos de zcalc, balan, volan, por separado para hacer prubas con el simulador


### Mini guia de funcionamiento
<ul>
    <li>**zcalc**: calcula la longitud de accion dos ruedas dentadas, el angulo en grados y las distancias todas en la misma unidad (el resultado sera en esta unidad), para el parametro "ex_0 in_1" si se introduce 1 es relacion interna si se introduce 0 es externa</li>
    <li>**balan**: calcula las posiciones y fuerzas para el equilibrio dinamico de un eje, el angulo en grados, la velocidad de rotacion en rad/s y las distancias todas en la misma unidad (el resultado sera en esta unidad)</li>
    <li>**volan**: calcula las energia de un volante de inercia, los parametros comunes son A el par de torsion Nm, w_2 la rotacion angular rad/s, k fluctuacion de velocidad en formato de porcentaje (de 0 a 1), despues para cada tramo de la rotacion completa se define segun la ecuacion K + A*B_x * sen(C_x*o2) esto es se define B, C y K, ademas de los rango en lo que son esos valores</li>
    <li>**barra**: seguir la guia original ./doc/Manual.pdf</li>
</ul>

### Como se obtuvo el codigo del programa de barras?
En la web (https://www.hpcalc.org/hp49/programming/libs/) se publico una utilidad (libEx 4.2, hay una copia en ./import/LE42.BIN) que permite obtener una codigo primitivo de una libreria instalada. De aqui se extrajo el archivo ./import/import.hpe el cual es editable. Con codigo primitivo se refiere a que es una version importada por lo que como se puede observar el archivo ./import/import.hpe no conserva la indentaciones, los intros y los comentarios originales, pero mantiene la funcionalidad y es editable. Por lo que se puede mantener a futuro, se ha hecho ya algo de limpieza.

Credito al usuario Peter F. Geelhoed. de la web anterio cullo perfil es (https://www.hpcalc.org/authors/112)

### Mini guia de programacion

### Mini guia de instalacion
1. Pasar la ultima version del binario a la tarjeta SD
2. En la calculadora acceder a "FILES" y copiar de la tarjeta SD el binario a la carpeta FLASH
3. Reiniciar la calculadora ON + F3
4. La biblioteca se habara intalado en la posicion L1101, se peude accder desde LIB tinme le nombre de "Bibli"





