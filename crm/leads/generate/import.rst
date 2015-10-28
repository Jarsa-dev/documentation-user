================================
¿Cómo importar contactos al CRM?
================================

En Odoo CRM, se puede importar una base de datos de clientes potenciales, 
por ejemplo para una campaña de llamadas o de correos electrónicos para dar 
información de la empresa, a través de un archivo CSV. Usted se preguntará 
si la mejor opción es importar sus contactos como clientes potenciales u 
oportunidades; depende de sus especificaciones de negocios y flujo de trabajo:

-  Algunas compañías pueden decidir no usar iniciativas y en su lugar prefieren
	mantener toda la información directamente en una oportunidad. Para algunas 
	empresas, clientes potenciales no son más que un paso adicional en el 
	proceso de venta. Usted podría llamar a esta extensión (comienzo de iniciativa) 
	contra la simplificación (inicio de la oportunidad) de gestión de relaciones 
	con los clientes.

-  Odoo permite perfectamente que cualquiera de estos enfoques sea seleccionado. 
	Si su empresa maneja en las ventas un paso precalificación, no dude en activar 
	primero el escenario principal como se describe a continuación con el fin de 
	importar la base de datos y las iniciativas.

Activar las etapas de las iniciativas
=====================================

Por defecto, la etapa de la iniciativa no se activa en Odoo CRM. Si desea importar 
los contactos como iniciativas en lugar de oportunidades, vaya a 
:menuselection:`Configuración --> Ajustes`, seleccione la opción **Usar iniciativas 
si** ... como se muestra a continuación y haga clic en **Aplicar**.

.. image:: ./media/import01.jpg
   :align: center

Esta activación creará un nuevo submenú :menuselectio:`Ventas --> Iniciativas` 
desde la que se podrá importar sus contactos con el botón **Importar** (si desea 
crear una iniciativa de forma manual, :doc: haga clic aquí <manual>`)

.. image:: ./media/import02.jpg
   :align: center

Importar sus archivos CSV
=========================

En el nuevo submenú :menuselection: `Ventas --> Iniciativas`, haga clic en **Importar** 
y seleccione el archivo de Excel para importar desde el botón **Elegir archivo**. 
Asegúrese de que su extensión sea .csv y no se olvide de configurar las opciones de 
formato de los archivos correctamente (**Codificación** y *Separador**) para que 
coincida con los valores locales y se muestren las columnas correctamente.

.. Nota::
	Si la base de datos a los prospectos se proporciona en otro formato que no sea CSV, 
	usted puede fácilmente convertir al formato CSV con Microsoft Excel, OpenOffice / 
	LibreOffice Calc, Google Docs, etc.

.. image:: ./media/import03.jpg
   :align: center

Seleccionar filas para importar
===============================

Odoo asignará automáticamente los encabezados de las columnas de su archivo CSV a 
los campos correspondientes, si se marca *La primera fila del archivo, contiene la 
etiqueta de la columna* como opción. Esto hace que las importaciones sean más fáciles, 
especialmente cuando el archivo tiene muchas columnas. Por supuesto, puede reasignar 
los encabezados de la columna para describir la propiedad que va a importar de datos 
dentro (Nombre, Apellidos, Correo electrónico, etc.).

.. image:: ./media/import04.jpg
   :align: center

.. Consejo::

	Si desea importar los contactos como oportunidades en lugar de iniciativas, 
	asegúrese de añadir la columna *Tipo* en su csv. Esta columna se utiliza para 
	indicar si al importar se marcará como una iniciativa (tipo = Iniciativa) o 
	como una oportunidad (tipo = Oportunidad).

Haga clic en el botón **Validar** si desea dejar a Odoo verificar que todo se 
encuentre bien antes de importar. De lo contrario, puede hacer clic directamente 
en el botón Importar: y se realizarán las mismas validaciones.

.. Nota::

	Para obtener información técnica adicional sobre cómo importar contactos en Odoo 
	CRM, lea la sección de **Preguntas Frecuentes** situada debajo de la herramienta 
	de Importar en la misma ventana.
	
.. seealso::

	- :doc:`manual`
	- :doc:`emails`
	- :doc:`website`

.. rst-class:: text-muted

| Escrito por Geoffrey Bressan (Odoo)
| Revisado por Samuel Cabodi (Odoo)
| Traducción por Alejandra Escandón (Jarsa)
