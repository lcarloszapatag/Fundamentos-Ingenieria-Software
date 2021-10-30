## Idea básica al escribir y enviar un mail:

### Escribimos el mail XD
    
1-  Apretamos enter para enviar el mail.
2.  Al apretar enter estamos enviando una señal eléctrica desde el teclado
    - Esta señal es enviada a la motherboard, la motherboard la envia al CPU
    - La CPU recibe la señal del teclado y la envia al sistema operativo
    - El sistema operativo (a través de drivers, que son softwares
    que interpretan las señales eléctricas de los periféricos) interpreta la señal eléctrica y 
    la envía al navegador (pues sabe que nosotros queriamos enviarla ahí por donde apretamos el enter (mientras estabamos en el navegador)
   - . Nosotros cuando estamos en una pestaña de chrome en realidad estamos en un html, 
    un html posee uno o varios script, 
    y ahí un script que esta preparado para hacer algo al momento de pulsar la tecla enter
    (al momento que ocurra el evento “Pulsar tecla enter”),
    el cual va a hacer pues hemos apretado a tecla enter.
    
   - Javascript entiende que al ocurrir el evento enter tiene que hacer algo con el mail que hemos escrito.
   - AJAX permite enviar datos al servidor (el mail en este caso) y que la pagina no se recargue. 
    AJAX es un API (interfaz de programación), que, entre sus multiples funciones,
    encapsula los datos que deseamos enviar de una manera que luego el servidor comprendera.
    
   - La forma de encapsular los datos se denomina formato. AJAX encapsula el mail en un formato llamado JSON
   -  AJAX envía el mail en formato JSON a través del protocolo REST (es un conjunto de 
    reglas de como se envían los datos a un servidor) a través de HTTP (esta incluido en REST).
   -  HTTP y HTTPS son protocolos de transferencia de texto. HTTPS es más seguro porque
    permite que solo al servidor al cual estamos enviando los datos pueda interpretar la información, 
    solo el receptor final podrá ver los datos que enviamos.
    De esta manera se evita que alguien se pueda meter en el medio de al transferencia y ver los datos. 
    Los datos se envían a una dominio DNS, que es la dirección de un servidor
   - El servidor recibe los datos en forma de señales eléctricas, 
    el sistema operativo del servidor (en general linux(muerte al capitalismo 😛 )) a través de ethernet, 
    transforma los datos que están encapsulados según el protocolo TCP/IP. Este protocolo luego crea los datos hacia el protocolo HTTP,
    HTTP es recibido por un servidor de HTTP de linux.
   -El servidor HTTP ahora permite que los programas en el backend procesen la información recibida según corresponda.
    Los datos procesados son guardados en una base de datos para luego poder acceder a estos datos.
   - El mail ahora si es enviado al dominio que sigue al @.
   - El mail ahora va al servidor de mail del dominio que se envía, 
    este lo envía a la base de datos del mail que corresponde (el que esta previo al @), es decir va a la bandeja del receptor.
   - La bandeja del receptor recibe una notificación
   - La bandeja envía una notificación a un servidor de notificaciones, e
   -el servidor de notificación avisa a nuestro celular que se ha recibido un mail.
   -El mail fue envía y el receptor fue notificado a su celular.

Más claro échale agua 😛

NOTA: Los DNS es una base de datos que relaciona un nombre con un IP.
