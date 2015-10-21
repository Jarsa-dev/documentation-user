========================================================================================
Automatice la asignación de iniciativas a los equipos de ventas o vendedores específicos
========================================================================================

Dependiendo del flujo de trabajo y las necesidades de su empresa, usted necesita 
enviar a sus iniciativas entrantes a diferentes equipos de ventas o incluso 
especificar a cuales vendedores serán asignados. Éstos son algunos ejemplos: 

- Su empresa tiene varias oficinas base en diferentes regiones geográficas. Usted
	tendrá que asignar las iniciativas basadas en la región; 

- Uno de sus equipos se dedica a tratar a las oportunidades de las grandes empresas,
	mientras que otro equipo debe estar especializado en las PYMES. Usted tendrá que
	asignar las iniciativas en base al tamño de la empresa;

- Uno de sus representantes de ventas es el único en hablar idiomas extranjeros,
	mientras que el resto des equipo habla Inglés solamente. Por lo tanto, tendrá
	que asignar a esa persona todas las iniciativas de los países donde el idioma
	Inglés no es su lengua nativa. 

Como se pueden imaginar, asignar manualmente nuevas iniciativas a personas específicas
puede ser tedioso y lento, especialmente si su empresa genera un gran volumen de
clientes potenciales cada día. Afortunadamente, Odoo CRM permite automatizar el proceso
de asignación de iniciativas en base a criterios específicos, tales como la ubicación,
intereses, tamaño de la empresa, etc., con flujos de trabajo específicos y reglas precisas,
usted será capaz de distribuir todas sus oportunidades automáticamente a los equipos de
ventas y/o al vendedor adecuado.

Configuración
=============

Si usted acaba de iniciar a trabajar con Odoo y no sabe como estableces equipos de ventas, ni registrar a us vendedores, :doc:`revisa este documento primero <../../overview/started/setup>`.

Defina reglas para sus equipos de ventas
========================================

Desde el módulo de ventas, vaya a su panel de control y haga clic en el botón **Más** del equipo de ventas deseado, luego en **Configuración**. Si usted no tiene ningún equipo de ventas, :doc:`es necesario crearlo primero <../../salesteam/setup/create_team>`.

.. image:: ./media/automatic01.jpg
   :align: center

En el menú de su equipo de ventas, use el **Dominio** del campo específico con su regla
(para más detalles técnicos sobre el dominio, hacemos referencia al
`Tutorial de Construcción de Módulos <https://www.odoo.com/documentation/8.0/howtos/backend.html#domains>`__
o a la  `Guía de referencias de Sintaxis <https://www.odoo.com/documentation/8.0/reference/orm.html#reference-orm-domains>`__)
el cual permitirá que sólo las iniciativas coincidan con el equipo de ventas. 

Por ejemplo, si usted quiere que su equipo de *Ventas Directas* sólo reciba
derivaciones procedentes de Estados Unidos y Canadá, el dominio será de la
siguiente manera:

``[[country_id, 'in', ['United States', 'Canada']]]``

.. image:: ./media/automatic02.jpg
   :align: center

.. Nota::

	también se puede basar la asignación automática de la puntuación atribuida a sus 
	lientes potenciales. Por ejemplo, podemos imaginar que desea que todos las iniciativas
	con una puntuación por debajo de 100, se asignarán a un equipo de ventas entrenados para 
	royectos más ligeros y las iniciativas de más de 100 a un equipo de ventas con más
	experiencia. Lea más sobre :doc:`la forma de puntuación clientes potenciales aquí <lead_scoring>`.

Defina reglas para los vendedores
=================================

Usted puede ir un paso más allá en sus reglas de asignación y decidir como asignar los
clientes potenciales a un equipo de ventas o a un vendedor específico. Por ejemplo,
si quiero que Toni Buchanan del equipo de *Ventas Directas* únicamente reciba iniciativas
procedentes de Canadá, puedo crear una regla que asignará automáticamente las iniciativas
ese país.

Aún en el menú de equipo de ventas (ver aquí arriba), haga clic en el vendedor de su
opción en el submenú asignación. A continuación, introduzca su regla en el campo *Dominio*.

.. image:: ./media/automatic03.jpg
   :align: center

.. Nota::

	En Odoo, una iniciativa siempre se asigna a un equipo de ventas antes de ser asignado
	a un vendedor. Por lo tanto, es necesario asegurarse de que la regla de asignación de su
	vendedor es un hijo de la regla de asignación del equipo de ventas.

.. vertambien::

	* :doc:`../../overview/started/setup`

	.. todo:: * How to assign sales activities into multiple sales teams?

	.. todo:: * How to make sure my salespeople work on the most promising leads?


.. rst-class:: text-muted

| Escrito por Geoffrey Bressan (Odoo)
| Revisado por Samuel Cabodi (Odoo)
| Traducción por Alejandra Escandón (Jarsa)
