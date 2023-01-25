(thecontacts)=
# **7**. __Segunda fotolitografía__: CONTACTOS DEL SENSOR
Se repetirán los procesos de limpieza y recubrimiento explicados en la sección anterior. Sin embargo, se deberán tomar en consideración dos particularidades: por un lado, con el fin de evitar el deterioro de las estructuras pertenecientes al sensor, se reducirá el tiempo del baño de ultrasonidos a aproximadamente 20 segundos. Por otro, debido a la simetría del vidrio, existe el riesgo de confundir ambas superficies, luego es recomendable dibujar una muesca con punta de diamante en una esquina como marca de identificación.

## **7.1** ___Alignment mode___: alineación de capas

```{figure} alignment.PNG
---
height: 100px
name: alignment
---
Se fijarán las posiciones $\mathbf{r}_{0}$ y $\mathbf{r}_{1}$ en cada uno de los elementos del sensor mediante la correcta alineación de las cruces de la figura [5](descrosses). Así, posteriormente se depositará el material de los contactos en el área adecuada.
```
La figura [25](alignment) esquematiza el proceso de creación de los contactos. Antes de nada, se transferirá la máscara perteneciente a los contactos al programa de la máquina.

```{figure} contactsslicinggrid.PNG
---
height: 400px
name: stitchcontacts
---
_Stitching mode_ de la segunda capa. Ver las explicaciones de la figura [15](stitch).
```

```{figure} cross1alignment.PNG
---
height: 500px
name: stitchcontacts
---
Pasos del _Semi-automatic alignment mode_: __1.__ Calibrar la cámara ;  __2.__ Escoger el punto del sustrato a vista de cámara ($P_{1}^\prime$: centro de la cruz 1) ;  __3.__ Escoger el punto a alinear con $P_{1}^\prime$ a vista del dibujo ($P_{1}$: centro de la cruz 1 de la segunda capa). ;  __4.__ (Paso opcional) Escoger otro punto del dibujo ($P_{2}$: centro de la cruz 2 del dibujo) ;  __5.__ Verificar el alineamiento.
```
A continuación, se procederá al __alineamiento entre capas__. Primeramente, se activará el microscopio de la máquina (_Microscope Mode_). Así, haciendo mover el soporte, se hallarán las cruces de la exposición número 1 con el permalloy depositado para comenzar con el alineamiento. En la figura \ref{almode} se explica el proceso del alineamiento en modo semi-automático. Este paso requiere gran minuciosidad debido a las limitaciones de la cámara de la máquina. Al aumentar la imagen, ésta pierde calidad, por lo que resulta complicado acertar en el centro de las cruces de alineación. Además, la distancia de superposición entre sensor y contacto es de tan solo $2 \; \mu\text{m}$, por lo que un ínfimo desvío acarrearía un alineamiento inadecuado, tanto en horizontal como en vertical (obsérvese con detenimiento la figura \ref{contacts1.8s}).

## **7.2** __Exposición nº 2__

Habido configurado el alineamiento, se realizará la __exposición de la segunda capa__. Se deberán seguir los pasos de la sección anterior para ajustar la dosis de exposición de los contactos.

> __Número de columnas y filas__: $3 \times 1$

> __Distancia horizontal entre exposiciones__: $\Delta x = 2,5 \; \text{mm}$

> __Tiempo inicial__: $1 \; \text{s}$

> __Aumento de tiempo__: $0,4 \; \text{s}$

Así, los tiempos de exposición serán los siguientes:

$$
1 \; \mathrm{s} \; \rightarrow \; 1,4 \; \mathrm{s} \; \rightarrow \; 1,8 \; \mathrm{s} \;.
$$


```{admonition} Nota
En exposiciones posteriores se ha variado ligeramente la dosis del tiempo. Por otro lado, al hilo de lo mencionado previamente, en sesiones posteriores se requerirán dosis mayores.
```
Tras la exposición, se dará paso al __revelado__ y al análisis de los resultados.

```{figure} contactsbad1.PNG
---
height: 200px
name: cbad1
---
$t_{\text{exp}}=1,1 \;\text{s}$ y $t_{\text{rev}}=60 \;\text{s}$. El grado de revelado es muy bajo. El sensor no fue correctamente depositado previamente.
```

```{figure} contacts12.PNG
---
height: 200px
name: cbad2
---
$t_{\text{exp}}=1,4 \;\text{s}$ y $t_{\text{rev}}=60 \;\text{s}$. El resultado ha mejorado. No se aprecia el sensor.
```
```{figure} contactsgood.PNG
---
height: 200px
name: cgood1
---
$t_{\text{exp}}=1,8 \;\text{s}$ y $t_{\text{rev}}=60 \;\text{s}$. Contactos limpios con bordes bien definidos. La alineación entre sensor y contactos no es aceptable, pues apenas se aprecia contacto entre ambos elementos.
```
```{figure} contactsgooDD.PNG
---
height: 200px
name: cgood2
---
$t_{\text{exp}}=1,9 \;\text{s}$ y $t_{\text{rev}}=60 \;\text{s}$. Contactos limpios con bordes bien definidos. La alineación entre ambas capas es aceptable.
```
De las figuras [28](cbad1)-[31](cgood2) se concluye que las __dosis adecuadas__ de __exposición__ y de __revelado__ para la __segunda fotolitografía__ son las siguientes:

