
# Procesado - Apilado

Aunque existen otras herramientas gratuitas de procesado de im�genes astron�micas, nosotros usaremos [PixInsight](https://pixinsight.com/). Es probablemente el software mas completo y potente que existe en el mercado. Adem�s, dispone de un libro con gran detalle sobre sus herramientas, scripts y funcionalidades.

![pixinsight](img/pixinsight.jpg)

Un tutorial que explica en secuencia los pasos b�sicos para procesar una imagen puede encontrarse en este [v�deo tutorial](https://www.youtube.com/watch?v=_lqrXaJEs7g). Dado el enfoque de este art�culo, yo propongo unos pasos muy resumidos para conseguir un buen resultado en poco tiempo con el objetivo de pasarlo bien y hacer una peque�a iteracci�n sobre la herramienta con los datos que nos hemos bajado.


## 1. Abrir las im�genes

Lo primero de todo, ser�a abrir las im�genes (todos los archivos **.fit**).

![pixinsight](img/pixinsight/open.jpg)

A continuaci�n, usando la herramienta: 
```
Process >> (All Processes) >> Screen Transfer Function
```
visualizaremos cada una de las im�genes para buscar defectos o posibles errores.

![pixinsight](img/pixinsight/open_stf.jpg)

## 2. Alinear las im�genes

El fin �ltimo de alinear todas las im�genes, es poder combinar toda la informacion de los diferentes canales (R,G,B,L,Ha,...) que se han tomado en las diferentes exposiciones en una sola imagen maestra. Por lo tanto, lo siguiente que tenemos que hacer, es realizar un alineamiento de todas las im�genes; para ellos, usaremos la herramienta:

```
Process >> (All Processes) >> Star Aligment
```
Simplemente, en primer lugar seleccionaremos una imagen como referencia y en segundo lugar todas las dem�s para alinear.

![pixinsight](img/pixinsight/star_aligment.jpg)

Esto generar�, de nuevo todas las im�genes alineadas, como se aprecia en la salida del proceso:

![pixinsight](img/pixinsight/star_aligment_folder.jpg)


## 3. Integrar los datos de cada canal

Usando las im�genes que hemos alineado en el paso previo, usaremos la herramienta:

```
Process >> (All Processes) >> Image integration
```
![pixinsight](img/pixinsight/image_integration.jpg)

![pixinsight](img/pixinsight/image_integration_output.jpg)


para combinar las se�ales de cada canal y generar una �nica imagen por canal. En el ejemplo de la siguiente figura, integramos todas las im�genes del canal de Luminancia (L) obteniendo una sola imagen con todas la informaci�n combinada.

![pixinsight](img/pixinsight/image_integration_output_stf.jpg)

Repitiendo esto para los cuatro canales, obtenemos las siguientes im�genes master:

![pixinsight](img/pixinsight/LRGB.jpg)


## 4. Combinar canales previamente integrados (LRGB o RGB)

Ahora, podemos combinar las cuatro im�genes integradas previemante: L,G,R y B. Para ello usaremos la herramienta:

```
Process >> (All Processes) >> LRGB combination
```

Como resultado, obtenemos la imagen combinada a partir de los cuatro canales integrados.

![pixinsight](img/pixinsight/LRGB_output.jpg)

Si no tenemos el canal de Luminancia o solamente tenemos RGB, podr�amos usar la herramienta: 
```
Process >> (All Processes) >> Channel Combination
```