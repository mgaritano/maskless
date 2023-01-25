(medidas)=
# **9**. Mediciones de magnetorresistencia

Primero, se cortará parte del vidrio mediante una punta de diamante, puesto que sus dimensiones superan las del porta muestras de las mediciones. Como  el sustrato de vidrio es muy quebradizo, corre el riesgo de dañar las estructuras, por lo que el corte se deberá efectuar con sumo cuidado. Acto seguido, se fijará con kapton, y se trazarán dos líneas de pintura de plata que unirán los contactos del porta muestras con los contactos externos de oro auxiliares.

Para comenzar, el soporte se colocará entre dos carretes circulares de Helmholtz, y se conectarán los cables en ambos extremos (figura [42](helmholtz)). El sensor deberá quedar alineado con respecto al eje. La resistencia eléctrica se calculará midiendo el voltaje y la intensidad ($R=V/I$). Esto se realizará mediante la denominada _medida a cuatro puntas_.

```{figure} setup.PNG
---
height: 300px
name: helmholtz
---
El soporte de las mediciones con el sustrato entre los carretes de Helmholtz. La __muestra 2__ ha sido la elegida.
```

Se empleará una fuente de gran precisión (resolución de $1 \; \text{nA}$), la cual hará circular una corriente de $0,5 \; \text{mA}$ en dirección paralela al eje largo del sensor. Un nanovoltímetro de 8 dígitos y medio de resolución medirá la tensión: $0,13 \; \text{V}$. En consecuencia, el sensor mostrará una resistencia inicial de $266 \; \Omega$. Después, los carretes de Helmholtz generarán un campo magnético $\mathbf{H}_{\text{ext}}$. Como la muestra se ha colocado en el eje de los carretes, la dirección del campo externo será paralela a la corriente. El soporte especial empleado en la deposición del permalloy ha inducido una anisotropía transversal. En consecuencia, en ausencia del campo externo, el sensor presentará una imanación $\mathbf{M}$ perpendicular a su eje largo (figura [43](sensorfield)).

```{figure} field.PNG
---
height: 100px
name: sensorfield
---
Imanación inicial de cada elemento del sensor y campo externo aplicado.
```

El objetivo es medir los cambios de la __magnetorresistencia anisótropa (AMR)__. Este fenómeno es característico de los materiales ferromagnéticos. En ellos, la resistividad muestra una dependencia en el ángulo entre las direcciones de la corriente y la imanación. Cuando el campo externo es pequeño, los cambios en la resistividad se agudizan, debido a la rotación de la imanación. Por otro lado, si el campo aumenta, la resistividad debería adquirir un comportamiento lineal {cite}`amr`. Considerando lo mencionado, se hará variar el valor del campo externo, siguiendo a este ciclo:

$$
150 \; \mathrm{Oe} \; \rightarrow \; 0 \; \mathrm{Oe} \; \rightarrow \; -150 \; \mathrm{Oe} \; \rightarrow \; 0 \; \mathrm{Oe} \; \rightarrow 150 \; \mathrm{Oe}  \;.
$$

La imanación del sensor responderá a dicha variación. Al comienzo, se alineará con el campo. No obstante, a medida que el módulo de $\mathbf{H}_ {\text{ext}}$ disminuye, el sensor recobrará su imanación inicial. En consecuencia, la magnetorresistencia disminuirá, y alcanzará un mínimo en $\mathbf{H}_{\text{ext}} = \mathbf{0}$. A continuación, aumentará, llegando a un nuevo máximo. En el gráfico de la figura [44](graph) se pueden observar los resultados de las mediciones.


```{figure} plot.PNG
---
height: 275px
name: graph
---
Cambio en porcentaje de la magnetorresistencia en el tramo de ida de las mediciones. A campos más bajos se ha incrementado el número de puntos.
```

En el gráfico se ha incluido únicamente el tramo de ida ($H_{\textrm{ext}} = 150 \; \mathrm{Oe} \rightarrow -150 \; \mathrm{Oe}$), en aras de mayor claridad visual. De hecho, se puede observar que, aunque la curva atiende a las explicaciones precedentes, el efecto del ruido es considerable, y de mayor agudeza en las zonas de campos pequeños $(\vert H_{\mathrm{ext}}\vert < 10 \; \mathrm{Oe})$. Partiendo de dos puntos correspondientes a la zona lineal, se calculará la sensibilidad del sensor:

$$
s = \frac{\Delta R}{\Delta H_{\text{ext}}} = \frac{(266,245 - 266,058) \; \Omega}{(-9,599 - 0,202) \; \textrm{Oe}} = -0,02 \; \frac{\Omega}{\textrm{Oe}} \; .
$$ (eq)

Por otra parte, los valores de la figura [44](graph) se han determinado por medio de la siguiente ecuación:

$$
\Delta R \; (\%) = 100 \times \frac{R - R_{\text{min}}}{R_{\text{min}}} \; .
$$ (eq2)

Así, el cambio máximo de magnetorresistencia es $\Delta R_{\text{max}} \; (\%) = 0,154 \; \% \;$. Este valor es relativamente pequeño. De hecho, los valores que se adquieren normalmente rondan el $4\; \%$; es decir, se esperaba una mayor caída en la zona sensible del sensor. Lo anterior se podría deber a deficiencias en el proceso de deposición del material. La muestra de permalloy se sometió a un proceso de mecanizado, lo cual alteró sus propiedades y deterioró su calidad. El equipo de _sputtering_, por su lado, ha sufrido percances recientemente, y se está trabajando de cara a  optimizar los parámetros del proceso.