$$
\boxed{t_{\text{exp}} \approx 1,9 \; \mathrm{s} \; ; \; t_{\text{rev}} = 60 \; \mathrm{s}} \; .
$$

Se llevarán a cabo dos procesos de _sputtering_, teniendo en cuenta el procedimiento explicado previamente. Sin embargo, esta vez no será necesario definir la imanación del material, luego se empleará un soporte convencional para el sustrato.

Primero, se depositará una capa de 8 nm de __titanio__, puesto que la adhesión del oro al vidrio es débil. Seguidamente, se creará la capa de __oro__ de 100 nm perteneciente a  los contactos. Los respectivos parámetros se recogen en la tabla [3](paramau).

```{list-table} Parámetros de _sputtering_ de Ti (primera fila) y Au (segunda fila).
:header-rows: 1
:name: paramau

* - $\text{Flujo}_{\text{Ar}} \; (\text{sccm})$
  - $p_{\text{Ar}} \; (\mu\text{bar})$
  - $P \; (\text{W})$
  - $\Delta V \; (\text{V})$
  - $I \; (\text{A})$
  - $\text{Esp.} \; (\text{nm})$
  - $t_{\text{pre}} \; (\text{min})$
  - $t_{\text{sp}} \; (\text{min})$
* - $11$
  - $2,5$
  - $70$
  - $384$
  - $0,18$
  - $8$
  - $6$
  - $40$
* - $11$
  - $2,5$
  - $70$
  - $369$
  - $0,19$
  - $100$
  - $2$
  - $2$
```

La figura [32](aulayer) muestra el resultado después de la deposición.

```{figure} sput_au.PNG
---
height: 300px
name: aulayer
---
Deposición de oro en el sustrato.
```
Mediante el posterior paso de _lift off_ se eliminará la película de oro, creando de esta forma los contactos.

## **7.3** __Resultados tras la segunda deposición__

En las siguientes figuras se recogen dos muestras de cruces y sus pertenecientes sensores y contactos.


```{figure} crossesgold.PNG
---
height: 300px
name: crossesgold
---
__Muestra 1__. El alineamiento entre la primera capa de Py y la segunda de oro es adecuado.
```

```{figure} crossesaualignbad.PNG
---
height: 300px
name: crossesgoldbadal
---
__Muestra 2__. El alineamiento entre ambas capas no es del todo acertado. De hecho, en la cruz 2 se puede observar un ligero desvío en el eje horizontal. Estos resultados son indicadores del hecho de que se ha trabajado al límite de la resolución de la máquina.
```
```{figure} layer12badal.PNG
---
height: 200px
name: contactssensors1
---
__Muestra 1__. Deposición de oro en los contactos pertenecientes a las cruces de la figura [33](crossesgold). Se puede apreciar un desplazamiento inesperado en horizontal entre sensores y contactos.
```

```{figure} layer12goodal.PNG
---
height: 200px
name: contactssensors2
---
__Muestra 2__. Deposición de oro en los contactos pertenecientes a la cruz de la figura [34](crossesgoldbadal). En este caso, lo que cabe destacar es la excelente alineación entre sensores y contactos.
```

Considerando comentarios de las figuras [33](crossesgold) - [36](contactssensors2), es evidente que la alineación entre las cruces no coincide con aquélla entre sensores y contactos. Este factor se puede deber a pequeñas derivas en el ajuste de la posición del soporte del equipo de fotolitografía mientras dura la exposición. De hecho, atendiendo a la figura [26](stitchcontacts), el soporte realiza seis cambios de coordenadas. Un pequeño desvío de incluso $0,5 \; \mu\text{m}$ puede acarrear resultados como el de la figura [35](contactssensors1). Debido a ello, convendría ajustar el control del motor que hace mover el soporte.

De todos modos, en la mayoría de las sesiones finalmente se ha logrado alinear las dos capas de tal forma que la corriente pueda ser transmitida de los contactos al sensor. Por lo tanto, se han cumplido los objetivos propuestos inicialmente.

Habiendo ajustado y optimizado los procesos de exposición de ambas capas, se preparará un sustrato adicional con dos muestras para llevar a cabo mediciones de magnetorresistencia. Sin embargo, previamente será necesario añadir una tercera capa de contactos exteriores.
