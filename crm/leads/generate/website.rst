=============================================
¿Cómo generar iniciativas desde mi sitio web?
=============================================

Su sitio web debe ser la primera herramienta de generación de iniciativas 
de la empresa. Con el sitio web en el eje central de sus campañas de publicidad 
en línea, usted va a conducir naturalmente tráfico cualificado para alimentar 
a su flujo de ventas. Cuando un prospecto cae en el sitio web, su objetivo es 
capturar la información, con el fin de ser capaz de mantenerse en contacto 
con él y empujarlo más abajo del canal de ventas.

De esta manera es el proceso de trabajo de la generación de iniciativas: 

-  Un visitante en su sitio web, hace clic en una llamada de acción (CTA) 
    desde uno de sus materiales de publicidad (por ejemplo, un boletín electrónico, 
    un mensaje de los medios de comunicación sociales o una entrada de blog)

-  La CTA lleva a su visitante a una página de destino que incluye un formulario 
    que se utiliza para recoger su información personal (por ejemplo, su nombre, 
    su dirección de correo electrónico, su número de teléfono)

-  El visitante envía el formulario y automáticamente se genera como iniciativa 
    en Odoo CRM

.. Consejo::

	Las llamadas de acción, las páginas y formas de destino, son las piezas 
  clave del proceso de generación de iniciativas. Con el sitio web de Odoo, 
  usted puede crear fácilmente y optimizar los elementos críticos sin tener 
  que codificar o utilizar aplicaciones de terceros. Obtenga más información 
  `aquí <https://www.odoo.com/page/website-builder>`__.

En Odoo, el sitio web y los módulos de CRM están totalmente integrados, lo que 
significa que usted puede fácilmente generar clientes potenciales de diversas 
maneras a través de su sitio web. Sin embargo, incluso si usted es anfitrión de 
su sitio web en otro CMS, aún así es posible completar los datos que requiere 
Odoo CRM con clientes potenciales generados desde su sitio web.

Activar las etapas de las iniciativas
=====================================

Por defecto, la etapa de la iniciativa no se activa en Odoo CRM. Por lo tanto, 
nuevas iniciativas se convierten automáticamente en oportunidades. Usted puede 
activar fácilmente la opción de agregar iniciativas. Si desea importar los 
contactos que tiene como oportunidades, desde el módulo de Ventas ir a 
:menuselection: `Configuración --> Ajustes`, seleccione la opción **Usar 
iniciativas si...** como se muestra a continuación y haga clic en **Aplicar**.

.. image:: ./media/website01.jpg
   :align: center

Tenga en cuenta que, incluso sin activar este paso, la información que sigue 
entrando, todavía es aplicable - la iniciativa generada aterrizará en el tablero 
de  oportunidades.

Desde el sitio web de Odoo
==========================

Supongamos que desea obtener la mayor cantidad de información posible acerca 
de cada visita al sitio web. Pero, ¿cómo podría usted asegurarse de que cada 
persona que quiere saber más sobre los productos y servicios de su empresa, 
dejará la información en cualquier lugar? Gracias a la integración de Odoo 
entre sus módulos de CRM y sitios Web, usted puede automatizar fácilmente 
los procesos de adquisición de iniciativas, gracias a los módulos de **Formulario 
de Contacto** y **Construcción de Formularios**

.. Nota::

	otra gran manera de generar iniciativas desde el sitio web de Odoo es mediante 
  la recopilación de direcciones de correo electrónico  de los visitantes gracias 
  a la Newsletter o Boletín emergente CTA. Estos fragmentos crearán nuevos contactos 
  en su lista de correo electrónico de publicidad. Obtenga más información 
  `aquí <https://www.odoo.com/page/email-marketing>`_.

Configuración
-------------

Comience por instalar el módulo constructor del sitio web. Desde el panel de 
control principal, haga clic en **Aplicaciones**, escriba "**Sitio Web**" en 
la barra de búsqueda y haga clic en **Instalar**. Usted será redirigido 
automáticamente a la interfaz web.

.. image:: ./media/website02.png
   :align: center

.. Consejo::

	Un tutorial emergente aparece en la pantalla si esta es la primera vez que 
  utiliza el Sitio Web de Odoo. Este le ayudará a iniciar con la herramienta 
  y usted será capaz de utilizarlo en cuestión de minutos. Por lo tanto, 
  le recomendamos usarlo.

Crear una iniciativa mediante el módulo de Formulario de contacto
-----------------------------------------------------------------

Puede generar iniciativas sin esfuerzo a través de un formulario de contacto 
en su página de **Contáctanos**. Para ello, primero debe instalar el Módulo 
de Formulario de Contacto. Se agregará un formulario de contacto en su página 
de **Contáctanos** y automáticamente se generará una presentación de los 
formularios de las diferentes iniciativas.

