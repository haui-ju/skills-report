# RAT — MVP 1

## 1. Supuestos priorizados

La fuente de verdad de supuestos riesgosos para el MVP es este archivo. Todos quedan `pendiente_campo` hasta ser contrastados por una contraparte de Romantex o por evidencia documental externa al estudiante.

### R1 — La muestra puede normalizarse sin perder identidad

- ID: R1
- Supuesto: En dos o tres familias priorizadas, cada variante puede relacionarse con una referencia de proveedor, una familia, una unidad de venta y una regla de normalización sin borrar el valor original.
- Etiqueta actual: pendiente_campo
- Impacto si falso: alto
- Incertidumbre: alta
- Falsación:
  - observar: revisar 20 registros o fichas y contrastarlos con etiqueta, catálogo, documento de proveedor o fuente actual; registrar campos faltantes, duplicados y conflictos de unidad.
  - con_quien: responsable de catálogo o comercial y responsable de almacén.
  - umbral: si al menos 18 de 20 registros tienen referencia, familia, unidad y fuente verificable, R1 queda apoyado; con menos de 18, R1 queda falsado para la muestra.
  - ventana: una sesión de revisión de 60–90 minutos y una segunda comprobación de los casos conflictivos dentro de la misma semana.
- Dueño_entregable: estudiante
- Contraparte_campo: responsable de catálogo/comercial y responsable de almacén
- Origen: DT + Lean + profile

### R2 — El SKU propuesto permite recuperar una variante sin duplicidad

- ID: R2
- Supuesto: Un SKU interno basado en familia, referencia de proveedor, variante y unidad permite que comercial y almacén lleguen al mismo registro de la muestra.
- Etiqueta actual: pendiente_campo
- Impacto si falso: alto
- Incertidumbre: alta
- Falsación:
  - observar: entregar 10 búsquedas con nombre, referencia o muestra y comparar el resultado obtenido por dos usuarios usando la ficha y el SKU propuesto.
  - con_quien: un asesor comercial y un responsable de almacén.
  - umbral: al menos 8 de 10 búsquedas deben llegar al mismo registro sin duplicidad y sin consultar verbalmente al estudiante; de lo contrario, R2 queda falsado.
  - ventana: una sesión de prueba de 30 minutos posterior a la carga de la muestra.
- Dueño_entregable: estudiante
- Contraparte_campo: asesor comercial y responsable de almacén
- Origen: DT + Lean + profile

### R3 — Existe capacidad de adopción y ownership

- ID: R3
- Supuesto: Un rol interno puede validar los atributos y mantener la fecha, el estado y las excepciones de cada ficha sin depender del estudiante.
- Etiqueta actual: pendiente_campo
- Impacto si falso: alto
- Incertidumbre: alta
- Falsación:
  - observar: pedir a un responsable interno que complete o revise 10 fichas con la plantilla, asigne estado y deje una observación cuando falte un dato.
  - con_quien: responsable de catálogo, comercial o almacén designado por Romantex.
  - umbral: 10 de 10 fichas deben quedar con responsable, fecha y estado; si ninguna persona acepta la responsabilidad o más de 2 fichas quedan sin dueño, R3 queda falsado.
  - ventana: una sesión de 45 minutos y confirmación de la responsabilidad al cierre de la semana.
- Dueño_entregable: estudiante
- Contraparte_campo: responsable interno designado
- Origen: DT + Lean + profile

### R4 — La calidad del dato debe preceder a la integración

- ID: R4
- Supuesto: La muestra contiene suficientes diferencias de nomenclatura, unidad o completitud como para justificar reglas de calidad antes de conectar canales.
- Etiqueta actual: pendiente_campo
- Impacto si falso: medio
- Incertidumbre: media
- Falsación:
  - observar: comparar 20 registros entre la fuente actual y la ficha piloto, clasificando completitud, duplicidad, consistencia de unidad y trazabilidad.
  - con_quien: docente/tutor y contraparte de catálogo o almacén; la contraparte valida la fuente, el docente revisa el conteo.
  - umbral: si al menos 4 de 20 registros presentan una diferencia verificable o un campo obligatorio ausente, R4 queda apoyado; con menos de 4, se reduce la prioridad de un MVP de calidad previo a integración.
  - ventana: una revisión de muestra y validación de resultados dentro de una semana.
- Dueño_entregable: estudiante
- Contraparte_campo: responsable de catálogo/almacén; docente como tercero de revisión
- Origen: FODA-Amenaza + Lean + profile

## Cola no RAT

- Disponibilidad por ubicación y estado reservado: se prueba en el MVP 2 después de estabilizar atributos y SKU.
- Utilidad de indicadores de rotación: requiere datos históricos consistentes; queda para MVP 3.
- Elección de herramienta PIM/ERP: se difiere hasta conocer calidad, volumen y reglas internas.

## Regla de decisión

No se recomendará una integración técnica como siguiente inversión si R1 o R3 quedan falsados. Si R2 falla, se simplificará el esquema de búsqueda y se conservarán alias; si R4 falla, se reducirá el MVP a gobernanza y documentación antes de ampliar el alcance.
