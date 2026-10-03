# Perfil del proyecto

## Tema

Digitalización del inventario y estandarización de atributos y medidas de producto textil en Romantex S.A.C.

## Descripción

El proyecto propone diagnosticar y diseñar una base común para la información de productos, variantes, medidas, unidades de venta y disponibilidad de Romantex S.A.C. El foco estará en dos o tres familias textiles priorizadas y en el flujo que conecta el alta o recepción del producto con la consulta comercial, la cotización y el pedido.

El resultado será un modelo de datos aplicable a telas, revestimientos y accesorios, con atributos como familia, referencia de proveedor, composición, color, ancho, unidad de venta, aplicación, mantenimiento, ubicación y estado. La estandarización conservará el valor original del proveedor y registrará la normalización adoptada, sus excepciones y la persona responsable de validarla.

## Problema identificado

La diversidad de marcas, materiales, colores, composiciones, medidas y aplicaciones puede dificultar que los equipos comerciales y de almacén consulten el mismo producto con los mismos criterios. Esto puede traducirse en búsquedas repetidas, cotizaciones inconsistentes, dudas sobre la disponibilidad o dificultad para usar los datos de ventas en reposición y análisis básico. Estas situaciones son hipótesis de diagnóstico, no hechos internos demostrados por fuentes públicas; deberán comprobarse mediante una muestra de fichas, registros, movimientos y entrevistas.

El riesgo central es automatizar o conectar datos ambiguos. Por eso, el proyecto prioriza la calidad del dato y las reglas de actualización antes de proponer una integración técnica entre almacén, showrooms y canal web.

## Alcance

El trabajo abarcará el almacén y los showrooms públicos de San Isidro y Surco como contexto operativo, junto con el canal web de Romantex. La fase actual se limitará a dos o tres familias prioritarias, por ejemplo telas de tapicería y cortinas, revestimientos murales o línea Contract.

El entregable principal será el **MVP 1: diagnóstico y modelo maestro de producto**, compuesto por un mapa AS-IS validable, un diccionario de datos, una taxonomía textil, una propuesta de SKU, una plantilla de ficha y una matriz de calidad y responsabilidades. Como secuencia posterior se definirán un MVP de consulta de disponibilidad por ubicación y un MVP de indicadores comerciales y roadmap.

Quedan fuera la implementación completa de un ERP o WMS, la migración masiva de todo el histórico, la exigencia de inventario en tiempo real, RFID, inteligencia artificial predictiva y la evaluación financiera definitiva de proveedores.

## Tipo de sujeto

empresa

## MVP entregables

### MVP de arranque (recomendado al equipo)

**MVP 1 — Diagnóstico y modelo maestro de producto.** Permite verificar el problema con una muestra acotada, no depende de elegir una plataforma y habilita cualquier trabajo posterior de inventario o analítica.

### Secuencia

| MVP | Objetivo                                         | Entregables                                                                                                                                                             | Criterio de éxito                                                                                                               | Estado           |
| --- | ------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------- | ---------------- |
| 1   | Ordenar y validar el lenguaje del producto       | Mapa AS-IS; muestra de 2–3 familias; diccionario de datos; taxonomía; plantilla de ficha; propuesta de SKU; matriz de calidad y responsables                            | Cada registro de la muestra tiene atributos obligatorios, unidad de venta, estado de validación y excepción documentada         | se trabaja ahora |
| 2   | Diseñar una consulta confiable de disponibilidad | Estados disponible/reservado/no disponible; mapa de movimientos; reglas de actualización y reserva; especificación o prototipo de consulta; indicadores de conciliación | El usuario puede responder qué variante existe, en qué unidad, dónde está y cuándo se actualizó, o identificar el dato faltante | después          |
| 3   | Habilitar decisiones básicas de reposición       | Indicadores de rotación, quiebres, stock inmovilizado y completitud; backlog priorizado; roadmap TO-BE; opciones de herramientas                                        | Cada indicador tiene fuente, definición, periodicidad, responsable y limitación                                                 | después          |

### Fuera de secuencia / descartado

- Implantación total de ERP, WMS o PIM.
- Sincronización obligatoria en tiempo real entre todos los canales.
- Migración exhaustiva del histórico de todas las marcas.
- RFID, inteligencia artificial predictiva y automatización avanzada de almacén.
- Afirmar fallas de Romantex sin registros o entrevistas que las comprueben.

## Origen

- polish: docs/topics/IRD-2/theme-audit-polish.md
- veredicto: GO_con_cambios

## Marco PICOCT

| Componente | Definición           | Criterios / descripción del caso                                                                                                                                                                                                                                                                                                      |
| :--------: | :------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
|   **P**    | Population / Problem | PYME comercializadora de textiles decorativos con catálogo multimarca, inventario distribuido entre almacén y showrooms, y necesidad de mejorar la consistencia de productos, medidas, unidades de venta y disponibilidad para atención B2B/B2C. Problema: datos de producto e inventario potencialmente fragmentados o heterogéneos. |
|   **I**    | Intervention         | MVP 1 de diagnóstico y modelo maestro: diccionario de datos, taxonomía textil, propuesta de SKU, reglas de calidad, responsables y trazabilidad de normalizaciones; como continuación, diseño de consulta de disponibilidad por ubicación.                                                                                            |
|   **C**    | Comparison           | Práctica actual por validar: registros o catálogos separados, descripciones no normalizadas, consultas manuales y actualización no unificada. Alternativa: integrar canales antes de ordenar los datos maestros.                                                                                                                      |
|   **O**    | Outcome              | Completitud de atributos; porcentaje de variantes identificadas sin duplicidad; tiempo de búsqueda o respuesta; discrepancias entre muestra física y registro; porcentaje de consultas resueltas con una fuente común; existencia de responsables y fecha de actualización.                                                           |
|   **C**    | Context              | Perú, Lima; empresa de retail y distribución de decoración textil; venta consultiva residencial y comercial/Contract; almacén, showrooms y canal digital.                                                                                                                                                                             |
|   **T**    | Time / Type of study | 2026; revisión documental y estudio de diagnóstico aplicado con análisis de procesos y diseño de MVP.                                                                                                                                                                                                                                 |
