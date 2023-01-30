(thesensors)=
# **6**. __Primera fotolitografía__: SENSOR

En esta sección, se explicará el primer proceso de fotolitografía, mediante la cual se reproducirán los patrones de la figura [3](dessensors) en un sustrato de __vidrio__, de las siguientes dimensiones: $(24 \times 40 \times 0,15) \; \mathrm{mm}$.

(clean1)=
## **6.1** Limpieza del sustrato

Primeramente, el sustrato se debe limpiar, para eliminar posibles contaminantes y agentes orgánicos. De esta forma, se propiciará la adhesión de la resina. Para comenzar, el sustrato será sometido a un __baño de acetona__ que eliminará contaminantes orgánicos. Se debe verter la suficiente cantidad al recipiente correspondiente, de tal manera que el vidrio quede completamente sumergido. El recipiente se colocará en la máquina de ultrasonidos (figura [11](aceultra)), y se mantendrá ahí durante dos minutos. Una vez que haya transcurrido ese tiempo, el sustrato se sacará del envase, sosteniéndolo cuidadosamente con las pinzas por un extremo. Con la pistola de nitrógeno se aplicarán ráfagas discontinuas con una pequeña inclinación respecto a su plano paralelo, para así eliminar los restos de acetona. Las pinzas también deben quedar limpias.

```{admonition} Nota
Esta máquina contiene un generador de ondas de sonido de altas frecuencias. La diferencia entre las presiones de los máximos y mínimos de estas ondas de compresión produce burbujas en el líquido, las cuales fomentan la remoción de contaminantes y partículas {cite}`ultrasonic`.
```
```{figure} aceultrasonidos.jpg
---
height: 250px
name: aceultra
---
El recipiente de acetona con el sustrato en el baño de ultrasonidos.
```

Después, se procederá al __baño de isopropanol__ para eliminar los residuos de acetona, en el cual se deberán seguir los pasos explicados anteriormente.

(clean1)=
## **6.2** _Spin coating_: deposición de resina

Al finalizar la limpieza, el sustrato se colocará bien centrado en la centrifugadora, también denominada _spinner_, donde quedará sujeta mediante vacío (Figura [12](spinner)). Primero, se cubrirá gran parte de su superficie ($\approx 80\%$) con un __promotor de adherencia__ que consiste en una solución de HMDS (_hexametildisilazano_) {cite}`adhesion`, el cual fortalecerá la resistencia de la adhesión de la resina al vidrio. Por otro lado, cabe mencionar que una humedad muy elevada ($>60\%$) puede debilitar la adhesión considerablemente.

```{figure} obleaspinner.jpg
---
height: 250px
name: spinner
---
El vidrio queda sujeto al soporte del _spinner_ mediante vacío. También recibe un flujo de aire comprimido ($\text{N}_2$) para reducir la humedad. Éstos son esenciales para la inicialización y el desarrollo completo de los programas de centrifugado.
```

El usuario cerrará la cubierta y se asegurará de que el vacío se está realizando adecuadamente (la pantalla no debe parpadear). Después, seleccionará el programa E, por lo que el sustrato girará a $4000 \; \text{rpm}$ durante $30  \; \text{s}$. Es importante percatarse de que dicho programa consiste de siete fases en total: tres de aceleración, la principal y tres de deceleración. Es decir, la velocidad aumenta y decrece progresivamente (figura [13](spgraph)). Así, se creará una capa de aproximadamente $15 \; \mathrm{nm}$ de espesor. Cuando el HMDS se haya distribuido uniformemente, se depositará la __resina fotosensible__ (con otra pipeta). El _photoresist_ que se emplea es positivo {cite}`resist`. Es conveniente almacenar el bote seguidamente tras su uso, para así evitar el deterioro de la resina debido a la humedad y otros factores. En este caso se seleccionará programa S, el cual hará girar al sustrato a $4000 \; \text{rpm}$ durante $60  \; \text{s}$, adquiriendo de esta forma un espesor de $1 \; \mathrm{μm}$, según la hoja de especificaciones.

```{figure} spinnergraph.PNG
---
height: 300px
name: spgraph
---
Fases de aceleración, principal y deceleración del programa S del spinner, empleado en la deposición de la resina.
```

(exp1)=
## **6.3** Exposición nº 1

A continuación, el sustrato se posicionará en el soporte de la máquina. Se debe procurar que los bordes queden bien alineados (figura [14](soporte)). Hecho esto, los pasos subsiguientes se llevarán a cabo mediante el programa _SFTPrint_. La máscara del sensor se transferirá siguiendo el formato de _stitching_ (figura [15](stitch)), con el objeto de aumentar la resolución.
En la pantalla principal (sección $(i)$ de la figura [7](smartgen)) se seleccionará el objetivo de mayor aumento ($\times 10$) y sustrato de vidrio. Cabe destacar que las dimensiones del sensor a fabricar se encuentran en el límite de la resolución de la cámara $(2\; \mathrm{μm})$.

