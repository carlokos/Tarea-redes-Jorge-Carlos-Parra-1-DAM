# Jorge Carlos Parra Montoya | Tarea redes #
## Cosas a tener en cuenta ##
- Las IPs las he enumerado empezando desde "192.10.1" siendo el "10.1" el indicador de la tarea (la "20.2" sería la segunda tandas de redes" y así hasta que he llegar al "50.5" siendo la última tarea)
- He hecho el trabajo lo mejor posible, aún así no logro del todo el tema de redes y me temo que no esta del todo bien, agradecería que pudiese corregir este ejercicio en clases

## Primer ejercicio ## 
La primera parte consistia de hacer subredes de 100, 30 y 6 hosts. Para hacer una subred basta con modificar la mascara para lograr distintas redes del mismo tipo (ej: 255.255.255.0 pasa a 255.255.255.128 para lograr subredes con 6 hosts) el último número indica el número de host. Para saber cuantos hots permite la máscara basta con pasar el número a binario y contar los 0 en el octeto, y hacer 2^n para saber cuantas direcciones de hosts permite (ej: tenemos 224 que es 11100000; 2^5 = 32; 32-2 = 30 hosts diferentes).

A la hora de indicar la subred, podemos poner una barrita contando los 1 que usa la máscara (por ejemplo, en las subredes de 30 host la máscara tiene 27 1 y se usa /27 después de la IP para indicarlo.)

## Segundo ejercicio ##
Este ejercicio se trataba de hacer 8 ordenadores con IP dinámicas, para hacer el servidor tiene que proveer las IP. Hay que configurarlo para que de el rango de IP deseado y las DNS para que se pueda conectar a la página. Después los ordenadores, a poner las IPs en dinámicas, se configuran solos gracias al servidor

## Tercer ejercicio ##
Era igual que el segundo ejercicio, solo que estas vez son 4 ordenadores con IP dinámica. Hay que seguir el mismo proceso.

## Cuarto ejercicio ##
Aquí había que hacer 4 ordenadores con IP fija y conectar un punto de acceso para 5 ordenadores con IP dinámica. Para IP fija basta con configurar la IP de cada ordenador dentro del rango de IP deseado, además aquí hay que configurar también la DNS para que se puedan conectar a las páginas web de los servidores. 

Para los 5 ordenadores conectados a la IP dinámica podemos tratar al punto de acceso como un switch más y configurarlo para conectarlo al servidor (o en este caso al switch que esta conectado al servidor). También a los portatiles hay que ponerle fisicamente un punto de wifi para que se puedan conectar al punto de acceso. Al tener IP dinámica tenemos que configurar el punto de acceso para que se la brinde a los ordenadores.

## Quinto ejercicio ##
Consistia en hacer otros 5 ordenadores con IP fija, así que bastaba con configurar los ordenadores con el rango de IP adecuado 

Si hemos conectado bien todos los router, todas las redes están conectadas entre si y se podría acceder a las 3 páginas web desde cualquier ordenador (esto se logra gracias a las DNS y hay que configurarlo desde los servidores). Para que los routers estén bien conectados hay que añadirle puertos sata y conectarlos entre si, también yo he necesitado conectar puestos ethener para poder conectar todos los switch. Cada router tambien lleva una dirección IP que indica a que servidor esta conectado para poder pasale la información a los otros.
