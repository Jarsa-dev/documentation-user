===============================================================
Solicitud de Cotización, Propuesta de Compra u Orden de Compra?
===============================================================

A pesar de que están íntimamente relacionados, las solicitudes de cotización, 
las ofertas de compra y órdenes de compra no son las mismas.

Una **Solicitud de Cotización** (RFQ) se utiliza cuando se va a comprar algunos 
productos y le gustaría recibir un presupuesto para esos productos. En Odoo, 
la solicitud de cotización se utiliza para enviar la lista de productos deseados 
a su proveedor. Una vez que el proveedor ha respondido a su solicitud, puede optar 
por seguir adelante con la oferta y la compra o para rechazar la oferta.

Una **Propuesta de Compra** (PT), también conocida como Convocatoria, se 
utiliza para impulsar la competencia entre varios proveedores con el fin de 
obtener la mejor oferta para una lista de productos. En comparación con los RfQ, 
una propuesta de compra se envía a múltiples proveedores, indicando si cada uno 
compiten entre sí, y cual es la mejor oferta para ganar. El interés principal, 
por lo general conduce a mejores ofertas.

Las **Órdenes de Compra** (PO) son órdenes actuales que colocan al proveedor que 
se haya elegido, ya sea a través de un RfQ, una solicitud de compra o simplemente 
cuando usted ya conoce qué proveedor está en la orden.

Cuándo usarlo?
==============

Un **RfQ** es interesante cuando usted no ha comprado antes productos con ese 
proveedor, y por lo tanto no sabe su precio. También es útil si se quiere desafiar 
a sus proveedores una vez que se tenga una relación bien establecida con ellos. 
También se puede utilizar para evaluar el costo de un proyecto y ver si se hace factible.

Una **Propuesta de Compra** se utiliza para las ofertas públicas que requieren 
una oferta abierta de varios proveedores. También es útil cuando se necesita 
para hacer una orden de una sola vez para un producto y desea obtener la mejor 
oferta, no importa qué proveedor sea. Se puede utilizar cuando el proveedor no 
ha llegado hasta sus estándares y le gustaría empujarlos para ofrecer un mejor 
servicio, o encontrar un reemplazo en sus competidores.

Cuándo no usarlo?
=================

**RfQ**\ se vuelven innecesarias una vez que se haya establecido el proveedor 
preferido de cada artículo, y sólo aumentará el retraso en la entrega de sus 
artículos. En ese caso, el proceso será más sencillo partiendo directamente 
de una Orden de Compra.

**Propuestas de compras** son un proceso largo y tedioso que es probable que 
tome varias semanas, en el mejor de los casos. Si necesita una entrega rápida, 
este no es el camino a seguir. Además, si usted tiene una relación bien establecida 
con un proveedor, piense dos veces antes de iniciar un PT con ellos, ya que podría 
romper la relación y, finalmente, dar lugar a ofertas menos interesantes.

Ejemplo

Mi empresa construye muebles de madera. Para la nueva serie de mesas que estamos 
diseñando, necesitamos algunos tornillos, marcos metálicos y protecciones de goma.

Puedo crear una Solicitud de Cotización en Odoo con estos productos a mi proveedor 
habitual, y enviarlo por correo electrónico. Él responde con una oferta. Sin embargo, 
no estoy convencido por la oferta, y quiero ver si alguien puede dar una mejor.

Decido empujar la competencia un poco y configurar una Propuesta de Compras, que 
Odoo enviará a una lista de proveedores con las características especificas. De 
las 8 ofertas que recibo, uno tiene mi atención y decide seguir adelante con eso.

Confirmo el pedido al proveedor mediante la creación de una Orden de Compra del PT, 
y me pregunta Odoo automáticamente la entrega de los artículos con el proveedor.

Configuración
=============

Si desea conocer acerca de cómo crear una **Orden de Compra**, lea el 
documento :doc:`from_po_to_invoice`

Si desea conocer acerca de cómo crear un **RfQ**, lea el documento :doc:`../purchases/rfq/create`

Si desea conocer acerca de cómo crear una **Propuesta de Compra**, lea el documento :doc:`../purchases/tender/manage_multiple_offers`

.. rst-class:: text-muted

| Escrito por Samuel Cabodi (Odoo)
| Revisado por Geoffrey Bressan (Odoo)
| Traducción por Alejandra Escandón (Jarsa)