Para instalarlo, vuelva a la pantalla de fondo utilizando el icono cuadrado 
en la esquina superior izquierda. A continuación, haga clic en **Aplicaciones**, 
escriba "**Formulario de contacto**" en la barra de búsqueda (no se olvide de 
quitar la etiqueta **Aplicaciones** de otro modo que no verá el módulo) y haga 
clic en **Instalar**.

.. image:: ./media/website03.png
   :align: center

Una vez instalado el módulo, el siguiente formulario de contacto se integrará 
a su página "**Contáctanos**". Este formulario está vinculado a Odoo CRM, lo 
que significa que todos los datos introducidos a través del formulario serán 
capturados por el CRM y se creará una nueva iniciativa.

.. image:: ./media/website04.jpg
   :align: center

Cada iniciativa creada a través del formulario de contacto está disponible 
en el módulo de Ventas, haciendo clic en :menuselection:`Ventas --> Iniciativas`. 
El nombre de la iniciativa corresponde al campo "Asunto" en el formulario de 
contacto y toda la otra información se almacena en los campos correspondientes 
dentro del CRM. Como vendedor, usted puede añadir información adicional, 
convertir la iniciativa en una oportunidad o incluso directamente marcarlo 
como Ganado o Perdido.

.. image:: ./media/website05.jpg
   :align: center

Crear iniciativas usando el módulo de Construcción de Formularios
-----------------------------------------------------------------

Puede crear formularios personalizados totalmente editables en cualquier 
página de entrada en su sitio web con el fragmento de Forma de construir. 
En cuanto al módulo de Formulario de contacto, el Constructor de Formularios 
generará automáticamente una iniciativa después de que el visitante haya 
completado el formulario y haga clic en el botón **Enviar**.

Desde el backend, vaya a Configuración e instalar el módulo "**Constructor 
de Formularios**" (no te olvides de quitar la etiqueta **Aplicaciones** de 
lo contrario no verán los módulos). Luego, de vuelta en el sitio web, vaya 
a la página de destino que desee y haga clic en Editar para acceder a los 
fragmentos disponibles. El fragmento de Constructor de Formularios establece 
en la sección de **Características**.

.. image:: ./media/website06.png
   :align: center

Tan pronto como se le ha caído el fragmento en el que desea que aparezca el 
formulario en su página, una ventana de **Parámetros del formulario** aparecerá. 
En la lista desplegable **Acción**, seleccione **Crear iniciativa** para crear 
automáticamente una iniciativa en Odoo CRM. En el campo **Gracias**, seleccione 
la dirección URL de la página que desea redirigir a su visitante después de 
haber completado la forma (si no agrega ninguna URL, el mensaje "El formulario 
ha sido enviado con éxito" confirmará la acción).

.. image:: ./media/website07.png
   :align: center

A continuación, puede empezar a crear su formulario personalizado. Para añadir 
nuevos campos, haga clic en **Seleccione el bloque contenedor** y luego en el 
botón azul **Personalizar**. Aparecerán 3 opciones:

.. image:: ./media/website08.png
   :align: center

- **Cambie los parámetros de formulario**: esto le permite ir de nuevo a los 
  parámetros de formulario y cambiar la configuración

- **Añadir un campo al modelo**: esto le permite añadir un campo ya existente 
  en Odoo CRM de una lista desplegable. Por ejemplo, si se selecciona el campo 
  del *País*, el valor introducido por la iniciativa aparecerá bajo el campo *País* 
  en el CRM - incluso si se cambia el nombre del campo en el formulario.

- **Agregar un campo personalizado**: esto le permite añadir campos adicionales 
  que no existen de forma predeterminada en Odoo CRM. Los valores introducidos 
  se añadirán en "Notas" en el CRM. Usted puede crear cualquier tipo de campo: 
  casilla de verificación, botón de radio, texto, número decimal, etc.

Cualquier formulario presentado creará una entrada en la base de datos.

Desde otro CMS 
==============

Si utiliza Odoo CRM pero no el sitio web, todavía se puede automatizar el proceso 
de generación de prospectos en línea utilizando servidores de correo electrónico 
editando el botón "Enviar" de cualquier forma y reemplazar el hipervínculo por un 
mailto correspondiente a su nombre de correo electrónico (aprenderá a crear su nombre 
de ventas :doc:`aquí <emails>`).

Por ejemplo, si el nombre de su empresa es **salesEMEA@mycompany.com**, 
agregue ``mailto: salesEMEA@mycompany.com`` en el código del hipervínculo regular 
(CTRL+K) para generar una iniciativa en el equipo de ventas relacionadas en Odoo CRM.

.. image:: ./media/website09.png
   :align: center

.. seealso::

	- :doc:`manual`
	- :doc:`import`
	- :doc:`emails`

.. rst-class:: text-muted

| Escrito por Geoffrey Bressan (Odoo)
| Revisado por Yves-Pascal Mukadi, Samuel Cabodi (Odoo)
| Traducción por Alejandra Escandón (Jarsa)
