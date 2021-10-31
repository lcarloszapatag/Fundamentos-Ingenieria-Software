Los routers son las puertas enlace a diferentes redes.
El router asigna IPs dentro de la red local y
esa IP es única en esa red, 
hacia afuera todos los equipos se conectan con la IP que te da el proveedor de internet que tienes contratado.

Para asignar IPs un software se encarga de revisar la Mac address de cada dispositivo y asignarle una IP que esté disponible.
‘
En los esquemas de red se crea un red virtual dentro de los sistemas operativos con un concepto interno que se le conoce como los puertos.
Un puerto es una puerta especifica para un programa específico.
cada solicitud que tu haces desde tu pc a traves de una red trabaja con una ip y un puerto amigo,
los puertos sirven para identificar los miles de servicios que maneja un SO,
ejemplo: cuando tu entras a twitter desde tu navegador tu estas haciendo una peticion a (102.102.20.02, ejemplo de ip de twitter),
y el puerto 80 pero si quisieras subir un archivo por protocolo ftp seria 102.102.20.02 por puerto 21
que se ve reflejado como 102.102.20.02:21 y así sucesivamente cambia el puerto dependiendo del servicio.
’
“Los protocolos son como un lenguaje de comunicación entre máquinas y 
los puertos son autopistas donde los mensajes del protocolo pueden transitar”.

La cantidad total de puertos disponibles es 65,535 gracias a que internamente hay dos bytes disponibles para definir la cantidad de puertos que existen.
Explicación del por qué tenemos 65, 535 puertos disponibles:
un byte son 8 bits si tu tienes el valor 11111111 es igual a 255 por consiguiente dos bytes puede ser 256 (si incluimos el 0) por 256
256 * 256 = 65.536
Ahora restamos 1 por el puerto 0, porque no es valido y obtenemos los 65.535

El sistema operativo tiene reservado los puertos del 1 al 1024, para usarlos necesitas elevar los privilegios de usuario.
