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

     **Gastos Operativos** (OPEX) inclyen administración, ventas y salarios, así como 
     la renta y los servicios públicos, gastos diversos, seguros... nadamás lo que está 
     en los costos de los productos vendidos

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

   examples of accounting entries for various transactions. Example:

   Example 1: Customer Invoice:

   Explanation:

     - You generate a revenue of $1,000
     - You have a tax to pay of $90
     - The customer owes $1,090

   Configuration:

     - Income: defined on the product, or the product category
     - Account Receivable: defined on the customer
     - Tax: defined on the tax set on the invoice line

     The fiscal position used on the invoice may have a rule that
     replaces the Income Account or the tax defined on the product by another
     one.

   Example 2: Customer Payment:

   Explanation:

     - Your customer owes $1,090 less
     - Your receive $1,090 on your bank account

   Configuration:

     - Bank Account: defined on the related bank journal
     - Account Receivable: defined on the customer

.. _accounting/reconciliation:

Reconciliación
==============

Reconciliation is the process of linking journal items of a specific account,
matching credits and debits.

Its primary purpose is to link payments to their related invoices in order to
mark invoices that are paid and clear the customer statement. This is done by
doing a reconciliation on the *Accounts Receivable* account.

An invoice is marked as paid when its Accounts Receivable journal items are
reconciled with the related payment journal items.

Reconciliation is performed automatically by the system when:

* the payment is registered directly on the invoice
* the links between the payments and the invoices are detected at the bank
  matching process


.. h:div:: doc-aside reconciliation-example

   .. rubric:: Customer Statement Example

   .. rst-class:: table-condensed d-c-table

   +-------------------------+-------------------------+-----------------------+
   |Accounts Receivable      |Debit                    |Credit                 |
   +=========================+=========================+=======================+
   |Invoice 1                |100                      |                       |
   +-------------------------+-------------------------+-----------------------+
   |Payment 1.1              |                         |70                     |
   +-------------------------+-------------------------+-----------------------+
   |Invoice 2                |65                       |                       |
   +-------------------------+-------------------------+-----------------------+
   |Payment 1.2              |                         |30                     |
   +-------------------------+-------------------------+-----------------------+
   |Payment 2                |                         |65                     |
   +-------------------------+-------------------------+-----------------------+
   |Invoice 3                |50                       |                       |
   +-------------------------+-------------------------+-----------------------+
   |                         |                         |                       |
   +-------------------------+-------------------------+-----------------------+
   |Total To Pay             |50                       |                       |
   +-------------------------+-------------------------+-----------------------+


Bank Reconciliation
===================

Bank reconciliation is the matching of bank statement lines (provided by your
bank) with transactions recorded internally (payments to suppliers or from
customers). For each line in a bank statement, it can be:

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