```{figure} objective.jpg
---
height: 250px
name: soporte
---
El sustrato en el soporte, debajo del objetivo.
```

```{figure} sensorsslicinggrid.PNG
---
height: 400px
name: stitch
---
_Stitching Mode_ de la primera capa. El diseño del sensor se repartirá en seis celdas. De esta forma, la exposición se realizará en seis pasos, siguiendo las flechas rojas.
```
Tras finalizar la configuración inicial, se procederá a la selección de la zona de interés (figura [16](focusdraw)). Ésta no ha de quedar muy cerca de los bordes, dado que existiría el riesgo de dañar los diseños al sujetar el vidrio con las pinzas.

```{figure} focus.PNG
---
height: 200px
name: focusdraw
---
Puntos de enfoque en el sustrato.
```

Como se va a llevar a cabo un test de dosis, se realizarán varias exposiciones, una tras otra. Por ello, el área escogida deberá ser lo suficientemente extensa. Después, se corregirá el __enfoque__. Este paso es vital, pues de ello depende en gran medida que la imagen sea transferida nítidamente al sustrato. Además, como se ha mencionado previamente, las dimensiones del borde corto de cada componente del sensor coinciden con el límite de la resolución de la cámara de la máquina. Por ende, se deberá prestar especial atención a este paso.
Al pulsar en _FOCUS MODE_ (sección $(ii)$ de la figura [7](smartgen)), en la pantalla de la cámara aparecerá una red con letras y números. Se guardarán las coordenadas del punto $P_{1}$, y en él se ajustará la posición del eje $z$, haciendo mover verticalmente el motor del soporte mediante las flechas. Seguidamente, moviendo el soporte en horizontal, se fijará el punto $P_{2}$, ajustando en él el eje $x$ manualmente. Este proceso se repetirá varias veces, hasta asegurarse de que el enfoque es correcto en la totalidad de la zona (figura [17](goodfocus)b).


```{figure} goodbadfocus.PNG
---
height: 400px
name: goodfocus
---
Red de enfoque a vista de cámara.
```

Una vez arreglado el enfoque, se procederá a la propia exposición. Mediante la opción _dose test_, se __determinará la dosis__ adecuada; es decir, el tiempo óptimo de exposición para garantizar la correcta transferencia de los patrones a la resina. Para ello, se fijará el soporte en el punto $P_{1}$, y se especificarán los siguientes puntos (ver figura [9](dose)):

> __Número de columnas y filas__: $3 \times 1$

> __Distancia horizontal entre exposiciones__: $\Delta x = 2,5 \; \text{mm}$

> __Tiempo inicial__: $1,5 \; \text{s}$

> __Aumento de tiempo__: $0,6 \; \text{s}$

Observando las especificaciones introducidas, se efectuarán tres exposiciones en horizontal. Como la imagen entera de la figura [5](descrosses) ocupa una longitud de $2,1 \; \text{mm}$, se dejará un espacio de $2,5 \; \text{mm}$ entre exposiciones. Los tiempos de exposición serán los siguientes:

$$1,5 \; \mathrm{s} \; \rightarrow \; 2,1 \; \mathrm{s} \; \rightarrow \; 2,7 \; \mathrm{s} \;.$$

```{admonition} Nota
 Los datos corresponden a la sesión del 28 de febrero de 2022. En sesiones posteriores se han requerido mayores tiempos de exposición para obtener resultados deseables. Ver sección [10](problems).
```

Antes de comenzar, el usuario deberá colocarse las gafas protectoras, y no deberá quitárselas hasta la culminación del proceso. Además, deberá retirar el filtro protector de luz azul de la máquina. Mientras dura la exposición, observará los resultados a vista de cámara en la pantalla del programa. Al finalizar, volverá a colocar el filtro.

(rev1)=
## **6.4** Revelado y análisis de los resultados

Se procederá al último paso en la sala blanca. En el recipiente correspondiente, se preparará la solución de revelado, mediante el revelador AR 300-35 {cite}`developer` y agua desionizada, siguiendo la proporción $2:1$; es decir, dos partes de agua $(50 \; \text{ml})$ por cada una de revelador $(25 \; \text{ml})$. El sustrato se mantendrá sumergido durante $90 \; \text{s}$. Se le aplicarán movimientos transversales, con el objeto de propiciar la penetración del revelador en la resina. Al transcurrir el periodo de tiempo, el sustrato se meterá en agua para detener la reacción. Después, se verterá agua en abundancia en la superficie incidida, para así eliminar el revelador residual. Tras eliminar los restos con $\text{N}_{2}$, se observarán los resultados por medio del microscopio de la alineadora (figura [18](crossesexp)).

