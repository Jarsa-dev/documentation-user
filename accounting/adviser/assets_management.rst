============================
Administre sus activos fijos
============================

El módulo "Activos" le permite mantener un registro de sus activos fijos, 
como maquinaria, terrenos y edificios. El módulo permite generar entradas de 
depreciación mensuales automáticamente, junta toda la depreciación, vende o 
enajena los activos y realizar informes sobre los activos de la compañía.

A modo de ejemplo, puede comprar un coche por $ 36.000 (valor bruto) y planea la 
amortización de acuerdo a 36 meses (3 años). Cada mes (periodicidad), Odoo crearán 
una entrada de depreciación reduciendo automáticamente el valor de los activos por 
$ 1,000 y esos $1,000 pasan como un gasto. Después de 3 años, este patrimonio cuenta 
por $ 0 (valor residual) en su balance.

Los diferentes tipos de activos se agrupan en "Tipos de Activos" que describen cómo 
deprecian un activo. He aquí dos ejemplos de activos tipos:

- Edificio: 10 años, depreciación lineal anual
- Coche: 5 años, la depreciación lineal mensual

Configuración
=============

Instalar el módulo de Activos
-----------------------------

Iniciar con *Instalar el Módulo de Activos.*

Una vez que el módulo ya está instalado, usted podrá ver los dos menús que se 
espliegan en la aplicación de Contabilidad: 

-  :menuselection:`Asesor --> Activos`
-  :menuselection:`Configuración --> Tipos de Activos`

Antes de registrar su primer activo, usted debe :ref:`definir sus Tipos de Activos 
<accounting/adviser/assets_management/defining>`.

.. _accounting/adviser/assets_management/defining:

Definir los Tipos de Activos
----------------------------

Los Tipos de Activos se utilizan para configurar toda la información acerca de 
un activo: cuentas de activos y depreciación, método de depreciación, etc. De 
esta manera, los asesores pueden configurar los tipos de activos y los usuarios 
pueden continuar con el registro de activos sin tener que proporcionar ninguna 
información contable que sea compleja. Sólo tienen que proporcionar un tipo de 
activo en la factura de proveedor.

Usted debe crear tipos de activos para cada grupo de activos que compra con 
frecuencia como "Carros: 5 años", "Hardware de la Computadora: 3 años". Para 
el resto de los activos, se pueden crear tipos de activos genéricos. Nombre 
de acuerdo a la duración del activo como "36 meses", "10 Años", ...

Para definir los Tipos de Activos, vaya a :menuselection:`Configuración --> Tipos de Activos`

.. image:: media/image01.png
   :align: center

.. demo:fields:: account_asset.action_account_asset_asset_list_normal_sale

.. demo:action:: account_asset.action_account_asset_asset_list_normal_sale

   Ver *Tipos de Activos* en la demostración en línea.

Crear Activos manualmente
=========================

Para registrar activos manualmente, vaya al menú :menuselection:`Asesor
--> Activos`.

.. image:: media/image08.png
   :align: center

Una vez creado su activo, no se olvide de confirmarlo. También puede hacer 
clic en el botón Depreciación Computadora para comprobar en el tablero antes 
de confirmar la depreciación del activo.

.. Consejo::

   si crea un activo manualmente, usted todavía necesita crear la factura del 
   proveedor para este activo. El documento activo sólo producirá los asientos 
   de diario de depreciación, no los relacionados con la factura del proveedor.

Explicación de los campos:

.. demo:fields:: account_asset.action_account_asset_asset_form

.. demo:action:: account_asset.action_account_asset_asset_form

   Trata de crear un *Activo* en la demostración en línea. 

Crear activos automáticamente desde la factura del proveedor
============================================================

Los activos se pueden crear de forma automática desde las facturas de los 
proveedores. Todo lo que se necesita hacer es establecer una categoría de 
activos en su línea de factura. Cuando el usuario haga válido el proyecto, 
se creará automáticamente un activo, utilizando la información de la factura 
de proveedor.

.. image:: media/image09.png

En función con la información de la categoría de activo, el activo se creará 
en el proyecto o se puede validarlo directamente\ *.* Es más fácil confirmar 
activos directamente para que no se le olvide el hacerlo después. (comprobar 
el *Saltar Estados del Proyecto* sobre *Categoría de Activos*) Generar activos 
en el proyecto sólo cuando usted quiere que su asesor controle todos los activos 
antes de la publicación a sus cuentas.

.. Consejo:: 
        si usted pone el activo en el producto, la categoría del activo automáticamente se cubrirá en la factura de proveedor.

¿Cómo depreciar un activo?
==========================

Odoo creará diarios de asientos de depreciación de forma automática en la fecha 
adecuada para cada activo confirmado. (no a los proyectos de). Usted puede controlar 
en el tablero de la depreciación: una viñeta verde que significa que la entrada 
de diario se ha creado para esta línea.

Pero también se puede publicar entradas de diario antes de la fecha prevista, haga clic en el botón verde y así se hará creará la entrada de la depreciación relacionada.

.. image:: media/image11.png
   :align: center

.. Nota:: En el tablero de Depreciación, haga clic en el botón rojo para dar la entrada del diario. De clic en :guilabel:`Artículos` botón que se encuentra en la parte superior, el cual permitirá ver las entradas publicadas. 

¿Cómo modificar un activo existente?
====================================

-  Da clic en :guilabel:`Modificar Depreciación`
-  Cambiar el valor de la depreciación

Odoo recalculará automáticamente el cambio y lo mostrará en una nueva entrada del tablero.

¿Cómo regstrar la venta o disposición de un activo?
===================================================

Si usted vende o dispone de un activo, es necesario despreciar completamente este activo. 
Haga clic en el botón :guilabel:`Vender o Disponer`. Esta acción publicará los costos 
completos de estos activos pero no va a registrar la transacción de venta que debe ser 
registrada por medio de una factura de cliente.

.. todo:: → This has to be changed in Odoo: selling an asset should:

   #. remove all "Red" lines
   #. create a new line that deprecate the whole residual value

.. rst-class:: text-muted

| Escrito por Fabien Pinckaers (https://odoo.com)
| Revisado por Laurence Henrion, Antony Lesuisse
| Traducción por Alejandra Escandón (Jarsa)
