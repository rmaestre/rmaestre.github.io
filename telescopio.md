


[Volver al inicio](https://rmaestre.github.io/ <<<)
<hr>

# Obtener Imágenes

Para obtener las imágenes tienes dos opciones:

- Irte al campo a un sitio muy oscuro, montar tu telescopio, alinearlo, ponerlo en estación, acoplar tu cámara DSLR o CCD, seleccionar un objetivo en el cielo y empezar a tomar las fotografías. Para tomar las fotografías hay que jugar con muchos parámetros como ISO, tiempo de exposición, ... Finalmente, cuando has tomado las fotografías, hay que tomar imágenes de calibración que luego se usaran para procesar las imágenes.

- Usar usar un servicio remoto de telescopios profesionales (o semi-profesionales) como es el servicio de **[iTelescope.net](https://go.itelescope.net/)**. Con esta opción podras acceder a telescopios de todo el mundo (y por lo tanto a diferentes objetos) y, programar y ejecutar un plan para tomar imágenes de objetos de cielo profundo.

## iTelescope - Red de telescopios remoto

Con iTelescope podrás acceder a diferentes telescopios ubicados en diferentes puntos de la tierra, como se muestra en la siguiente imagen. Es un mapa que muestra:

* Las estaciones con telescopios disponibles, como **puntos rojos**.
* El sol, con un **punto amarillo** y el área que ilumina.
* La luna, con su estado (luminosidad asociada).

![iTelescope-launchpad](img/networkit.jpg)

En cada una de las estaciones (puntos rojos del mapa anterior) existen diferentes telescopios que podemos usar para tomar nuestras fotografías. Para ver el listado, deberemos de acceder a la página principal de _iTelescope_ y entrar en el *Launchpad*. 

![iTelescope-launchpad](img/launchpad.jpg)

Desde el Launchpad podremos ver el listados de las diferentes estaciones como por ejemplo _Chile_,_New Mexico_,_Siding Spring_,... En cada estación, podremos ver los telescopios con su estatus: los que están siendo usados y porque usuarios, los que están disponibles y los que están off-line.

![iTelescope-launchpad](img/telescopios.jpg)

## Trabajar con un telescopio

Los telescopios de la red tienen como identificador una *T* seguido de un número. Para entrar a alguno de ellos y operarlos remotamente hay que pulsar sobre los enlaces que se muestran en la figura anterior.


### 1. Planificar

Lo primero es, dada una estación de trabajo, seleccionar que objetos y a que hora pueden observarse. Para ello, nos apoyaremos en otra excelente herramienta de planificación. Desde [la página principal (o Launhpad)](https://go.itelescope.net/) pulsaremos en el enlace "Start planning here".

![Start planning](img/start_planning.jpg)

lo que abrirá el siguiente menú donde elegiremos:

* **Site**: La estación de telescopios donde está el telescopio que vamos a operar. Es decir, desde donde vamos a tomar las imágenes.
* **Data**: La fecha para la que planificaremos la toma de imágenes
* **Objet** y *Types*: Criterios para  filtrar los diferentes tipos de objetos.

![Planner](img/planner.jpg)

Como ejemplo, yo he buscado que objetos se pueden observar el día *2020-03-18* desde la estación de *New Mexico Skies*

![Planner example](img/planner_execution.jpg)

Aparece una lista con los objetos visibles desde la estación de *New Mexico Skies* en el día elegido. Se lista el nombre del objeto, el tipo, su posición (RA,Dec), su maginutd, ... 

**Nota: Un dato muy importante es el de la visibilidad; es decir a que hora se empieza a ver, su hora de tránsito y a que hora se deja de ver.** Podemos ver estos datos en la columna visibilidad. Pulsando en el enlace de _Telescopius.com_ podremos obtener información ampliada sobre el objeto, y en concreto información sobre su visibilidad y tránsito. En este ejemplo, vemos que su mayor altitud es a las 6:34 pm, pero habría que esperar un poco para que se haga de noche y poder fotografiar el objeto.

![Visibility](img/visibility.jpg)


### 2. Acceder a un telescopio

Imaginemos, que hemos seleccionado la nebulosa brillante **NGC 1980** como objetivo de algún telescopio de la estación de *New Mexico Skies* en la fecha seleccionada. El siguiente paso, es crear un plan en el telescopio. Para ello, entramos en el telescopio usando los enlaces de [la página principal (o Launhpad)](https://go.itelescope.net/):

![iTelescope-launchpad-telescopios](img/telescopios.jpg)

Por ejemplo, entraremos en el telescopio [T11](http://t11.itelescope.net/index.asp#Welcome) y una vez introducido nuestro nombre de usuario y contraseña, nos aparecerá la siguiente página:

![iTelescope-launchpad-telescopios](img/t11.jpg)

### 3. Crear un plan

Ahora, pulsaremos el enlace **Deep Sky** para crear un plan. Aparece la siguiente pantalla.

![Paso_1](img/plan_1.jpg)

Rellenaremos los campos, *Plan name* con el nombre del plan que queramos, y *Target (e.g. M51):* con el identificador del objeto que queramos fotografiar, en nuestro caso *NGC 1980*. Finalmente, pulsamos en el enlace de la derecha que pone **Get coordinates**, esto nos dirá si podemos observar el objeto desde la estación y nos rellenará automáticamente los campos de Ascensión recta y declinación, como podemos ver en la siguiente imagen.

![Paso_2](img/plan_2.jpg)

Seguidamente, seleccionaremos los filtros para tomar las imágenes. En este caso tomaré cuatro imágenes con los filtros **L,R,G,B**. Dependiendo del telescopio, se pueden usar mas filtros como HA, por ejemplo. La exposición de cada imagen será de 160 segundos y repetiré la captura de estas imágenes 5 veces; por lo que tendré en total 5*4=20 imágenes y un tiempo total de exposición de 5*4*160=3200 segundos (o 53.3 minutos).

![Paso_3](img/plan_3.jpg)

Una vez que tenemos todos los datos del objeto y de los filtros rellenos, procederemos a pulsar el enlace de abajo que pone **Create plan for later**. Esto creará un plan en el telescopio que luego añadiremos a un calendario para su ejecución.

![Paso_4](img/plan_4.jpg)




### 4. Reservar

Ahora, solo queda reservar un slot en el telescopio para que se ejecute el plan que hemos diseñado en el paso anterior. Para ellos, pulsaremos el enlace de **Make a reservation** del menú de la parte izquierda. Aparecerá un calendario como el de la siguiente imagen. En el, se marca en verde los espacios que ya han reservado los usuarios para ejecutar una planificación. 


![Paso_5](img/plan_5.jpg)

Ahora tenemos que elegir un hueco libre (siempre teniendo en cuenta el tránsito del objeto y su visibilidad) y seleccionarlo pulsando con el ratón en el calendario. Deberemos rellenar:

* **Start Time** y **End time**: el rango seleccionado para la ejecución del plan
* **Plan to run**: seleccionando el nombre del plan que creamos en el paso anterior

cuando todo esté correctamente relleno, pulsaremos el botón *Confirm Reservation*.

![Paso_6](img/plan_6.jpg)

En este paso, aparecerá reservado nuestro espacio en el telescopio para ejecutar nuestro plan. Solo tenemos que esperar !

### 5. Esperar

Un unas horas, si todo ha ido bien, se recibe el siguiente correo:

![info mail](img/reservation_mail_info.jpg)

Seguidamente, pasadas las dos horas, se recibe el correo confirmando que ha entrado en ejecución:

![info mail exe](img/reservation_mail_info_launch.jpg)

Y si todo ha ido bien, recibiremos un mail con toda la información de la ejecución del plan:


![info mail exe](img/reservation_mail_info_procesed.jpg)

<hr>

[Volver al inicio](https://rmaestre.github.io/ <<<)

