# Reporte de Compras histórico sobre datos de Pedidos en Natura (2019-2023)

<img src="https://www.sana-commerce.com/wp-content/uploads/1152x720_NaturaBrasil.jpg" width="576" height="360" alt="natura logo">

## Introducción

Hace un año en el que iniciaba mi trayectoria en el mundo de la programación -En este punto aún no había elegido que quería convertirme en un especialista de datos- y estaba en la búsqueda de un empleo decidí que debía reaprender ciertas herramientas y así poder estar actualizado para poder emplearme más fácilmente. En este caso el programa que elegí fue Microsoft Excel, pues su uso es muy extendido y ya había tenido un acercamiento a este, por lo que estuve algunas semanas aprendiendo más funciones y entendiendolo a profundidad. 

Buscando como poner en práctica mis conocimientos recién adquiridos, a mi novia se le ocurrió una excelente idea, que yo analizara su historial de pedidos que había hecho en [Natura](https://www.natura.com.mx/) durante los años anteriores. Pero ¿Qué es Natura? Natura es una compañia multinacional brasileña que fabrica y comercializa productos de belleza e higiene a través de la venta directa la cual es hecha por consultores independientes, y de los cuales mi novia es una. 

En su página personal ella puede descargar una hoja de Excel que le brinda datos sobre sus pedidos, pero no tenía una idea clara de que podía hacer con ellos, pues el documento estaba en un formato algo viejo y la limpieza de datos no es algo que dominara, por lo que me pregunto si podía hacer algo con ellos o qué era lo que se podía hacer. 

En esa fecha que fue febrero de 2022 hice un Dashboard en Excel, y recientemene con datos actualizados hice el mismo reporte pero con Power BI.
Así que en esta presentación mostraré lo que hice para ella, con el permiso de poder compartirlo.

## Datos

Los datos fueron extraidos de la cuenta personal de Natura de mi novia, la cual otrogo me el permiso de revisar y publicar.

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
 
 
## Informes

### Informe de 2022

Este primer informe fue terminado el 17 de febrero del 2022 y fue elaborado en Microsoft Excel.

Con Excel se pueden hacer muchas cosas, entre ellas está el hacer Dashboards. El proceso que se uso fue simple:
- **Escoger indicadores:** Opté por utilizar solamentelos campos de fecha, valor total de compra, ciclo y estado.
- **Limpieza de datos:** 
  - Fecha: El formato de la fecha tiene algunos errores, pues aparece como texto, así que solo tuve que darle un formato de fecha.
  - Estado: Excluí los pedidos anulados mediante el uso filtros.

<img src="Assets/DashEPE10.png" width="430" height="215" title="Datos del 2022">

- **Análisis:** Procedí a hacer un formato de tabla para tablas dinámicas con los siguiente elementos:
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

- **Dashboard:** 
Finalmente uní todo en formato de referencia, agregue estructura y formato, y finalmete agregué segmentadores y los conecté a todas las tablas.
[]

