
## Software y configuración

### Requerimientos de Cableado:

- El cable **Din** de la primera barra LED debe conectarse a través de una resistencia de 470ohm al pin D4 del ESP8266.
- El  **GND** del ESP8266 y de los LED debe estar interconectado.
- El ESP8266 dispone de un pin llamado **Vin** que permite alimentar al ESP8266 sin necesidad de usar la toma USB. En ese caso es un conector de entrada. Pero cuando se conecta el USB este pin ofrece 5V de salida, siempre que no conectemos nada que supere una determinada intensidad. Según las fuentes leo que 500mA, otras que hasta 1000mA (1A). Asi que puede usarse para alimentar LED si no son muchos.
- A priori los LED deben tener un suministro propio de 5V ya que su amperaje puede superar con creces el que puede ofrecer el EP8266. Pero **el software WLED incluye una funcion muy interesante que permite limitar la corriente de salida**, asi que la ponemos a 500mA y nos garantizamos que la matriz LED puede funcionar. Esto nos permite conectar 5V a Vin y simplifica mucho la instalación.
 
La clave es saber si **es suficiente para que se desde Vin y con intensidad limitada los LED se pueden encender e iluminar bien. La respuesta es que si**, como podemos ver en la foto adjunta. Tanto es asi que podemos conectar a un banco de energía portátil y funcionará sin problema, haciendo el equipo completamente portable.

![Encendido con powerbank](encendidoconpowerbank.png)

### Carga del firmware

- Lo hacemos mediante el software WLED que podemos encontrar en su pagina oficial [**WLED**](https://kno.wled.ge/). Disponemos de tutoriales, comunidad y multitud de información que nos puede ayudar ajustar nuestro dispositivo.
- Dispone de varios procedimientos de instalación, el mejor es desde la web, lo tienes [**aquí.**](https://install.wled.me/) . Tendrás que tener el ESP8266 conectado por USB.
- Al conectar por cable desde el administrador de dispositivos (boton dcho en inicio, lo verás en el desplegable que se abre) verás que se activa un puerto COM, es en el que está conectado.
- En la web tenemos una opción para instalar, nos pedirá elegir el puerto, ponemos el que hemos visto activarse al conectar el ESP8266.
- Y ya casi está, la instalación es rápida y muy directa.
- OJO! Nos pedirá elegir una red Wifi para conectar, debemos poner la misma que usemos en el dispositivo desde el que conectamos. Normalmente será la doméstica. Pero yo me voy a eventos y para tener movilidad pongo mi móvil en modo punto de conexión, asi que aquí pongo el nombre de la red wifi que puedo asignar en mi movil. Si quieres usar en movilidad te recomiendo que hagas esto.

### Prueba de encendido

- Descargamos la app WLED para móvil, la tienes en la app store o google play.
- Nos aseguramos de que estamos en la misma red wifi.
- Al abrir la app pulsamos el boton **+** para buscar dispositivos compatibles.
- Nos avisará de que ha encontrado algo, salimos y veremos ahí el dispositivo con su num IP.
- Veremos que se encenderán en color ambar y muy suave unos cuantos LED, sobre 30. El SW está predeterminado asi , pero se puede cambiar. Para ello:
- Vamos a la pestaña de configuración y elegimos la opcion "LED preferences".
- Ahí dentro marcamos la casilla de limitacion de corriente, ponemos corriente máxima a 500mA, bajamos un poco y encontramos el num de LED que tenemos. Para Topotron V2 ponemos el valor 250. Subimos arriba y damos al botón "Save". Si todo ha ido bien veremos que se encienden todos los LED. A partir de ahi es jugar con la herramienta. Puedes seguir las instrucciones de la pagina web oficial y tambien hay videotutoriales en internet, casi todo en inglés.

### A partir de ahora?

Con el sw WLED se cumplen muchos de los requerimientos que buscaba en el proyecto, y se puede personalizar para llevarlo aun mas lejos. Pero hay algunas cosas que no son posibles y me gustaría que se puedan hacer. 

Por eso me propongo continuar con el proyecto y desarrollar un software propio, esto me llevara tiempo pq no es muy fuerte, pero estoy muy determinado asi que pasado un tiempo espero hacer actualizaciones al respecto.

Y si tienes alguna idea siempre puedes hacer algún **Pull Request**.

Seguimos!!







