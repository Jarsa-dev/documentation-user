==============================
La Contabilidad detrás de Odoo
==============================

Esta página resume las posiciones que ofrece Odoo de cuentas y transacciones típicas.

Contabilidad de doble entrada
=============================

Odoo crea automáticamente todas las entradas detrás de escena de los diarios 
para cada una de sus operaciones contables: facturas de clientes, orden del 
punto de venta, los gastos, movimientos del inventario, etc.

Odoo utiliza las reglas de la doble entrada: todas las entradas de diario 
se equilibran automáticamente (suma de los débitos = suma de créditos).

→ Comprender las transacciones contables de Odoo por documento. (enlace al recuerdo)

Métodos básicos de efectivo y formas de devengar el efectivo
============================================================

Odoo da soporte a los reportes básicos de efectivo y a los reportes por devengar. 
Esto le permite informar los ingresos o gastos en el momento que se realizan las 
transacciones, o cuando el pago se hace o se recibe.

Multi-empresas
==============

Odoo permite gestionar varias empresas dentro de la misma base de datos. Cada empresa 
tiene en su propio plan de cuentas algunas reglas. Usted puede obtener informes de consolidación siguiendo las reglas de consolidación que haya establecido.

Los usuarios pueden acceder a varias empresas pero siempre trabajar en una empresa al momento.

Multi-monedas
=============

Cada transacción se registra con la moneda base de la empresa. Para las transacciones 
que ocurren en otra moneda, Odoo toma tanto el valor de la moneda de la empresa y el 
valor en la moneda de la transacción para hacer los cambios necesarios. Odoo puede generar 
divisas de ganancias y pérdidas después de la reconciliación en los diarios de artículos.

Los tipos de cambio se actualizan una vez al día usando un servicio web en línea de yahoo.com.

Estándares Internacionales
==========================

La Contabilidad de Odoo da soporte a más de 50 países. Existe el núcleo de contabilidad 
en Odoo para implementar las normas de contabilidad que son comunes en todos los países 
y módulos específicos por país para las especificaciones de cada uno, como el plan de 
cuentas, impuestos, o interfaces bancarias.

En particular, el motor del soporte de contabilidad central de Odoo:

* Contabilidad Anglosajona (EE.UU., Reino Unido ,, y otro países que hablan Inglés 
	incluyendo Irlanda, Canadá, Australia, y Nueva Zelanda) donde el costo del bien 
	vendido se reporta cuando los productos son vendidos o entregados.
* Contabilidad Europea donde los gastos se contabilizan en la cuenta del proveedor.

Odoo también tienen módulos para cumplir con las normas IFRS.

Cuentas por cobrar y por pagar
==============================

Por defecto, Odoo utiliza una sola cuenta para todas las entradas de las cuentas 
por cobrar y una para todas las entradas de las cuentas por pagar. Puede crear 
cuentas separadas por clientes y/o por proveedores, pero no es necesario.

Como las transacciones están asociados a los clientes o proveedores, se obtienen 
informes para realizar análisis por cliente y/o proveedor, tales como la declaración 
del cliente, los ingresos por clientes, cuentas por pagar por cobrar, edad, ...

Amplia gama de reportes financieros
===================================

En Odoo, se puede generar reportes financieros en tiempo real. Los reportes de 
Odoo van desde reportes básicos de contabilidad hasta los reportes de gestión 
avanzada. Los reportes de Odoo incluyen:

* Reportes de rendimiento (tales como las pérdidas o ganancias, variantes del presupuestos)
* Reportes de posición (como balance general, cuentas por pagar pasadas, cuentas por cobrar pasadas)
* Reportes de efectivo (tales como el resumen de los bancos)
* Reportes a detalle (tales como el balance y la contabilidad general)
* Gestión de reportes (como presupuestos y resumen ejecutivo)

La configuración de informes en Odoo le permite personalizar su propio informe sobre 
la base de sus propias fórmulas.

Importar automáticamente los canales de bancos
==============================================

La conciliación bancaria es un proceso que se ajusta a las líneas de extractos de 
la cuenta suministrada por el banco, a sus operaciones contables en el libro mayor. 
Odoo hace la conciliación bancaria facilitada con frecuencia para importar líneas 
de extractos de la cuenta de su banco directamente en su cuenta de Odoo. Esto 
significa que usted puede tener una vista diaria de su flujo de efectivo sin tener 
que acceder a su banca en línea o esperar sus estados de cuenta bancarios impresos.

Odoo acelera la conciliación bancaria, haciendo coincidir la mayoría de sus líneas 
de los estados bancarios importados a sus operaciones contables. Odoo también recuerda 
cómo se han tratado otras líneas de extractos de cuenta y proporciona sugerencia de 
transacciones del libro mayor.

Calcula los impuestos que debe su autoridad fiscal
==================================================

Odoo totaliza todas sus transacciones contables para el período impositivo y utiliza 
estos totales para calcular su obligación tributaria. A continuación, puede comprobar 
el impuesto sobre las ventas mediante la ejecución del Reporte de Impuestos de Odoo.

Valoración del inventario
=========================

Odoo soporta valoraciones de inventario tanto periódicas (manuales) y fijas 
(automatizadas). Los métodos disponibles son el precio estándar, precio medio, 
LIFO (para los países que le permiten) y FIFO.

→ Ver el impacto del método de valoración de las transacciones (enlace a memento)

Utilidades retenidas fácilmente
===============================

Las utilidades retenidas son la porción de la renta retenida por la empresa. 
Odoo calcula automáticamente las ganancias del año en curso en tiempo real, que 
no se requieren en ningun diario. Esto se calcula para informar de la ganancia 
y la pérdida en su reporte de balance general automáticamente.

| Traducción por Alejandra Escandón (Jarsa)
