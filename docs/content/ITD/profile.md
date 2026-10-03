# Perfil del proyecto

## Tema
Digitalización del inventario y estandarización de atributos de producto textil en Romantex S.A.C.

## Descripción
El proyecto examina cómo se articulan hoy el inventario físico — almacén central y showrooms de San Isidro y Surco —, el catálogo multimarca importado y los canales comerciales de Romantex S.A.C.: venta consultiva, línea Contract y presencia web. A partir de ese diagnóstico, se propone diseñar una fuente única de verdad del producto mediante atributos textil estandarizados (composición, color, ancho, unidad metro/rollo y aplicación residencial o contract), de modo que las consultas de disponibilidad sean confiables, los pedidos más eficientes y los datos de venta aprovechables en análisis básicos, sin pretender un ERP enterprise ni omnicanal en tiempo real.

## Problema identificado
Romantex gestiona un catálogo comercial heterogéneo en el que cada marca importada emplea nomenclaturas propias, mientras el registro de inventario y la atención multicanal carecen de un lenguaje común de producto. Esa desalineación dificulta confirmar con oportunidad si un material está disponible en stock o debe pedirse por catálogo, genera inconsistencias en cotizaciones entre almacén, showrooms y canal digital, y limita el uso de datos de venta para reposición y tendencias. Se formula como **hipótesis verificable** mediante entrevistas a roles operativos y observación de flujos, no como magnitud del dolor ya cuantificada.

## Alcance
El alcance geográfico y operativo comprende el almacén central, los showrooms de Av. Paz Soldán 185 (San Isidro) y Av. El Polo 376 (Surco), y el canal web romantex.com.pe. En producto, se priorizan dos o tres familias (telas de tapicería/cortinas, revestimientos murales y línea Contract). El entregable académico incluye mapeo AS-IS con supuestos validables, benchmark sectorial, propuesta TO-BE (taxonomía, modelo de datos y reglas de sincronización inventario–catálogo–comercial) y recomendaciones priorizadas; cualquier roadmap de implementación queda **condicionado** a los hallazgos del diagnóstico. Quedan excluidos ERP/WMS enterprise, RFID, IA predictiva y la estandarización exhaustiva del histórico importado completo.

## Tipo de sujeto
empresa

## MVP entregables

### MVP de arranque (recomendado al equipo)
**MVP 1 — Taxonomía textil + SKU piloto** — Define el lenguaje común del producto antes de cualquier integración multicanal; sin atributos y SKU acordados, sync de inventario o analítica solo amplifica inconsistencias. Gana el debate frente a MVPs 2–4 por dependencia de datos.

### Secuencia
| MVP | Objetivo | Entregables | Criterio de éxito | Estado |
|-----|----------|-------------|-------------------|--------|
| 1 | Fuente única de producto (taxonomía + SKU piloto) | Mapa AS-IS flujo dato producto; taxonomía deco mínima; modelo datos TO-BE; convención SKU interna; piloto 30–50 refs en maestro gobernado; matriz brechas nomenclatura proveedores; designación data owner | ≥90 % ítems piloto con atributos obligatorios completos; vendedor responde qué es, composición y unidad de venta sin cruzar 3 fuentes | se trabaja ahora |
| 2 | Visibilidad multisede consultable | Modelo ubicaciones; procedimiento conteo/ajuste periódico; tablero stock por sede para piloto; flujo transferencias almacén↔showroom; SLA frescura de dato | Consulta disponibilidad piloto en <2 min; discrepancia físico vs registro ≤10 % en auditoría muestral | después (condicionado a MVP 1) |
| 3 | Alineación catálogo web existente | Mapa campos web vs taxonomía; reglas publicación; proceso sync manual/asistido hacia romantex.com.pe; guía consulta Contract | 100 % piloto alineado con maestro; cero divergencia atributos clave en auditoría trimestral | después (condicionado a MVP 1+2) |
| 4 | Analítica comercial básica (opcional) | 5–8 KPIs; plantilla reporte mensual; reglas reposición simples min/max | ≥1 decisión compra/reposición documentada con dato estandarizado en trimestre post-piloto | después (opcional) |

### Fuera de secuencia / descartado
- ERP/WMS enterprise, RFID, IA predictiva, omnicanal DOM tipo Pittarello/OneStock.
- Estandarización de todo el catálogo multimarca histórico en fase diagnóstico.
- «Puente web greenfield» — el catálogo digital ya existe; el gap es alinear atributos/stock, no crear canal desde cero.
- Matriz talla–color tipo confección Gamarra (inaplicable a metro/rollo deco).

## Origen
- polish: docs/topics/ITD/theme-audit-polish.md
- veredicto: GO_con_cambios

## Marco PICOCT

| Componente | Definición | Criterios / descripción del caso |
| :---: | :--- | :--- |
| **P** | Population / Problem | Romantex S.A.C. (~17 trabajadores) y su cadena corta importador–showroom–cliente B2B2C; desalineación catálogo multimarca, inventario físico multisede y atención comercial consultiva (stock vs pedido por catálogo, cotizaciones inconsistentes, datos de venta infrautilizados) |
| **I** | Intervention | Diagnóstico + diseño TO-BE de taxonomía textil, modelo SKU piloto y reglas de sincronización periódica inventario–catálogo–comercial (PIM ligero / gobernanza de datos, no ERP enterprise) |
| **C** | Comparison | Práctica actual inferida: fichas dispersas, catálogos PDF, registros manuales o desconectados entre almacén, showrooms y web (OpenCart/cotización sin cantidades); alternativas commodity ERP local (Odoo/Kaypi) sin taxonomía deco previa |
| **O** | Outcome | Confirmación oportuna de disponibilidad; ≥90 % atributos obligatorios completos en piloto; reducción retrabajo en cotizaciones; exactitud inventario piloto ≥95 % (aspiración proxy sector); tiempo respuesta consulta stock <2 min en piloto |
| **C** | Context | Perú, Lima (San Isidro, Surco); retail decoración / textiles de interior importados; PYME importador-showroom con línea Contract; venta consultiva alta gama |
| **T** | Time / Type of study | **2026**; artículos, informes sectoriales, casos de implementación y tesis académicas sobre digitalización inventario textil/retail |