```{figure} res1.PNG
---
height: 250px
name: crossesexp
---
Cruz nº 2 de alineación tras la primera exposición.
```

```{admonition} Nota
 No se han incluido imágenes correspondientes a los patrones del sensor tras el revelado, debido a su reducido tamaño. La cámara de la alineadora de la sala blanca (figura [2](cleanroom)(d)) no permite tomar fotos con la suficiente resolución y calidad.
```

En figura [18](crossesexp)a se puede apreciar claramente que la resina expuesta por la luz ultravioleta no ha sido adecuadamente disuelta y extraída por el revelador, puesto que su interior muestra una tonalidad muy oscura, la cual va disminuyendo en las figuras adyacentes. Esto no es aceptable, pues impediría la correcta deposición del material. Solamente deben quedar marcados los bordes de los patrones. El fenómeno mencionado se puede deber a varios factores:

_Un recocido insuficiente_
: Este factor se descarta, puesto que otras cruces del mismo sustrato han salido claramente definidas.

_Tiempo insuficiente de revelado_
: En otros sustratos con $t_{\text{rev}}=30 \; \text{s}$  y $60 \; \text{s}$, la resina no ha sido debidamente disuelta. Se ha concluido que el tiempo adecuado es de $90 \; \mathrm{s}$.

Tiempo insuficiente de exposición
: En este caso, éste es el factor causante. El tiempo de revelado es el adecuado: 90 s. Además, se puede observar claramente que, a medida que $t_{\mathrm{exp}}$ aumenta, la tonalidad oscura disminuye considerablemente.

Teniendo en cuenta que el único resultado permisible es el de la figura [18](crossesexp)(c), se concluye que las __dosis adecuadas__ de __exposición__ y de __revelado__ para la __primera fotolitografía__ son las siguientes:

$$\boxed{t_{\text{exp}} = 2,7 \; \mathrm{s} \; ; \; t_{\text{rev}} = 90 \; \mathrm{s}} \; .$$

En sesiones subsiguientes, se prepararon dos muestras con la dosis adecuada para así proceder a la deposición del permalloy.

(rev1)=
## **6.5** _Sputtering_ de permalloy y _lift off_

La técnica denominada _sputtering_ es ampliamente empleada para la creación de películas delgadas {cite}`edu, sputtering`.

```{figure} sputtering_scheme.PNG
---
height: 400px
name: sput
---
Proceso esquematizado del _sputtering_ magnetrón. Los iones de argón impactan contra el blanco de permalloy, extrayendo átomos y creando así una fina capa en el sustrato. El campo magnético aplicado confina los iones a la región del blanco, lo cual incrementa el número de colisiones, reduciendo el tiempo de deposición.
```

```{list-table} Parámetros de _sputtering_ de permalloy
:header-rows: 1
:name: parampy

* - $\text{Flujo}_{\text{Ar}} \; (\text{sccm})$
  - $p_{\text{Ar}} \; (\mu\text{bar})$
  - $P \; (\text{W})$
  - $\Delta V \; (\text{V})$
  - $I \; (\text{A})$
  - $\text{Esp.} \; (\text{nm})$
  - $t_{\text{pre}} \; (\text{min})$
  - $t_{\text{sp}} \; (\text{min})$
* - $11$
  - $2,8$
  - $110$
  - $396$
  - $0,27$
  - $100$
  - $3$
  - $6$
```

El esquema del proceso de deposición ha sido representado en la figura [19](sput). En la tabla [2](parampy) se han recogido los siguientes valores: flujo y presión del argón $(\text{Flujo} _ {\text{Ar}}$ y $p_{\text{Ar}})$, potencia $(P)$, diferencia de potencial $(\Delta V)$, corriente $(I)$, espesor de la capa $(\text{Esp.})$, tiempo de _pre-sputtering_ $(t_{\text{pre}})$ y tiempo de _sputtering_ $(t_{\text{sp}})$.

El sustrato se colocará en un soporte especial, el cual permitirá definir la imanación del sensor en el sentido perpendicular al eje largo (figuras  [21](pylayer) y figura [43](sensorfield)), aplicando un campo magnético de $250 \; \mathrm{Oe}$. De esta forma, se propiciará la detección del cambio de la magnetorresistencia. Seguidamente, se introducirá en el lugar correspondiente de la cámara (figura [20](inside)).

