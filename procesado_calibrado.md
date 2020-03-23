


# Procesado - Calibrado

## 1. DynamicBackground (Extraction)

Usaremos la siguiente herramienta:

```
Process >> (All Processes) >> DynamicBackgroundExtraction
```

La primera acci�n, es definir puntos sobre el fondo en los sitios mas neutrales. Selecionaremos de forma autom�tica pulsando primero en la imagen y luego en el bot�n **sample**. La siguiente imagen muestra el resultado:

![pixinsight](img/pixinsight/DBE.jpg)

Una vez que esto puntos se han generado, pulsamos en **Target Image Correction** y seleccionamos: **Correction: Substraction**. Como resultado obtenemos  la imagen corregida con el modelo de fondo que ha sido calculado:


![pixinsight](img/pixinsight/DBE_output.jpg)

Descartamos el modelo de fondo, y volviendo a pulsar el bot�n de **Auto strech** de la herramienta **STF** podemos ver la imagen corregida. EN la figura que adjunto, muestro el antes y el despu�s de la correcci�n de los gradientes de luz:


![pixinsight](img/pixinsight/DBE_output_comp.jpg)



## 2. BackGroundNeutralization

Usaremos la herramienta:

```
Process >> (All Processes) >> BackGroundNeutralization
```

En este caso, seleccionaremos una preview como referencia donde solo tengamos fondo negro sin estrellas ni estructuras. Con esta imagen de referencia, esta herramienta balancea los canales RGB. Para ello seleccionamos una preview donde solo tengamos fondo negro.


![pixinsight](img/pixinsight/BN_preview.jpg)

Hay que situar la preview en fondo negro.

![pixinsight](img/pixinsight/BN_preview_black.jpg)

Una vez aplicada, tendremos balanceados los tres canales, como se muestra en la siguiente figura:

![pixinsight](img/pixinsight/BN_preview_applied.jpg)



## 3. ColorCalibration

Ahora procedemos a calibrar el color. Para ello usaremos la herramienta:

```
Process >> (All Processes) >> ColorCalibration
```

Necesitamos crear otra *preview*, en este caso de una zona luminosa. Seleccionaremos parte de la nebulosa. Adem�s, usaremos tambi�n la preview del fondo que usamos en el paso anterior.

![pixinsight](img/pixinsight/CC.jpg)


En este punto, ya hemos calibrado los canales. Revisamos que la mediana estad�stica de los tres canales se parezca. Para ello usamos la herramienta:

```
Process >> (All Processes) >> Statistics
```

Nos fijatemos que los tres canales tienen el mismo valor en la mediana. En este caso, el canal rojo tiene un poco m�s debido a la emisi�n en H-Alpha.

![pixinsight](img/pixinsight/statistics.jpg)


## 4. SCNR

Con esta herramienta, reducimos el sesgo del color. Tipicamente, cuando aparece verde es esp�reo y podemos atribuirlo a un error.  Para visualizar este problema, aumentaremos la saturaci�n de toda la imagen para ver estos borrones verdes. Usamos la herramienta:

```
Process >> (All Processes) >> CurvesTransformation
```
y modificando la saturaci�n de la imagen, podemos observar las zonas verdes.

![pixinsight](img/pixinsight/CurvesTransformation_preview.jpg)

Por lo tanto, si ahora aplicamos la herramienta SCNR con los valores por defecto:

```
Process >> (All Processes) >> SCRN
```


![pixinsight](img/pixinsight/scrn.jpg)

y volvemos a modificar los niveles de saturaci�n, observamos que ese verde ha desaparecido:



![pixinsight](img/pixinsight/scrn_ok.jpg)


