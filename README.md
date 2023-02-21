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

Cada uno de los registros representa un pedido en general el cual contiene los siguientes datos:
- **Número de pedido:** Puede entenderse como el id del pedido.
- **Número de factura
- **Fecha de pedido:** Fecha en que se realizo el pedido, no la fecha de entrega la cual se hace en alrededor de 5 días. 
- **Valor total de compra:** Suma total de los costos de los productos, envío, impuestos y otros.
- **Puntos obtenidos:** Los puntos natura son indicador del nivel en la empresa.
- **Ciclo:** Cada ciclo tiene una revista diferente, en la cual se ofrecen distintos productos y ofertas. Dura 21 días y hay 17 por año.
- **Estado:** Este campo indica si el pedido se realizó o no.



