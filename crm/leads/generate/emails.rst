============================================================
¿Cómo generar un cliente potencial desde un correo recibido?
============================================================

Hay varias maneras para que su empresa pueda :doc:`generar clientes potenciales
con Odoo CRM <manual>` Uno de ellos es el uso de correo electrónico genérico
de su empresa como un disparador para crear una nueva pista en el sistema.
En Odoo, cada uno de sus equipos de ventas está vinculado a su propia dirección
de correo electrónico desde que las perspectivas pueden llegar a ellos. Por ejemplo,
si la dirección de correo electrónico personal de su equipo de directo es
**direct@mycompany.example.com**, cada correo electrónico enviado creará
automáticamente una nueva oportunidad en el equipo de ventas.

Configuración
=============

Lo primero que necesita hacer es configurar **los servidores de correo electrónico salientes**
y **el correo electrónico de entrada** desde el :menuselection:`Módulo Ajustes -->
Configuración General`.

Luego de configurar el nombre del dominio en el campo que se muestra a continuación y
haga clic en **Aplicar**.

.. image:: ./media/emails01.jpg
   :align: center

Crear un nombre de dominio del equipo
=====================================

Vaya al módulo de Ventas y haga clic en **Tablero**. Usted verá que la activación
del nombre de su dominio ha generado un nombre de correo electrónico predeterminado para
sus equipos de ventas existentes.

.. image:: ./media/emails02.jpg
   :align: center

Usted puede personalizar fácilmente los nombres de sus equipos de ventas. Haga clic en
el botón Más desde el equipo de ventas de su elección, luego en **Configuración** para acceder
al formulario del equipo de ventas. Desde el campo **Nombre de correo electrónico**, escriba
su nombre de correo electrónico y haga clic en **Guardar**. Asegúrese de permitir poder recibir
correos electrónicos de todo el mundo.

A partir de ahí, cada correo electrónico enviado a esta dirección, generará una nueva
iniciativa en el equipo de ventas relacionado.

.. image:: ./media/emails03.jpg
   :align: center

Configurar un dominio de correo catch-all
=========================================

Adicionalmente al nombre del equipo de ventas, también puede crear un nombre de
correo electrónico genérico (por ejemplo, *contacto@* o *info@*), que también va a
generar un nuevo contacto en Odoo CRM. Después, desde el módulo de ventas, vaya a 
:menuselection:`Configuración --> Ajustes` y configure su dominio de correo catch-all.

.. Consejo::

	Usted puede elegir si los contactos generados a partir del correo catch-all se convierten
	en clientes potenciales u oportunidades utilizando los botones de radio que se ven la
	captura de pantalla a continuación. Tenga en cuenta que, por defecto, la etapa de la
	iniciativa no se activa en Odoo CRM.

.. image:: ./media/emails04.jpg
   :align: center

.. seealso::

	* :doc:`manual`
	* :doc:`import`
	* :doc:`website`

.. rst-class:: text-muted

| Escrito por Geoffrey Bressan (Odoo)
| Revisado por Samuel Cabodi (Odoo)
| Traducción por Alejandra Escandón (Jarsa)
