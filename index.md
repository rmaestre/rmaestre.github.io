# Introducci�n

Este peque�o manual est� pensado como introducci�n _pr�ctica y divertida_ a la toma y procesado de im�genes astron�micas en el contexto que se ha producido en nuestras sociedades a ra�z del impacto del coronavirus [#YoMeQuedoEnCasa](https://twitter.com/search?q=%23YoMeQuedoEnCasa&src=typed_query).

Son muchos los que me han inspirado a invertir tiempo y preparar los datos y materiales. Un buen ejemplo es el de [Javier Cansado](https://twitter.com/cansado2/status/1239894169365209088) y sus partidas online de juegos de mesa. Con este su enfoque en mente, pens� que tal vez, la gente pudiera hacer **astrofotograf�a sin salir de CASA** ! Es en realidad como trabajan los astr�nomos y astrof�sicos profesionales cuando realizan sus investigaciones, ya que se necesitan equipos muy precisos y con tecnolog�as avanzadas que son gestionados y mantenidos en centros espec�ficos.

Este peque�o tutorial est� pensado para tener un primer contacto con la astrofotograf�a desde casa, pero siempre teniendo en cuenta **que la parte mas divertida y donde mas se aprende es en el campo con tu telescopio (en mi opini�n!)**. A continuaci�n pongo algunos profesionales a los cuales admiro y de los cuales intento aprender: [Javier Mart�nez Mor�n](https://twitter.com/jmartinezmoran) o [�lvaro Ib��ez P�rez](https://twitter.com/kokehtz).

Un ejemplo de lo que se puede hacer, con este tutorial, es lo siguiente:

![M81](img/Integrated_cut_M81.jpg)

o

![NGC3324](img/NGC3324.jpg)




# Obtener Im�genes

Para obtener las im�genes tienes dos opciones:

- Irte al campo a un sitio muy oscuro, montar tu telescopio, alinearlo, ponerlo en estaci�n, acoplar tu c�mara DSLR o CCD, seleccionar un objetivo en el cielo y empezar a tomar las fotograf�as. Para tomar las fotograf�as hay que jugar con muchos par�metros como ISO, tiempo de exposici�n, ... Finalmente, cuando has tomado las fotograf�as, hay que tomar im�genes de calibraci�n que luego se usaran para procesar las im�genes.

- Usar usar un servicio remoto de telescopios profesionales (o semi-profesionales) como es el servicio de **[iTelescope.net](https://go.itelescope.net/)**. Con esta opci�n podras acceder a telescopios de todo el mundo (y por lo tanto a diferentes objetos) y, programar y ejecutar un plan para tomar im�genes de objetos de cielo profundo.

## iTelescope - Red de telescopios remoto

Con iTelescope podr�s acceder a diferentes telescopios ubicados en diferentes puntos de la tierra, como se muestra en la siguiente imagen. Es un mapa que muestra:

* Las estaciones con telescopios disponibles, como **puntos rojos**.
* El sol, con un **punto amarillo** y el �rea que ilumina.
* La luna, con su estado (luminosidad asociada).

![iTelescope-launchpad](img/networkit.jpg)

En cada una de las estaciones (puntos rojos del mapa anterior) existen diferentes telescopios que podemos usar para tomar nuestras fotograf�as. Para ver el listado, deberemos de acceder a la p�gina principal de _iTelescope_ y entrar en el *Launchpad*. 

![iTelescope-launchpad](img/launchpad.jpg)

Desde el Launchpad podremos ver el listados de las diferentes estaciones como por ejemplo _Chile_,_New Mexico_,_Siding Spring_,... En cada estaci�n, podremos ver los telescopios con su estatus: los que est�n siendo usados y porque usuarios, los que est�n disponibles y los que est�n off-line.

![iTelescope-launchpad](img/telescopios.jpg)

## Trabajar con un telescopio

Los telescopios de la red tienen como identificador una *T* seguido de un n�mero. Para entrar a alguno de ellos y operarlos remotamente hay que pulsar sobre los enlaces que se muestran en la figura anterior.


### 1. Planificar

Lo primero es, dada una estaci�n de trabajo, seleccionar que objetos y a que hora pueden observarse. Para ello, nos apoyaremos en otra excelente herramienta de planificaci�n. Desde [la p�gina principal (o Launhpad)](https://go.itelescope.net/) pulsaremos en el enlace "Start planning here".

![Start planning](img/start_planning.jpg)

lo que abrir� el siguiente men� donde elegiremos:

* **Site**: La estaci�n de telescopios donde est� el telescopio que vamos a operar. Es decir, desde donde vamos a tomar las im�genes.
* **Data**: La fecha para la que planificaremos la toma de im�genes
* **Objet** y *Types*: Criterios para  filtrar los diferentes tipos de objetos.

![Planner](img/planner.jpg)

Como ejemplo, yo he buscado que objetos se pueden observar el d�a *2020-03-18* desde la estaci�n de *New Mexico Skies*

![Planner example](img/planner_execution.jpg)

Aparece una lista con los objetos visibles desde la estaci�n de *New Mexico Skies* en el d�a elegido. Se lista el nombre del objeto, el tipo, su posici�n (RA,Dec), su maginutd, ... 

**Nota: Un dato muy importante es el de la visibilidad; es decir a que hora se empieza a ver, su hora de tr�nsito y a que hora se deja de ver.** Podemos ver estos datos en la columna visibilidad. Pulsando en el enlace de _Telescopius.com_ podremos obtener informaci�n ampliada sobre el objeto, y en concreto informaci�n sobre su visibilidad y tr�nsito. En este ejemplo, vemos que su mayor altitud es a las 6:34 pm, pero habr�a que esperar un poco para que se haga de noche y poder fotografiar el objeto.

![Visibility](img/visibility.jpg)


### 2. Acceder a un telescopio

Imaginemos, que hemos seleccionado la nebulosa brillante **NGC 1980** como objetivo de alg�n telescopio de la estaci�n de *New Mexico Skies* en la fecha seleccionada. El siguiente paso, es crear un plan en el telescopio. Para ello, entramos en el telescopio usando los enlaces de [la p�gina principal (o Launhpad)](https://go.itelescope.net/):

![iTelescope-launchpad-telescopios](img/telescopios.jpg)

Por ejemplo, entraremos en el telescopio [T11](http://t11.itelescope.net/index.asp#Welcome) y una vez introducido nuestro nombre de usuario y contrase�a, nos aparecer� la siguiente p�gina:

![iTelescope-launchpad-telescopios](img/t11.jpg)

### 3. Crear un plan

Ahora, pulsaremos el enlace ***Deep Sky* para crear un plan. Aparece la siguiente pantalla.

![Paso_1](img/plan_1.jpg)

Rellenaremos los campos, *Plan name* con el nombre del plan que queramos, y *Target (e.g. M51):* con el identificador del objeto que queramos fotografiar, en nuestro caso *NGC 1980*. Finalmente, pulsamos en el enlace de la derecha que pone **Get coordinates**, esto nos dir� si podemos observar el objeto desde la estaci�n y nos rellenar� autom�ticamente los campos de Ascensi�n recta y declinaci�n, como podemos ver en la siguiente imagen.

![Paso_2](img/plan_2.jpg)

Seguidamente, seleccionaremos los filtros para tomar las im�genes. En este caso tomar� cuatro im�genes con los filtros **L,R,G,B**. Dependiendo del telescopio, se pueden usar mas filtros como HA, por ejemplo. La exposici�n de cada imagen ser� de 160 segundos y repetir� la captura de estas im�genes 5 veces; por lo que tendr� en total 5*4=20 im�genes y un tiempo total de exposici�n de 5*4*160=3200 segundos (o 53.3 minutos).

![Paso_3](img/plan_3.jpg)

Una vez que tenemos todos los datos del objeto y de los filtros rellenos, procederemos a pulsar el enlace de abajo que pone **Create plan for later**. Esto crear� un plan en el telescopio que luego a�adiremos a un calendario para su ejecuci�n.

![Paso_4](img/plan_4.jpg)




### 4. Reservar

Ahora, solo queda reservar un slot en el telescopio para que se ejecute el plan que hemos dise�ado en el paso anterior. Para ellos, pulsaremos el enlace de **Make a reservation* del men� de la parte izquierda. Aparecer� un calendario como el de la siguiente imagen. En el, se marca en verde los espacios que ya han reservado los usuarios para ejecutar una planificaci�n. 


![Paso_5](img/plan_5.jpg)

Ahora tenemos que elegir un hueco libre (siempre teniendo en cuenta el tr�nsito del objeto y su visibilidad) y seleccionarlo pulsando con el rat�n en el calendario. Deberemos rellenar:

* **Start Time** y **End time**: el rango seleccionado para la ejecuci�n del plan
* **Plan to run**: seleccionando el nombre del plan que creamos en el paso anterior

cuando todo est� correctamente relleno, pulsaremos el bot�n *Confirm Reservation*.

![Paso_6](img/plan_6.jpg)

En este paso, aparecer� reservado nuestro espacio en el telescopio para ejecutar nuestro plan. Solo tenemos que esperar !

### 5. Esperar

Cuando falten dos horas para la ejecuci�n del plan, se recibe el siguiente correo:

![info mail](img/reservation_mail_info.jpg)

Seguidamente, pasadas las dos horas, se recibe el correo confirmando que ha entrado en ejecuci�n:

![info mail exe](img/![info mail](img/reservation_mail_info.jpg)

Y si todo ha ido bien, recibiremos un mail con toda la informaci�n de la ejecuci�n del plan:


![info mail exe](img/![info mail](img/reservation_mail_info_procesed.jpg)


### 6. Descargar las Im�genes

Una vez el plan se ejecute, nos llegar� al correo un resumen del estado de la ejecuci�n, n�mero de im�genes tomadas, visibilidad, etc, ... (correo de la imagen anterior) En ese momento, ya podemos ir al servidor ftp de iTelescope y descargar las im�genes: [Servidor de datos FTP ](https://data.itelescope.net/).

**Nota**: Una cosa interesante, es que podemos acceder a las im�genes ya calibradas. Pero si queremos las im�genes RAW, tendremos tambi�n disponibles las im�genes de calibraci�n bias, dark y flats.

Os pod�is saltar todos los anteriores pasos y descargar aqu� las im�genes de [M-81](http://bit.ly/2QAJ0kZ) y [NGC-3324](http://bit.ly/33zvvrb).


# Procesar Im�genes

En la siguiente publicaci�n ! 

