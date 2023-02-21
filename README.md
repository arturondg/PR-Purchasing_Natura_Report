# Reporte de Compras histórico sobre datos de Pedidos en Natura (2019-2023)

<img src="https://www.sana-commerce.com/wp-content/uploads/1152x720_NaturaBrasil.jpg" width="576" height="360" alt="natura logo">

## Introducción

Hace un año en el que iniciaba mi trayectoria en el mundo de la programación -En este punto aún no había elegido que quería convertirme en un especialista de datos- y estaba en la búsqueda de un empleo decidí que debía reaprender ciertas herramientas y así poder estar actualizado para poder emplearme más fácilmente. En este caso el programa que elegí fue Microsoft Excel, pues su uso es muy extendido y ya había tenido un acercamiento a este, por lo que estuve algunas semanas aprendiendo más funciones y entendiendolo a profundidad. 

Buscando como poner en práctica mis conocimientos recién adquiridos, a mi novia se le ocurrió una excelente idea, que yo analizara su historial de pedidos que había hecho en [Natura](https://www.natura.com.mx/) durante los años anteriores. Pero ¿Qué es Natura? Natura es una compañia multinacional brasileña que fabrica y comercializa productos de belleza e higiene a través de la venta directa la cual es hecha por consultores independientes, y de los cuales mi novia es una. 

En su página personal ella puede descargar una hoja de Excel que le brinda datos sobre sus pedidos, pero no tenía una idea clara de que podía hacer con ellos, pues el documento estaba en un formato algo viejo y la limpieza de datos no es algo que dominara, por lo que me pregunto si podía hacer algo con ellos o qué era lo que se podía hacer. 

En esa fecha que fue febrero de 2022 hice un Dashboard en Excel, y recientemene con datos actualizados hice el mismo reporte pero con Power BI.
Así que en esta presentación mostraré lo que hice para ella, con el permiso de poder compartirlo.

## Datos

Los datos fueron extraidos de la cuenta personal de Natura de mi novia, la cual me otorgo el permiso de revisar y publicar.

Cada uno de los registros representa un pedido en general el cual contiene los siguientes campos:
- **Número de pedido:** Puede entenderse como el id del pedido.
- **Número de factura**
- **Fecha de pedido:** Fecha en que se realizo el pedido, no la fecha de entrega la cual se hace en alrededor de 5 días. 
- **Valor total de compra:** Suma total de los costos de los productos, envío, impuestos y otros.
- **Puntos obtenidos:** Los puntos natura son indicador del nivel en la empresa.
- **Ciclo:** Cada ciclo tiene una revista diferente, en la cual se ofrecen distintos productos y ofertas. Dura 21 días y hay 17 por año.
- **Estado:** Este campo indica si el pedido se realizó o no.

#### Datos sin procesar

- [Enlace a datos del 2022](https://correobuap-my.sharepoint.com/:x:/g/personal/arturo_diazga_alumno_buap_mx/EUgOBeR3LuFNgWjDfPDCYjkB9lcOiwnqM6bBQzsTODIXwA?e=82di8E)  (Fecha de obtención: 9 de febrero del 2022) 
- [Enlace a datos del 2023](https://correobuap-my.sharepoint.com/:x:/g/personal/arturo_diazga_alumno_buap_mx/ESKp0cKSlF1CqOy_DvmgcxQB1vAXqRZ_uHOqltMU-nNbZQ?e=q0TACE)  (Fecha de obtención: 14 de febrero del 2023) 

<div>
 <img src="Assets/DashEPE1.png" width="433" height="488" title="Datos del 2022">
 <img src="Assets/DashEPE2.png" width="433" height="488" title="Datos del 2023">
</div>
 
 
## Reportes

### Informe de 2022 (Microsoft Excel)

Este primer informe fue terminado el 17 de febrero del 2022 y fue elaborado en Microsoft Excel.

Con Excel se pueden hacer muchas cosas, entre ellas está el hacer Dashboards. El proceso que se uso fue simple:
- **Escoger indicadores:** Opté por utilizar solamentelos campos de fecha, valor total de compra, ciclo y estado.
- **Limpieza de datos:** 
  - Fecha: El formato de la fecha tiene algunos errores, pues aparece como texto, así que solo tuve que darle un formato de fecha.
  - Estado: Excluí los pedidos anulados mediante el uso filtros.

<img src="Assets/DashEPE10.png" width="430" height="215" title="Datos del 2022">

- **Análisis:** Procedí a hacer un formato de tabla para tablas dinámicas junto con los siguientes gráficos dinámicos:
  - Compras totales por año - _Gráfico de barras_
  - Evolución de compras - _Gráfico de lineas_
  -  Top 5 por ciclo - _Gráfico de columnas_
  -  Top 5 por fecha - _Gráfico de columnas_
  -  Promedio - _Gráfico de pastel_
  
 [**Enlace de Tablas**](https://correobuap-my.sharepoint.com/:x:/g/personal/arturo_diazga_alumno_buap_mx/ETvuTTx2VzVFk64NTDnt0_YBUq0n_L_2sDfPf_Plofh6OQ?e=cYrlD8)
 
<div>
 <img src="Assets/DashEPE11.png" width="365" height="289" title="Gráfico de barras">
 <img src="Assets/DashEPE12.png" width="472" height="287" title="Gráfico de lineas">
 <img src="Assets/DashEPE13.png" width="437" height="191" title="Gráfico de columnas">
 <img src="Assets/DashEPE14.png" width="434" height="210" title="Gráfico de columnas">
 <img src="Assets/DashEPE15.png" width="383" height="229" title="Gráfico de pastel">
</div>

- **Reporte:** 
Por último uní todo en formato de referencia, agregue estructura y formato, y finalmete agregué dos segmentadores:
- Fecha
- Ciclo  
y los uní a todos los gráficos para que estos se actualizaran.

#### [Enlace al Informe en Microsoft Excel](https://correobuap-my.sharepoint.com/:x:/g/personal/arturo_diazga_alumno_buap_mx/ERgN8wGfXN9CvpTcfgUE1rEBp1KaBpr7n4WNSLrqK_ergw?e=XbXpJq)

<img src="Assets/DashEPE16.png" width="960" height="431" title="Dashboard Natura Excel">

### Reporte de 2023 (Microsoft Power BI)

Este reporte casualmente fue terminado el 12 de febrero del 2023 y fue elaborado con Power BI.  

Si bien este reporte está derivado del anterior, la creación fue mucho más rápida y con creces. A pesar de que es una herramienta con la que he interactuado un poco menos, su interfaz es fácil de usar y de aprender. Y el acabado es más estético y limpio. Me permitio visualizar rápidamente y no hubo muchas complicaciones, es casi todo automático. Si pudiera enumerar los pasos estos serían muy pocos, pero los muesto en comparación con el informe anterior:

- **Limpieza de datos:** Esta tarea la hizo power BI automáticamente, sólo basto con cargar los datos del archivo y estos ya tenian un formato, mis únicas tareas consistieron en filtrar el Estado de pedidos, y agrupar los ciclos para una mejor segmentación -algo que pude haber hecho en Excel-.

<img src="Assets/DashEPE21.png" width="438" height="315" title="Datos Power BI">

- **Análisis:** Agregué los mismos gráficos y una tarjeta con el número de pedidos hechos, pues este número es muy importante para tener una idea más clara al usar los segmentadores.

- **Reporte:** 
En cuestión de segmentadores ahora agregué tres diferentes:
  - Año
  - Mes
  - Ciclo: Este último fue mejorado con respecto al anterior para una mejor visualización y control.
 En realidad todos tuvieron una mejora sustancial, pues esto permite un mayor control del reporte, y es más intuitivo y limpio.

<div>
 <img src="Assets/DashEPE17.png" width="262" height="473" title="Segmentadores 2022 Excel">
 <img src="Assets/DashEPE23.png" width="366" height="453" title="Segmentadores 2023 Power BI">
</div>

#### [Enlace al Reporte en Power BI](https://www.novypro.com/project/natura-report-dmanpg) (Este enlace esta novypro, un sitio para almacenar reportes en Power BI) 

<img src="Assets/DashEPE22.png" width="867" height="484" title="Reporte Power BI 2023">

## Comentarios

No sólo se puede notar que Power BI es una mejor herramienta para hacer está clase de visualizaciones, sino que el tiempo invertido es mucho menor. Lo que me llevo varias horas con Microsoft Excel, lo pude reducir a unas cuantas con Power BI.

También hago notar, que si bien no parece un proyecto muy complejo o de gran alcance, para mi será de los más valiosos, y no sólo porque lo hice para mi novia -aunque me parece un buen motivo- sino que lo importante es que fue y es funcional para ella. Pudo visualizar tendencias, alzas y bajas, y también patrones en sus pedidos. Como lo veo y he aprendido, los datos incluso ya visualizados deben tener un objetivo, no sólo es mostrar por mostrar, estos deben informar, ser funcionales para el público objetivo, tener un impacto para la toma de decisiones y creo que logré materializarlo en este primer proyecto.
