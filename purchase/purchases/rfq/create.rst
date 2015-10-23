========================================
¿Cómo crear una Solicitud de Cotización?
========================================

Una Solicitud de Cotización (RfQ) se utiliza cuando se va a comprar 
algunos productos y le gustaría recibir un presupuesto para esos productos. 
En Odoo, la solicitud de cotización se utiliza para enviar una lista de 
productos deseados a su proveedor. Una vez que el proveedor ha respondido 
a su solicitud, puede optar por seguir adelante con la oferta y la compra 
o rechazar la oferta.

Para obtener más información sobre el mejor uso, por favor lea el capítulo :doc:`../../overview/difference`

Configuracións
=============

Creación de una Solicitud de Cotización
---------------------------------------

En el módulo de Compras, abra el menú :menuselection:`Compras --> Solicitud de Cotización`
y haga clic en **Crear**.

.. image:: ./media/image04.png
	:align: center

Seleccione a su proveedor en el menú de **Proveedor**, o puede crearlo en la marcha, 
haga clic en **Crear y Editar**. En el campo **Fecha de pedido**, seleccione la fecha 
en la que desea continuar con el orden real.

.. demo:fields:: purchase.purchase_rfq

.. demo:action:: purchase.purchase_rfq

   Vista de la *Solicitud de Cotización* en la demostración en línea

En los **Productos**, haga clic en Agregar un elemento. Seleccione el producto 
que desea ordenar en el menú **Producto**. Especifique la **Cantidad** insertando 
el número y la selección de la unidad de medida. En el campo **Precio por unidad**, 
especifique el precio que le gustaría ofrecer (también se puede dejar en blanco si 
no sabe cual precio debería ser), y añadir la fecha de entrega prevista en el campo 
**Fecha programada**. Haga clic en **Guardar** y, a continuación, **Imprimir Rfq**, 
o **Enviar Rfq por correo electrónico**, (asegúrese de que la dirección de correo 
electrónico sea especifica para este proveedor o introduzca uno nuevo.

.. image:: ./media/image08.png
	:align: center

Después de haber hecho clic en **Enviar**, usted se dará cuenta de que el estado 
de la petición de oferta pasará de **Borrador** a **RFQ enviados**.

.. image:: ./media/image06.png
	:align: center

Una vez que el proveedor ha respondido con la oferta, se deben actualizar los RfQ haciendo clic en **Editar** para adaptarse a la cotización (precios, impuestos, plazo de entrega previsto, condiciones de pago, etc.), a continuación, haga clic en **Guardar** para emitir una Orden de Compra.

Para continuar con la orden, haga clic en **Confirmar Orden** para enviar el pedido al proveedor. El estado del RfQ cambiará a **Orden de Compra**.

.. image:: ./media/image11.png
	:align: center

El estado de la RfQ cambiará a la ORDEN DE COMPRA. En la esquina superior derecha de la orden se mostrarán 1 Envío y 0 Facturas.

.. image:: ./media/image10.png
	:align: center

.. seealso:: 

	:doc:`../../overview/from_po_to_invoice`

.. rst-class:: text-muted

| Escrito por Samuel Cabodi (Odoo)
| Revisado por Geoffrey Bressan (Odoo)
| Traducción por Alejandra Escandón (Jarsa)
