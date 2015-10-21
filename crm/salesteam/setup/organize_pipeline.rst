=========================================
Establecer y organizar el flujo de ventas
=========================================

Un flujo de ventas bien estructurado es crucial para mantener el control
de su proceso de ventas y tener una visión de 360º de sus iniciativas,
oportunidades y clientes potenciales.

El canal de ventas es una representación visual de su proceso de ventas,
desde el primer contacto hasta la venta final. Se refiere al proceso mediante
el cual se genera, califica y se cierran iniciativas a través del ciclo de
ventas. En Odoo CRM, las iniciativas son traídas en el extremo izquierdo del
canal de ventas en la vista de Kanban, para después irlos trasladando a las
columnas de lado derecho según sea el avance de cada una.

Cada etapa se refiere a un paso específico en el ciclo de la venta y como se
específica cada iniciativa según su estado. El número de etapas se canaliza según
la venta, ya que varía de una compañía a otra. Un ejemplo de concetrar las ventas
sería con las siguientes etapas: *Nuevo, Calificación, Patrocinador Calificado,
Propuesta, Negociación, Ganados, Perdidos*.

.. image:: ./media/team_kanban.jpg
   :align: center

Por supuesto, cada organización define el canal de ventas en función a sus procesos
y al flujo de trabajo, por lo que pueden existir más o menos etapas de las ya mencionadas. 

Crear y organizar las etapas
============================

Añadir y reorganizar las etapas
-------------------------------

Desde el módulo de ventas, vaya al panel de control y haga clic en el botón
**FLUJO DE TRABAJO** del equipo de ventas deseado. Si usted no tiene ningún equipo
de ventas aún, es necesario crearlo primero.

.. todo:: link to the create salesteam page

.. image:: ./media/image09.jpg
   :align: center

.. todo:: ***Kanban view*** link to the CRM terminologies page

Desde el punto de vista Kanban de su flujo de trabajo, se pueden agregar etapas haciendo 
clic en **Añadir nueva columna**. Cuando se crea una columna, Odoo propondrá automáticamente
añadir otra columna con el fin de completar su proceso. Si desea cambiar el orden de sus
etapas, puede hacerlo fácilmente arrastrando y soltando la columna que desea mover a la
ubicación deseada.

.. image:: ./media/add_column.png
   :align: center

.. Consejo::

    Puede añadir tantas etapas como desee, aunque le aconsejamos no tener más de 6 con el
    fin de mantener un flujo de trabajo claro. 

Activar etapas a las iniciativas
--------------------------------

Algunas empresas utilizan una pre calificación para gestionar a sus iniciativas antes
de convertirlos en oportunidades. Para activar el escenario principal, vaya a
:menuselection:`Configuration --> Settings` y seleccione el botón de radio como se
muestra a continuación. Se va a crear un nuevo submenú **Iniciativas** abajo de **Ventas**
que le da acceso a una vista de lista de todos sus clientes potenciales.

.. image:: ./media/image01.jpg
   :align: center

Establecer probabilidades en las etapas
=======================================

Cuáles son las probabilidades de las etapas?
------------------------------------------------

Para entender mejor cuáles son las posibilidades de cerrar un acuerdo para una oportunidad
que se encuentra en su flujo, usted tiene que establecer un porcentaje de probabilidad para
cada una de sus etapas. Ese porcentaje se refiere a la tasa de éxito de cerrar el trato.

.. Nota:: La configuración de probabilidades de las etapas es esencial si se quiere estimar
los ingresos esperados de su ciclo de ventas

.. todo:: estimate the expected revenues of your sales cycle (*link to the related topic*)

Por ejemplo, si su ciclo de ventas contiene la etapa de Inicio, Calificación, Patrocinador
Calificado, la Propuesta, Negociación, Ganado y Perdido, entonces el flujo de trabajo podría
tener este aspecto:

- **Inicio** : La oportunidad se recibió de la Administración de Iniciativas
  o se creo a partir de una campaña. Los intereses del cliente aún no están
  confirmado. 

  *Tasa de éxito : 5%*

- **Calificación** : Se conoce el negocio y la perspectiva del flujo de trabajo,
  las áreas de oportunidad son identificadas y confirmadas, el presupuesto y el
  tiempo son conocidos. 

  *Tasa de éxito : 15%*

- **Patrocinador Calificado**: existe un contacto directo con la persona encargada
  de la toma de decisiones.
  
  *Tasa de éxito : 25%*

- **Propuesta** : El prospecto recibe la cotización.
  
  *Tasa de éxito : 50%*

- **Negociación**: El prospecto evalúa la cotización hecha.
  
  *Tasa de éxito : 75%*

- **Ganado** : El prospecto confirmó la contización y se recibe una orden de venta.
  El prospecto se ha convertido en cliente. 
 
  *Tasa de éxito : 100%*

- **Perdidos** : El prospecto no está interesado. 
  
  *Tasa de éxito : 0%*

.. Consejo:: 

      Dentro de su flujo de trabajo, cada etapa debe corresponder a un objetivo
      definido con una probabilidad correspondiente. Cada vez que se mueve su
      oportunidad a la siguiente etapa, la probabilidad de cierre de la venta
      se adaptará automáticamente.

      Usted debe considerar el uso de valor de probabilidad como **100** cuando se
      haya ganado o cerrado el acuerdo y **0** para acuerdo se cerró y está perdido.

Cómo establecer probabilidades en las etapas? 
---------------------------------------------

Para editar las etapas, haga clic en el botón **Configuración** que se encuentra de
lado derecho luego en EDITAR.

.. image:: ./media/image08.jpg
   :align: center

Seleccione la casilla del Cambio de probabilidad automático para permitir que Odoo
adapte la probabilidad de la oportunidad a la probabilidad definada en la etapa.
Por ejemplo, si se establece una probabilidad de 0% (Perdida) o 100% (Ganada),
Odoo asignará la etapa correspondiente cuando la oportunidad se marca como Perdida
o Ganada.

.. Consejo::

    En el campo de los requisitos se puede introducir los requisitos internos para
    esta etapa. Aparecerán como información sobre herramientas al colocar el puntero
    del ratón sobre el nombre de una etapa.

.. todo:: Read more

  - *How to estimate the effectiveness of my sales cycle?*
  - *How to estimate expected revenues ?*


.. rst-class:: text-muted

| Escrito por Geoffrey Bressan (Odoo)
| Revisado por Samuel Cabodi (Odoo)
| Traducción por Alejandra Escandón (Jarsa)

