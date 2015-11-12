:code-column:

================================================================
Recordatorio rápido de Contabilidad para Emprendedores (US GAAP)
================================================================

.. h:div:: intro-list

   .. rst-class:: intro-p-l

  El informe de **Pérdidas y Ganancias** (P&G) muestra el rendimiento de la 
  empresa durante un período determinado (generalmente el año en curso).

   * .. rst-class:: intro-gross-profit

     La **Ganancia Bruta** es igual a los ingresos provenientes de las ventas 
     menos el costo de los bienes vendidos.

   * .. rst-class:: intro-opex

     **Gastos Operativos** (OPEX) incluyen administración, ventas y salarios, así como 
     la renta y los servicios públicos, gastos diversos, seguros... nada más lo que está 
     en los costos de los productos vendidos.

   .. rst-class:: intro-balance

   La **Hoja de Balance** es una vista instantánea de las finanzas de la empresa en una fecha 
   determinada (a diferencia de la de pérdidas y ganancias, que es un análisis en un período)

   * .. rst-class:: intro-assets

     Los **Activos** representan la riqueza de la sociedad, las cosas que se poseen. 
     Activos fijos incluyen la construcción y las oficinas, activos corrientes incluyen 
     cuentas bancarias y dinero en efectivo. Un cliente que debe dinero es un activo. 
     Un empleado no es un activo.

   * .. rst-class:: intro-liabilities

     Los **Pasivos** son obligaciones de los acontecimientos pasados ​​que la empresa 
     tendrá que pagar en el futuro (facturas de servicios públicos, deudas, proveedores 
     pendientes de pago).

   * .. rst-class:: intro-equity

     La **Equidad** es la cantidad de los fondos aportados por los propietarios (fundadores 
     o accionistas), además de las ganancias retenidas previamente (o las pérdidas).

     .. rst-class:: intro-retained

     Cada año, las utilidades netas (o pérdidas) se reportan en los resultados acumulados.

.. h:div:: doc-aside accounts-table

   .. placeholder

Lo que es de la propiedad (un activo) se ha financiado a través del reembolso de deudas 
(pasivos) o del capital (ganancias, capital).

Una diferencia se hace entre la compra de un activo (por ejemplo, un edificio) y un 
gasto (por ejemplo, combustible). Los activos tienen un valor intrínseco en el tiempo, 
en comparación con los gastos que tienen otro valor, ya que se consumen para que la 
empresa "trabaje".


.. rst-class:: doc-aside

.. highlights:: Assets = Liabilities + Equity

Catálogo de Cuentas
===================

El **Plan de Cuentas** enumera todas las cuentas, ya sean cuentas del balance general 
o cuentas de las pérdidas y las ganancias. Cada transacción financiera (por ejemplo, 
un pago, una factura) modifican las cuentas por valor de pasar de una cuenta (crédito) 
a otro cuenta (débito).

.. h:div:: doc-aside

   .. highlights:: Balance = Débito - Crédito

   .. h:div:: chart-of-accounts

      .. placeholder


Entradas de Diario
==================

Cada documento financiero de la empresa (por ejemplo, una factura, un estado 
de cuenta bancario, un recibo de pago, un contrato de ampliación de capital) 
se registra como una entrada de diario, impactando varias cuentas.

Por cada entrada de diario debe ser *balanceada*, la suma de todos sus débitos 
debe ser igual a la suma de todos sus créditos.

.. h:div:: doc-aside journal-entries

   ejemplos de algunas entradas contables de diferentes entradas. Por ejemplo: 

   Ejemplo 1: Factura del cliente:

   Explicación:

     - Usted genera un ingreso de $1,000
     - Usted tiene un impuesto a pagar de $90
     - El cliente debe $1,090

   Configuración:

     - Ingresos: definido en el producto, o en la categoría del producto
     - Cuenta por Cobrar: definido en el cliente
     - Impuestos: definir en el conjunto de impuestos la línea de factura

     La posición fiscal utilizada en la factura puede tener una regla que sustituye a la Cuenta de ingresos o el impuesto definido en el producto por otro.

   Ejemplo 2: Pago del Cliente:

   Explicación:

     - Su cliente le debe $1,090 menos
     - Su recibo $1,090 en su cuenta bancaria

   Configuración:

     - Cuenta Bancaria: definida en el diario bancario relacionado
     - Cuenta por Cobrar: definido en el cliente

.. _accounting/reconciliation:

