==================================================
¿Cómo configurar una regla de almacenamiento manualmente?
==================================================

Para algunos artículos considerados en almacenamiento, puede ser útil 
contar con reglas para asegurarse de que nunca se quede sin existencias 
(por ejemplo, los productos con una alta demanda, o artículos de gran 
tamaño que requieren una gran cantidad de espacio de almacenamiento es 
decir donde es más difícil el almacenamiento).

Odoo le permite configurar reglas para que se haga una reposición automática 
para esos artículos, en base a las existencias mínimas disponibles.

¿Cuándo se debe utilizar el reordenar las reglas?
=================================================

Reordenar las reglas funciona mejor para los artículos que tienen una 
alta demanda y un alto flujo. Se le exime de un montón de trabajo para 
centrarse en el resto de sus actividades a sabiendas de que las acciones 
siempre estarán bien.

También puede ser utilizado cuando se tiene espacio de almacenamiento 
limitado y donde se necesita mantener los artículos grandes en almacenamiento. 
En este caso, se pueden mantener tan poco como 1 artículo almacenado, y se 
tiene una nueva ordenada, como la reposición en el artículo de la acción se vende.

¿Cuándo debo evitar reordenar las reglas?
=========================================

Si usted está ofreciendo un producto nuevo y no sabe aún qué tan rápido 
se va a vender, usted debe utilizar primero almacenamiento propio, y la 
configuración de la reordenación de reglas sólo unos meses después de la 
venta para tener mejores previsiones de la demanda.

Si usted vende los artículos que tienen una vida útil limitada, tales 
como artículos de moda, artículos de tecnología, o productos de trabajo 
junto con un sistema que está destinado a evolucionar, tiene que estar 
muy bien informado sobre cuándo dejar las reposiciones automatizadas, 
con el fin de evitar tener que vender estos artículos a un precio que 
no permita el punto de equilibrio.

Ejemplo
=======

Mi empresa vende muebles modernos. Vendemos un conjunto de mesa y 
sillas que están disponibles en 4 asientos y 6 asientos.

Para simplificar las cosas, tenemos en almacenamiento mesas y sillas 
por separado, pero vendemos a todos nuestros clientes las piezas juntas, 
como un conjunto. Con el fin de asegurarse de que siempre se puede ofrecer 
un completo conjunto de mesa y sillas, se puede configurar una regla de 
Reordenación de las sillas para asegurarse de que siempre se tenga al 
menos 10 sillas en bodega, pero no más de 20. De esta manera, puedo vender 
hasta 5 juegos de mesa a la vez, manteniendo mis acciones lo suficientemente 
bajas como para no desperdiciar todo mi espacio de almacenamiento.

La última mesa que vendí era una de 4 asientos, y había 12 sillas que 
quedaban almacenadas. Debido a que las acciones de las sillas es ahora 
de sólo 8 sillas, Odoo ordenará automáticamente 12 sillas nuevas para 
llenar mi bodega a la cantidad máxima.

Configuración
=============

Configure su producto
---------------------

En el módulo de Compras, abra el menú de Compras y haga clic en Productos. 
Abra el producto al que desea agregar una regla de Reordenamiento (o crear uno nuevo).

1. En :menuselection:`Información General --> Tipo de Productos`, hacer el 
almacenamiento del producto (tan pronto como sea posible, aparecerá el icono 
de "Reordenación de regla")
2. En :menuselection:`Inventario --> ruta`, marque la casilla "Comprar" (y 
desmarque la casilla Hacer una Orden)
3. Seleccionar un vendedor (no olvide poner una cantidad mínima superior a 0)

Crear una Regla de Reordenamiento
---------------------------------

Haga clic en la ficha Reordenar las Reglas, después haga clic en Crear. 
Se abrirá una nueva página.

.. image:: media/setup01.png
  :align: center

Por defecto, el Reordenamiento de Reglas en Odoo aparecerá con el nombre 
de "OP/XXXXX", pero usted puede usar cualquier nomenclatura. Usted puede 
modificar el archivo mediante **Nombre**.

El archivo **Producto** se creará mediante la regla hecha. 

Seleccione el almacén donde el producto debe ser entregado en el campo **Almacén**.

Si ha configurado varios almacenes y ubicación, especifiqué la ubicación en 
la que el producto se almacenará en el campo **Ubicación**.

.. seealso::

  :doc:`../../../inventory/settings/warehouses/difference_warehouse_location`


.. image:: media/setup02.png
  :align: center

En el campo *+Cantidad Mínima**, introduzca la cantidad a la que el sistema 
activará un nuevo orden para la reposición.

En el campo **Cantidad Máxima**, introduzca el máximo de elementos que tiene 
que ser abastecido. La orden de reposición se basa en que la cantidad de reordenar.

La **Múltilple Cantidad** es el menor número de artículos que se pueden pedir a 
la vez. Por ejemplo, algunos artículos pueden sólo estar disponibles para su 
compra en un conjunto de 2.

En la sección Miscelánea, la sección **Activo** le permite activar o desactivar la regla.

En la sección **Tiempo de Entrega**, puede introducir

-  el número de día(s) para la compra: corresponden al número de días para 
que el proveedor reciba la orden

-  el número de día(s) para obtener los productos

.. Consejo:: Por defecto, los plazos de entrega son en días naturales. 
        Usted puede cambiar eso en :menuselection:`Inventario --> Configuración --> 
        Ajustes --> Reglas de Mínimos`

Cuando haya introducido toda la información, haga clic en Guardar.

A partir de ahora, cada vez que un producto con una regla de reordenamiento alcance 
las existencias mínimas, el sistema enviará automáticamente un RfQ a su proveedor 
basado en su cantidad máxima para reponer sus existencias.

.. Consejo:: Las reposiciones se llevarán a cabo cuando el planificador en el módulo 
        de inventario se ejecute. Por defecto en Odoo, los cambios se ejecutarán todas las noches a las 12:00 PM.

          Para saber cómo configurar y ejecutar los cambios de forma manual, 
          consulte el documento :doc:`../../../inventory/management/miscellaneous/schedulers`

.. seealso::
  
  :doc:`replenishment_methods`

  :doc:`../../../inventory/management/miscellaneous/schedulers`

.. rst-class:: text-muted

| Escrito por Samuel Cabodi (Odoo)
| Revisado por Geoffrey Bressan (Odoo)
| Traducción por Alejandra Escandón (Jarsa)
