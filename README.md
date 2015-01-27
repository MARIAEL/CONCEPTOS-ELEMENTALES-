### IP  
 
**¿Qué es IP?**  

El protocolo de internet ( IP, Internet Protocol ) es un protocolo utilizado para la comunicación de datos a través de una red de paquetes combinados.  

**¿Qué es una dirección IP?** 
 
Es un número que identifica a una interfaz de cualquier dispositivo de red.

**IPS públicas / privadas**  

*Pública*:   
Una única IP que identifica nuestra red desde el exterior.  

*Privada*:   
Una IP que identifica a un dispositivo conectado en nuestra red interna. 
 
**Cómo ver mi IP privada** (del router hacia dentro)  
INICIO -- PANEL DE CONTROL -- REDES E INTERNET -- CENTRO DE REDES Y RECURSOS COMPARTIDOS -- CONEXION DE AREA LOCAL -- PROPIEDADES -- doble clic en PROTOCOLO DE INTERNET VERSION 4 (TCP/IPV4)  
  
**Cómo ver mi IP pública** (del router hacia fuera)   
Poner en el navegador de  internet *myip* o *miip* y nos dirá la IP pública del ordenador desde el que hacemos la consulta. (www.cual-es-mi-ip.net)


(Mi IP es 95.39.227.169) 

**IP estática / dinámica** 

*Dirección IP estática*


La dirección IP estática, como su propio nombre indica, permanece estática durante un determinado periodo de tiempo. Esto quiere decir que no se puede cambiar a menos que el usuario así lo decida.   
Las direcciones IP estáticas a menudo se emplean en redes protegidas, conexiones de redes privadas virtuales (VPN) y servidores web, entre otros usos.   
También pueden ser muy útiles cuando necesite realizar un reenvío de puertos en la red.

El equipo o dispositivo al que se le asigna tiene siempre la misma. Ya sea en Internet (IP fija pública) o en una red doméstica o empresarial (IP fija privada).


*Dirección IP dinámica*


Por otro lado, la dirección IP dinámica es aquella que cambia cada vez que el usuario se conecta a la red. Un ejemplo perfecto de una dirección IP dinámica es aquella que asigna el proveedor de servicios de Internet (ISP).  
Las IP de este tipo son variables. Un equipo o dispositivo puede tener una IP en un cierto momento y una distinta en otro.

No hay una norma fija sobre la frecuencia con que pueden cambiar. A veces se mantienen iguales durante mucho tiempo, mientras que otras cambian a menudo.

Muchos proveedores de Internet asignan IPs dinámicas a sus clientes. Si uno de ellos se desconecta de Internet -y ya "no necesita" su IP- el proveedor puede reutilizarla asignándosela a otro cliente que se conecte.

La "reutilización" de IPs optimiza recursos y abarata costos. Imagina a tu ISP como un hotel. Tiene un número limitado de habitaciones (IPs). Es mejor usar una misma habitación (una misma IP) para varios clientes que mantener la habitación cerrada (la IP sin usar) a la espera de que vuelva un cliente específico.

 



### ¿Qué es NAT? 

 La traducción de direcciones de red o NAT (del inglés Network Address Translation) es un mecanismo utilizado por routers IP para intercambiar paquetes entre dos redes que asignan mutuamente direcciones incompatibles.  
Consiste en convertir, en tiempo real, las direcciones utilizadas en los paquetes transportados.   
También es necesario editar los paquetes para permitir la operación de protocolos que incluyen información de direcciones dentro de la conversación del protocolo.  

Esta situación de varios dispositivos con una misma IP debe hacerse de forma ordenada para que funcione, por eso mismo el mecanismo que NAT provee es que “la red” se separe en dos (red privada y red pública) y el router NAT (cualquier router ADSL o WI FI lo es) en el medio, que se encarga de las traducciones de direcciones.

Un router NAT es, analogía mediante, el portero del edificio de la red.  

![](http://grabilla.com/05115-b5547413-9c57-4aac-94e5-ec3c879230e3.png)

  
El funcionamiento de un router NAT es mas o menos el siguiente:

1) Toda la gente (hosts) que viven en el edificio se encargan de hacer pedidos al exterior mediante él  

2) El NAT, que para la red interna es 10.0.0.2 pero le llaman así porque tienen confianza, se comunica con “internet” y le pregunta a Google lo que le transmitió 10.0.0.14, pero cuando lo hace, no se identifica como 10.0.0.2, ya que esta dirección es inválida en internet, sino que lo hace con su nombre y apellido, la IP Pública de la conexión (200.45.5.193 en el caso del gráfico)  

3) El Router NAT recuerda la respuesta, y luego se la envía a 10.0.0.14  

El router NAT (alias el portero del edificio) es nada más ni nada menos que un rápido traductor, que tiene 2 IP’s y dos formas de identificarse de acuerdo con quién se esté comunicando, también es el que se encarga de cambiar la IP en cada paquetito de acuerdo a qué IP interna se la haya pedido y mantiene una lista de cada request que haya sido realizado en la red interna, y como en todo edificio no puede faltar alguien que tiene la entrada libre, él mismo, mediante una configuración, puede dejar pasar personas sin identificación a un determinado departamento, lo que sería conocido como abrir un puerto para una IP.

TARJETA EFERNET  
