(problems)=
# **10**. Complicaciones

A lo largo del desarrollo de las sesiones de la sala blanca, han surgido tres problemas principales que han ralentizado el progreso experimental. Todos ellos están asociados al equipo de fotolitografía de _SmartPrint_.

__1. Inconsistencia en la dosis adecuada__: A medida que aumenta el uso de la máquina, se han requerido mayores tiempos de exposición con el fin de evitar la tonalidad oscura en los patrones. A causa de lo anterior, se han tenido que efectuar tests de dosis con cierta regularidad. Las tablas [4](table4) y [5](table5) denotan lo mencionado. En enero de 2022 se compró un bote nuevo de resina fotosensible, por lo que los tiempos de exposición y revelado crecieron considerablemente. De todas maneras, en el caso del sensor, se puede observar un incremento de más de 1 segundo en 3 meses para la misma resina. En el caso de la capa de los contactos, el aumento ha sido de 2 segundos en 2 meses. Finalmente, cabe mencionar que este equipo se ha destinado únicamente al desarrollo del presente trabajo de fin de grado (2 ó 3 sesiones por semana). Si aumentara la frecuencia de su empleo, el problema en cuestión se vería acentuado.

En cualquier caso, no se descarta que dicho incremento se pudiera deber a alteraciones en las propiedades la resina fotosensible, a causa de factores ambientales como la humedad o la exposición a la luz blanca.

```{list-table} Variación de la dosis de la primera capa.
:header-rows: 1
:name: table4

* - $\mathbf{Fecha}$
  - $\mathbf{Tiempo \; de\; exposición} \; (\text{s})$
  - $\mathbf{Tiempo \;de \;revelado} \; (\text{s})$
* - $13/07/21$
  - $0,8$
  - $60$
* - $28/02/22$
  - $2,7$
  - $90$
* - $05/05/22$
  - $3,5$
  - $90$
* - $19/05/22$
  - $4$
  - $90$
```

```{list-table} Variación de la dosis de la segunda capa.
:header-rows: 1
:name: table5

* - $\mathbf{Fecha}$
  - $\mathbf{Tiempo \; de\; exposición} \; (\text{s})$
  - $\mathbf{Tiempo \;de \;revelado} \; (\text{s})$
* - $31/03/22$
  - $1,7$
  - $60$
* - $12/05/22$
  - $2,5$
  - $60$
* - $26/05/22$
  - $2,7$
  - $60$
```

__2. Incoherencia en el alineamiento__: Como bien se ha indicado en la sección [7](thecontacts), pequeñas derivas en el posicionamiento del soporte han impedido que la correcta alineación se haya mantenido en la totalidad de la zona de interés. Una solución consistiría en prescindir del modo de alineamiento semi automático, y, por ende, de las cruces incluidas para este efecto. Pese a que el modo libre de alineamiento esté destinado a patrones de mayores dimensiones (objetivos $\times 1$ y $\times 2,5$) que no requieran un diseño en modo _stitching_, este método podría proporcionar resultados con la suficiente precisión y corrección.

__3. Problemas con el soporte motorizado__: En ocasiones, el motor del soporte no ha respondido a los comandos. Debido a ello, se ha tenido que recurrir al reinicio del equipo. Existe un cuaderno ubicado bajo la máquina que recoge las indicaciones a seguir ante este tipo de incidencias.