```{figure} inside.PNG
---
height: 300px
name: inside
---
Interior de la cámara
```

En primer lugar, se debe __generar vacío__ en el interior de la cámara por medio de dos bombas. La bomba auxiliar rotatoria servirá como apoyo inicial para la bomba turbo molecular, la cual, más lentamente, logrará llegar hasta  $1,6\times10^{-6} \; \text{mbar}$ (alto vacío).

A continuación, se deberá suministrar gas de argón (_sputtering gas_) a una presión de $2,8 \times 10^{-3} \; \text{mbar}$, y se establecerá una potencia de $110 \; \text{W}$ mediante una fuente de corriente continua para __generar el plasma__ dentro del campo magnético creado por los magnetrones $(\approx 0,3 \; \text{T})$. Este campo confinará los electrones presentes en el gas de argón cerca del blanco de permalloy. La diferencia de potencial entre el ánodo y el cátodo acelerará dichos electrones, y éstos colisionarán con los átomos de argón más próximos. La repulsión electrostática causará la ionización de estos últimos. De esta forma, los iones de argón  $(\text{Ar}^{+})$ serán acelerados e impactarán con gran energía contra la superficie de permalloy, cuyos átomos serán extraídos y adquirirán la suficiente energía cinética para poder alcanzar el sustrato y difundirse en su superficie para hallar la posición de energía mínima, en donde quedarán depositados. Esto favorece la adhesión de la película, y también aumenta su densidad, reduciendo así los defectos.

```{admonition} Nota
 Es típico escoger un gas de _sputtering_ de alto peso molecular para incrementar el número de colisiones. Esto, a la vez, aumenta la tasa de deposición y, por tanto, acorta el proceso.
```

Llegados a este punto, cabe mencionar que  primeramente se debe realizar una __deposición previa__ (_pre-sputtering_). Este paso es crucial, puesto que la muestra de permalloy contiene una capa inicial de óxido por el efecto de la atmósfera del ambiente, y, si se depositara directamente en el sustrato, ésta se contaminaría de impurezas. El tiempo de _pre-sputtering_ ha sido de $3$ minutos. A continuación, se dará paso al propio _sputtering_, el cual requerirá alrededor de $6$ minutos para conseguir la capa de permalloy de $100 \; \text{nm}$ deseada. En la figura [21](pylayer) se puede observar la película de permalloy en la superficie. Como se ha comprobado después, el material depositado ha sido de mala calidad, lo cual ha repercutido en los resultados de las medidas (sección [9](medidas)).

```{figure} pylayer.PNG
---
height: 300px
name: pylayer
---
El sustrato en el soporte especial. La flecha roja define la dirección de imanación.
```

Tras la finalización del proceso de deposición, se llevará a cabo el ___lift-off___ de la capa de permalloy y la  eliminación de la resina bajo ella. El vidrio se sumergirá en acetona dentro de un vaso de precipitado cubierto con _parafilm_ (para evitar la evaporación de la acetona), durante $30$ minutos. La capa de resina debe quedar completamente retirada. Un baño en ultrasonidos puede resultar útil para este efecto. Acto seguido, se someterá a un baño en isopropanol de $2$ minutos. Finalmente, se secarán los restos con la pistola de nitrógeno. De esta manera, el permalloy habrá quedado depositado únicamente en los patrones correspondientes al sensor y a las cruces. Acto seguido, se analizarán los resultados.

(resultpy)=
## __6.6__ Resultados tras deposición de permalloy

```{figure} crossespy.PNG
---
height: 300px
name: pycrosses
---
Las cruces de alineamiento tras la deposición de Py (objetivo $\times 20$).
```

```{figure} 2.9s_sensors_2.jpg
---
height: 100px
name: sensors1
---
Objetivo $\times 20$
```

```{figure} 2.9s_sensors_x50.jpg
---
height: 100px
name: sensors2
---
Objetivo $\times 50$
```

Las imágenes [23](sensors1) - [24](sensors2) han sido adquiridas mediante el microscopio del laboratorio de materiales. El contorno de las cruces parece haber salido correctamente. Éstas van a ser determinantes para garantizar la correcta alineación entre sensores y contactos. Por otro lado, mediante este microscopio de mayor resolución también se han tomado imágenes de mayor calidad del sensor de permalloy. En este caso, los bordes no se han definido claramente, lo cual deja en evidencia el límite de la resolución del equipo de fotolitografía. Pese a ello, los elementos constituyentes del sensor se observan bien alineados y espaciados, y el material se ha depositado adecuadamente en su interior. Por consiguiente, podrán desarrollar su función debidamente.
