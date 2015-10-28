==========================================
¿Cómo crear un contacto en el CRM de Odoo?
==========================================

Odoo CRM le permite añadir manualmente contactos en su flujo de ventas. 
Puede ser una iniciativa o una oportunidad.

Activar las etapas de las iniciativas
=====================================

Por defecto, la etapa de la iniciativa no se activa en Odoo CRM. 
Para activarlo, vaya a :menuselection:`Configuración --> Ajustes`, seleccione la opción ""use iniciativa si...** como se muestra a continuación y haga clic en **Aplicar**.

.. image:: ./media/manual01.jpg
	:align: center

Esta activación creará un nuevo submenú **Iniciativas** bajo las **Ventas** que 
le da acceso a una lista de todos sus iniciativas en la cual será capaz de crear 
un nuevo contacto.

.. image:: ./media/manual02.jpg
	:align: center

Crear una nueva inciativa
=========================

Ir a :menuselection:`Ventas --> Iniciativas` y hacer clic en el botón de **Crear**.

.. image:: ./media/manual03.jpg
	:align: center

Desde el formato de contacto, se proporcionan todos los detalles que se posean 
(nombre de contacto, correo electrónico, teléfono, dirección, etc.), así como 
alguna información adicional en el campo de **Notas Internas**. También se puede 
vincular la iniciativa con el link a una empresa ya existente editando el campo 
**CLiente**. Haga clic en Guardar y el contacto será visible como una iniciativa 
en su flujo de ventas.

.. Nota::

	su iniciativa está vinculada directamente a un equipo de ventas específico o a 
	un vendedor, haga clic en el botón **Convertir a Oportunidad** en la esquina 
	superior izquierda de la pantalla. 

Crear una nueva Oportunidad

También se puede añadir directamente un contacto a un equipo de ventas específico 
sin tener que convertir la iniciativa en primer lugar. En el módulo de Ventas, 
vaya a su panel de control y haga clic en el botón de **Flujo de trabajo** del 
equipo de ventas deseado. Si usted no tiene ningún equipo de ventas aún, 
:doc:`es necesario crearlo primero <../../salesteam/setup/create_team>`. 
A continuación, haga clic en **Crear** y llenar los datos del contacto como se 
muestra arriba. Por defecto, la oportunidad recién creada aparecerá en la primera 
etapa de su proceso de ventas.

Otra forma de crear una oportunidad es añadiéndolo directamente en una etapa específica. 
Por ejemplo, si usted tiene en el historial que habló con el Sr. Smith en una reunión y 
desea que envié una cita de inmediato, usted puede agregar los datos del contacto 
directamente en la etapa de la **Propuesta**. Desde el punto de vista de Kanban de 
su equipo de ventas, simplemente haga clic en el icono **+** a la derecha del tablero, 
para crear el contacto. Entonces, la nueva oportunidad aparecerá en la etapa correspondiente 
y, a continuación, puede completar los datos de contacto haciendo clic en él.

.. image:: ./media/manual04.png
	:align: center

.. seealso::

	* :doc:`import`

	* :doc:`emails`

	* :doc:`website`

.. rst-class:: text-muted

| Escrito por Geoffrey Bressan (Odoo)
| Revisado por Yves-Pascal Mukadi (Odoo)
| Traducción por Alejandra Escandón (Jarsa)
