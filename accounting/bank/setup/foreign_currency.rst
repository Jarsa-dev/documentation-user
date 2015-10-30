=====================================================
¿Cómo administrar un banco con una moneda extranjera?
=====================================================

En Odoo, cada transacción se registra en la moneda base de la compañía. Los 
informes se basan en la moneda que tiene registarda la empresa. Pero para las 
transacciones que ocurren en otra moneda, Odoo almacenará el valor de la moneda 
de la empresa y el valor en la moneda de la transacción.

Cuando usted tiene una cuenta bancaria en una moneda extranjera, por cada transacción, 
almacenará los dos valores:

-   La tarjeta de débito o de crédito en la moneda de la compañía

-   La tarjeta de débito o de crédito en la moneda de la cuenta bancaria

Los tipos de cambio se actualizan automáticamente usando yahoo.com, o los servicios 
web del Banco Central Europeo.

Configuración
=============

Activar la función multi-moneda
-------------------------------

Con el fin de permitir que su empresa pueda trabajar con múltiples monedas, debe 
activar el modo multi-moneda. En la aplicación de la contabilidad, ir a 
:menuselection:`Configuración --> Ajustes --> Características de Contabilidad y 
Finanzas` y haga que la casilla **Permitir Multi-divisas** esté marcada. Proporcione 
una Cuenta de **Ganancia o Pérdida**, después haga clic en **Aplicar**.

Configure monedas
-----------------

Una vez que el Odoo está configurado para soportar múltiples divisas, usted debe activar 
las monedas que planea trabajar. Para ello, vaya a :menuselection:`Configuración --> Monedas`. 
Todas las monedas se crean de forma predeterminada, pero usted debe activar las que desea 
utilizar. (para activar una moneda, compruebe su campo activo)

Después de haber activado las monedas que desea, puede configurar los parámetros para 
automatizar la actualización de tipos de cambio. Estas opciones también se encuentran 
en la configuración de la aplicación de Contabilidad, en la parte inferior de la página:

.. image:: media/foreign01.png
   :align: center

Haga clic en el enlace **Actualizar Ahora** para actualizar los tipos de cambio ahora.

Crear una nueva cuenta bancaria
-------------------------------

En la aplicación de Contabilidad, debe ir primero a :menuselection:`Configuración -->
Contabilidad/ Cuentas bancarias`, y crear una nueva.

.. image:: media/foreign02.png
   :align: center

Una vez que se ha guardado la cuenta bancaria, Odoo creará todos los documentos necesarios: 

- Una cuenta en el balance general

- Una cuenta en el tablero

- Información sobre la cuenta bancaria en el pie de página de sus facturas si está 
activada la casilla **Facturas de Pie de Página**

Ejemplo: Una factura de proveedor en moneda extranjera
======================================================

Basado en el ejemplo anterior, supongamos que recibimos la siguiente factura de un 
proveedor en China.

En la :menuselection:`Compras --> Facturas de proveedores`, esto es lo que se podrá ver:

.. image:: media/foreign03.png
   :align: center

Una vez que esté listo para pagar esta cuenta, haga clic en el pago de registro en 
la factura para grabar un pago.

.. image:: media/foreign04.png
   :align: center

Eso es todo lo que se tiene que hacer. Odoo publicará automáticamente la ganancia o 
pérdida cambiando la conciliación del pago en la factura, dependiendo de si el tipo 
de cambio aumenta o disminuye entre la factura y la fecha de pago.

Tenga en cuenta que usted puede pagar una factura extranjera con otra moneda. 
En tal caso, Odoo convertirá automáticamente entre os valores de las dos monedas.

Declaraciones de clientes
=========================

Los clientes y las declaraciones de los proveedores se gestionan en la moneda de 
la factura. Por lo tanto, la cantidad en deuda por el cliente (a su proveedor) 
siempre se expresa en la moneda de la factura.

Si tiene varias facturas con diferentes monedas para el mismo cliente, Odoo dividirá las 
declaraciones por cliente en tipo de moneda, como se muestra en el informe a continuación.

.. image:: media/foreign05.png
   :align: center

En el informe anterior, la cuenta asociada por cobrar  a Camptocamp no se gestiona en una moneda secundaria, lo que significa que mantiene cada transacción en su propia moneda. Si lo prefiere, puede configurar la cuenta por cobrar de este cliente con una moneda secundaria y todas sus deudas se convertirán automáticamente en esta moneda.

En tal caso, la declaración del cliente siempre tendrá sólo una moneda. En general, esto 
no es lo que espera el cliente, ya que él preferirá ver los importes en la moneda de las 
facturas que recibió;

| Traducción por Alejandra Escandón (Jarsa)
