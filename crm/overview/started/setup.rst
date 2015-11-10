=======================================================================
¿Cómo configurar los equipos, el proceso y los objetivos de las ventas?
=======================================================================

Esta guía rápida paso a paso los guiará a través Odoo CRM y les ayudará a manejar
y canalizar sus ventas fácil y constantemente, administrando las ventas de iniciativas
a clientes potenciales.

Configuración
=============

Primero es necesario crear una base de datos de `www.odoo.com/start <http://www.odoo.com/start>`__, seleccione el icono de CRM como primera aplicación para instalar, llene el formulario y
haga clic en *Crear ahora*. Usted será automáticamente dirigido al módulo cuando la base de
datos esté lista.

.. image:: media/setup01.png
  :align: center

.. Consejo::

        Usted se dará cuenta de que la instalación del módulo de CRM ha creado los submódulos Chat, Calendario y Contactos. Estos son obligatorios para que todas las características de la 
        aplicación funcionen sin problemas.

Introducción a la Planeación de ventas
======================================

El Planificador de Ventas es una guía útil paso a paso, creado para ayudarle a implementar
su canal de ventas y definir sus objetivos de ventas de manera sencilla. Le recomendamos
que vaya a través de cada paso de la herramienta la primera vez que utilice Odoo CRM y es 
necesario seguir los requisitos. Su entrada es estrictamente personal y esta pretende ser
una guía personal y como mentor en su trabajo. Como no interactúa con el servidor, usted
es libre de adaptar cualquier detalle cada vez que sienta que es necesario.

Se puede llegar al Planificador de Ventas desde cualquier lugar dentro del módulo de CRM,
haga clic en la barra de progreso situada en la parte superior derecha de la pantalla. Se
le mostrará hasta dónde está usted en el uso del Planificador de Ventas.

.. image:: ./media/setup02.png
   :align: center

Configure su primer equipo de ventas
====================================

Crea un nuevo equipo
--------------------

Un equipo de Venta Directa es creado por defecto en la instancia. Usted puede usarlo o crear uno nuevo. Consulte la página es :doc:`../../salesteam/setup/create_team` para más información.

Asignar vendedores responsables al equipo de venta
--------------------------------------------------

Cuando se crean equipos de ventas, el siguiente paso es vincular su personal de ventas al
equipo para que sean capaces de trabajar en las oportunidades que se supone deben recibir.
Por ejemplo, si dentro de su empresa Tim es el encargo de la venta de productos y John es
responsable de la  venta de contratos de mantenimiento, ellos serán asignados a diferentes
equipos y sólo recibirán oportunidades que tengan sentido para ellos.

En Odoo CRM, puede crear un nuevo usuario sobre la marcha y asignar directamente a un equipo
de ventas. Desde el **Tablero**, haga clic en el botón **Más** de su equipo de ventas seleccionado,
a continuación en **Configuración**. Luego, en la sección **Asignación**, haga clic en **Crear**
para agregar un nuevo vendedor al equipo.

Desde la **Creación: Vendedor** aparecerá la ventana (ver imagen abajo),
se puede asignar a alguien en su equipo:

- Puede ser que su vendedor ya existe en el sistema y usted sólo tiene que hacer
  clic en él en la lista desplegable y se le asignará al equipo
- O usted desea asignar un nuevo vendedor que no existe en el sistema sin embargo, usted puede
  hacerlo mediante la creación de un nuevo usuario sobre la marcha del equipo de ventas. Sólo
  tiene que introducir el nombre de su nuevo vendedor y haga clic en Crear (ver más abajo) para
  crear un nuevo usuario en el sistema y directamente asignarlo a su equipo. El nuevo usuario
  recibirá una invitación de correo electrónico para configurar su contraseña y entrar en el
  sistema. Consulte :doc:`../../salesteam/manage/create_salesperson` Para obtener más información
  acerca de este proceso.

.. image:: ./media/setup03.png
   :align: center

Configure su flujo de trabajo
-----------------------------

Ahora que su equipo de ventas esta creado y sus vendedores están vinculados al mismo, tendrá que
configurar su flujo de trabajo, crear el proceso por el que el equipo va a generar, calificar y cerrar las oportunidades a través de su ciclo de ventas. Consulte el documento :doc:`../../salesteam/setup/organize_pipeline` para definir las etapas del flujo de trabajo. 

Configuración del nuevo correo electrónico para generar oportunidades
---------------------------------------------------------------------

En Odoo CRM, una manera de generar oportunidades en su equipo de ventas es crear una dirección
de correo electrónico genérica como un disparador. Por ejemplo, si la dirección de correo electrónico personal de su equipo de directo es `direct@mycompany.example.com <mailto:direct@mycompany.example.com>`__\, cada correo electrónico enviado creará automáticamente una nueva oportunidad en el equipo de ventas.

Consulte la página :doc:`../../leads/generate/emails` para configurarlo.

Automatice la asignación de iniciativas
---------------------------------------

Si su empresa genera un gran volumen de clientes potenciales cada día, podría ser útil para automatizar
la asignación y así el sistema distribuirá todas sus oportunidades de forma automática al departamento correcto.

Consulte el documento :doc:`../../leads/manage/automatic_assignation` para más información.s

.. todo::
    
    Related topics
    -  CRM onboarding video

.. rst-class:: text-muted

| Escrito por Geoffrey Bressan (Odoo)
| Revisado por Samuel Cabodi (Odoo)
| Traducción por Alejandra Escandón (Jarsa)