Reconciliación
==============

La reconciliación es el proceso de vinculación de diarios de artículos en una 
cuenta específica, créditos y débitos a juego.

Su objetivo principal es vincular los pagos a sus facturas relacionadas con 
el fin de marcar cuales facturas fueron pagadas y mandar el comunicado al 
cliente. Esto se hace mediante una reconciliación en las *Cuentas por Cobrar*.

Una factura se marca como pagada cuando los diarios de artículos en Cuentas por 
cobrar son reconciliados con los artículos de diarios de pago relacionadas.

La reconciliación se realiza automáticamente por el sistema cuando:

* el pago se ha registrado directamente en la factura
* los vínculos entre los pagos y las facturas se detectan en el proceso del banco correspondiente

.. h:div:: doc-aside reconciliation-example

   .. rubric:: Ejemplo de Declaración del Cliente

   .. rst-class:: table-condensed d-c-table

   +-------------------------+-------------------------+-----------------------+
   |Cuentas por Cobrar       |Débito                   |Crédito                |
   +=========================+=========================+=======================+
   |Factura 1                |100                      |                       |
   +-------------------------+-------------------------+-----------------------+
   |Pago 1.1                 |                         |70                     |
   +-------------------------+-------------------------+-----------------------+
   |Factura 2                |65                       |                       |
   +-------------------------+-------------------------+-----------------------+
   |Pago 1.2                 |                         |30                     |
   +-------------------------+-------------------------+-----------------------+
   |Pago 2                   |                         |65                     |
   +-------------------------+-------------------------+-----------------------+
   |Factura 3                |50                       |                       |
   +-------------------------+-------------------------+-----------------------+
   |                         |                         |                       |
   +-------------------------+-------------------------+-----------------------+
   |Total por Pagar          |50                       |                       |
   +-------------------------+-------------------------+-----------------------+


Reconciliación Bancaria
=======================

Conciliación bancaria es la adecuación de las líneas de los estados bancarios (recibida 
por el banco) con transacciones registradas internamente (pagos a proveedores o desde 
los clientes). Para cada línea en un estado de cuenta bancaria, que puede ser: 

matched with a previously recorded payment:
  a payment is registered when a check is received from a customer, then
  matched when checking the bank statement
recorded as a new payment:
  the payment's journal entry is created and :ref:`reconciled
  <accounting/reconciliation>` with the related invoice when processing the
  bank statement
recorded as another transaction:
  bank transfer, direct charge, etc.

Odoo should automatically reconcile most transactions, only a few of them
should need manual review. When the bank reconciliation process is finished,
the balance on the bank account in Odoo should match the bank statement's
balance.

.. rst-class:: checks-handling

Checks Handling
===============

There are two approaches to manage checks and internal wire transfer:

* Two journal entries and a reconciliation
* One journal entry and a bank reconciliation

.. h:div:: doc-aside

   The first journal entry is created by registering the payment on the
   invoice. The second one is created when registering the bank statement.

   .. rst-class:: table-condensed d-c-table

   +-------------------------+--------------+------------+---------------+
   |Account                  |Debit         |Credit      |Reconciliation |
   +=========================+==============+============+===============+
   |Account Receivable       |              |100         |Invoice ABC    |
   +-------------------------+--------------+------------+---------------+
   |Undeposited funds        |100           |            |Check 0123     |
   +-------------------------+--------------+------------+---------------+

   .. rst-class:: table-condensed d-c-table

   +-------------------------+--------------+------------+---------------+
   |Account                  |Debit         |Credit      |Reconciliation |
   +=========================+==============+============+===============+
   |Undeposited funds        |              |100         |Check 0123     |
   +-------------------------+--------------+------------+---------------+
   |Bank                     |100           |            |               |
   +-------------------------+--------------+------------+---------------+

.. h:div:: doc-aside

   A journal entry is created by registering the payment on the invoice. When
   reconciling the bank statement, the statement line is linked to the
   existing journal entry.

   .. rst-class:: table-condensed d-c-table

   +-------------------------+--------------+------------+---------------+---------------+
   |Cuentas                  |Débito        |Credit      |Reconciliation |Bank Statement |
   +=========================+==============+============+===============+===============+
   |Account Receivable       |              |100         |Invoice ABC    |               |
   +-------------------------+--------------+------------+---------------+---------------+
   |Bank                     |100           |            |               |Statement XYZ  |
   +-------------------------+--------------+------------+---------------+---------------+
