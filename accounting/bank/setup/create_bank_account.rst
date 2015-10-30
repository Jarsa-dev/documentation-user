====================================
Configurar una nueva cuenta bancaria
====================================

En Odoo, se pueden administrar varias cuentas bancarias. En esta página, se le guiará 
en la creación, modificación o eliminación de un banco o de una tarjeta de crédito.

Ir a la lista de sus cuentas bancarias
--------------------------------------

Ir a :menuselection:`Configuración --> Ajustes --> Configurar su cuenta bancaria` >
Las cuentas bancarias estarán configuradas en la información de la empresa. Necesita entrar al modo de edición para configurar y generar los cambios necesarios. 

.. image:: media/image10.png
   :align: center

.. Nota::

	Si está trabajando en un entorno de multi-empresa, se debe de cambiar de empresa para agregar, editar o eliminar las cuentas bancarias de otras. 

Añadir o editar cuentas bancarias
---------------------------------

Da clic en **Añadir artículo** para añadir una nueva cuenta bancaria. Si desea editar alguna, simplemente de clic en el. 

.. image:: media/image03.png
   :align: center

.. Nota::
	
	Si la cuenta bancaria es de tipo IBAN, Odoo revisará que el número sea válidos.

.. demo:fields:: base.action_res_partner_bank_account_form

.. demo:action:: base.action_res_partner_bank_account_form

   Ver *Cuentas Bancarias* en la demostración en línea.

.. todo:: add inherited field tooltip

	**Display on reports :** Display this bank account on the documents that
	will be printed or send to the customers

	**Bank Identifier Code** = BIC : SWIFT Address assigned to a bank in
	order to send automated payments quickly and accurately to the banks
	concerned

El saldo inicial de una cuenta bancaria se establecerá en el saldo final de la anterior 
en el mismo diario automáticamente.

Como se puede reflejar en forma de diario, la cuenta especial que se ha generado 
de forma automática al crear una cuenta bancaria.

Eliminar una cuenta bancaria o cuenta de tarjeta de crédito
-----------------------------------------------------------

Haga clic en el icono de la papelera |image5| en la lista de sus cuentas bancarias se removerá la cuenta bancaria.

.. |image5| image:: media/image13.png
	:class: btn-group

.. rst-class:: text-muted

| Escrito por Benjamin Stiens (Odoo)
| Traducción por Alejandra Escandón (Jarsa)
