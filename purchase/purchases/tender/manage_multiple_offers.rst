===================================================================================
Cómo gestionar múltiples ofertas de los proveedores con las solicitudes de compras?
===================================================================================

Una **Solicitud de Compras** (PT), también conocido como Convocatoria, se utiliza 
para impulsar la competencia entre varios proveedores con el fin de obtener la mejor 
oferta para una lista de productos. En comparación con los RfQ, una solicitud de 
compras se envía a múltiples proveedores, indicando si cada uno compiten entre sí, 
y cual es la mejor oferta para ganar. El interés principal, por lo general conduce 
a mejores ofertas.

Para obtener más información sobre el mejor uso, por favor lea el capítulo :doc:`../../overview/difference`

Configuración
=============

Activar la función de Solicitudes de Compras
--------------------------------------------

Por defecto, la Solicitud de Compra no está activada. Para poder utilizar los PT, 
primero debe activar la opción.

En el módulo de Compras, abra el menú de Configuración y haga clic en Ajustes. 
En la sección de Órdenes de compra, localizar las solicitudes y marque la casilla **Permitir el uso de solicitudes** ... (avanzado) y, a continuación, haga clic en **Aplicar**.

.. image:: ./media/image16.png
	:align: center

Crear una Solicitud de Compra
-----------------------------

Para crear una nueva Solicitud de Compra, abra :menuselection:`Compras --> Solicitudes de Compras`.

.. image:: ./media/image19.png
	:align: center

En la ventana de Solicitudes de Compra, haga clic en **Crear**. Se abrirá una nueva ventana de Solicitudes de Compra.

Por defecto, el nombre que le asigna Odoo a una PT es "TEXXXXX" pero se puede cambiar si así usted lo desea. 

.. image:: ./media/image21.png
	:align: center

En el campo **Responsable**, puede seleccionar a la persona que estará a cargo de la PT.

En el menú **Tipo de Solicitud de Compra**, puede decidir:

- seleccionar sólo una RfQ y automáticamente se cancelará el resto de las ofertas: 
*Seleccione sólo una RFQ (exclusiva)*

- permitir que varias órdenes de compra para la PT: *Seleccione múltiple RFQ*

Marque en el cuadro **Múltiples proveedores de RFQ** si desea permitir que los 
proveedores envíen más de una solicitud de cotización.

.. image:: ./media/image18.png
	:align: center

En el campo **Fecha límite del cierre de Solicitudes**, seleccione la fecha de 
las ofertas que están cerradas para los proveedores.

En el campo **Programar fechas de Órdenes**, seleccione la fecha en que desea 
colocar el pedido.

En el campo **Fecha programada**, seleccione la fecha en que los productos 
deben ser entregados.

En el campo **Origen de documento**, puede insertar una PO anterior y como plantilla.

.. image:: ./media/image15.png
	:align: center

En la sección de Productos, haga clic en **Agregar un elemento**.

Seleccione el producto en **Lista de Productos**, y después en insertar **Cantidad**. 
Puede agregar tantos productos como desee.

.. image:: ./media/image04.png
	:align: center

Haga clic en **Guardar** y después en **Confirmar llamadas**. Dos nuevas ventanas de 
RFQ y Solicitudes han aparecido de lado derecho de la pantalla.

.. image:: ./media/image17.png
	:align: center

Haga clic en **Solicitar una Cotización** y escriba los nombres de los proveedores 
que desea incluir en la PT, después haga clic en **Crear solicitud de cotización**.

.. image:: ./media/image12.png
	:align: center

La lista de proveedores aparecerá en la sección de **Requesiciones de Cotizaciones**

.. image:: ./media/image09.png
	:align: center

Para enviar las RFQ a losproveedores, haga clic en el icono V verde. También puede 
revisar los RfQ antes de enviarlos haciendo clic sobre ellos.

Cuando reciba ofertas, haga clic en la ficha RFQ. En la vista de lista, seleccione 
la empresa y haga clic en Editar para adaptar los datos como se indica en la oferta.

.. image:: ./media/image20.png
	:align: center

Cuando haya editado todos los campos correspondientes, haga clic en **Guardar**.

Cuando se ha alcanzado la fecha límite, haga clic en **Cerrar Solicitud**. El estado 
de la PT ahora a pasado a la **Selección de subastas**. Abra el RFQ que desea usar. 

.. image:: ./media/image14.png
	:align: center

Haga clic en **Aprobar Orden** para convertir la RfQ en una Orden de Compra, al volver 
a la PT, haga clic en **Listo** para cerrar la PT.

.. demo:action:: purchase_requisition.action_purchase_requisition

   Vea *Solicitudes de Compras* en la demostración de Odoo en línea.

.. seealso:: 

	:doc:`../../overview/from_po_to_invoice`

	:doc:`../../overview/difference`

.. rst-class:: text-muted

| Escrito por Samuel Cabodi (Odoo)
| Revisado por Geoffrey Bressan (Odoo)
| Traducción por Alejandra Escandón (Jarsa)
