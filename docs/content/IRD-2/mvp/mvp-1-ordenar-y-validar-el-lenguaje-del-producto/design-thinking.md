# Design Thinking — MVP 1

## 1. Empatizar

### Roles priorizados

| Rol                                       | Necesidad que se investigara                                                                             | Evidencia disponible                                                                                                                        |
| ----------------------------------------- | -------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- |
| Asesor comercial de showroom              | Encontrar una ficha de producto y responder una consulta de disponibilidad con una unidad de venta clara | El sitio oficial publica showrooms y atencion a clientes residenciales y comerciales; el detalle de la rutina interna es `pendiente_campo`. |
| Responsable de almacén                    | Identificar una variante, ubicarla y mantener sus atributos y existencias actualizados                   | El contexto del proyecto menciona inventario fisico y catalogo amplio; registros y movimientos internos: `pendiente_campo`.                 |
| Responsable de catalogo o canal digital   | Publicar informacion consistente de telas, revestimientos y accesorios sin duplicar o perder atributos   | El sitio oficial publica catalogo y solicitud de muestras; proceso de alta y sincronizacion: `pendiente_campo`.                             |
| Responsable de proyectos Contract         | Comparar alternativas por aplicacion, composicion, medidas y disponibilidad para una cotizacion          | La empresa publica una linea Contract; criterios de cotizacion y reserva: `pendiente_campo`.                                                |
| Cliente diseñador o comprador de proyecto | Recibir una descripcion comprensible y confirmar si una variante sirve para su proyecto                  | Necesidad inferida del modelo de venta consultiva; validar mediante observacion de consultas reales.                                        |

### Plan de observacion de Fase 0

1. Observar una consulta real de una variante desde showroom o canal comercial hasta la respuesta.
2. Solicitar una muestra acotada de fichas, catalogos, registros de stock y movimientos de dos o tres familias.
3. Registrar las palabras usadas por cada rol para familia, color, composicion, ancho, unidad y disponibilidad.
4. Preguntar en el momento: “cuentame la ultima vez que buscaste esta variante”, “donde verificaste el stock” y “que hiciste cuando faltaba un atributo”.
5. No registrar nombres de clientes ni datos comerciales innecesarios; conservar solo evidencias de proceso y calidad de datos.

### Mapa de empatia

| Rol / perspectiva   | Dice                                                                    | Piensa                                                                      | Hace                                                  | Siente                                                         |
| ------------------- | ----------------------------------------------------------------------- | --------------------------------------------------------------------------- | ----------------------------------------------------- | -------------------------------------------------------------- |
| Comercial           | Hipótesis: “Necesito confirmar la variante antes de cotizar”.           | Hipótesis: puede depender de una ficha, otra persona o una consulta manual. | Busca por marca, nombre, color, muestra o referencia. | Incertidumbre cuando la unidad o disponibilidad no son claras. |
| Almacén             | Hipótesis: “El producto puede estar identificado con otra descripción”. | Hipótesis: la ubicación y el estado deben coincidir con el registro.        | Revisa etiquetas, estantes, registros o conteos.      | Fricción si debe corregir datos mientras atiende pedidos.      |
| Cliente de proyecto | Hipótesis: “Necesito comparar y saber si alcanza para mi proyecto”.     | Hipótesis: una medida o composición ambigua puede cambiar la decisión.      | Pide muestras, especificaciones y disponibilidad.     | Riesgo de retraso si la respuesta requiere varias consultas.   |

No se inventan citas ni métricas. Las afirmaciones anteriores son `hipótesis` hasta la observación de campo.

## 2. Definir

### POV

El equipo comercial y de almacén necesita una forma común de identificar y describir las variantes textiles porque la venta consultiva depende de responder con rapidez sobre atributos, unidad de venta y estado de disponibilidad sin perder la referencia original del proveedor.

### HMW primario

**¿Cómo podríamos ordenar y validar los atributos de dos o tres familias textiles para que comercial y almacén consulten la misma variante, unidad de venta y fecha de actualización antes de cotizar?**

### HMW secundarios

- ¿Cómo podríamos conservar la descripción original del proveedor y, a la vez, aplicar una nomenclatura interna consistente?
- ¿Cómo podríamos detectar una ficha incompleta o duplicada antes de publicarla o usarla en una cotización?
- ¿Cómo podríamos dejar visible quién validó una normalización y cuándo debe revisarse?

### Criterio de foco

El MVP 1 no implementa una plataforma. Entrega un lenguaje común y un modelo maestro validable sobre una muestra; la consulta multicanal y los indicadores se dejan para los MVP posteriores del profile.

## 3. Idear

| Idea                                                             | Valor para el problema                                     | Esfuerzo inicial | Decisión                                      |
| ---------------------------------------------------------------- | ---------------------------------------------------------- | ---------------: | --------------------------------------------- |
| Ficha maestra de producto con valor original y valor normalizado | Hace visibles los atributos obligatorios y las excepciones |             Bajo | Priorizar                                     |
| Código SKU por familia, proveedor, variante y unidad             | Permite buscar y evitar duplicidades                       |            Medio | Priorizar como propuesta, validar con muestra |
| Catálogo visual con filtros por atributos                        | Facilita consultas de showroom                             |            Medio | Diseñar como salida posterior de la ficha     |
| Formulario de alta con validaciones                              | Reduce registros incompletos                               |            Medio | Dejar especificado, no implementar ahora      |
| Integración automática con web y stock                           | Reduce doble registro si los datos ya son confiables       |             Alto | Fuera del MVP 1                               |

### Idea seleccionada

Un **registro maestro piloto** para dos o tres familias, construido con una plantilla de ficha y un diccionario de datos. Cada fila conservará la referencia de proveedor, agregará atributos normalizados, indicará unidad de venta y ubicación si existe el dato, y mostrará estado de validación y responsable.

## 4. Prototipar

### Artefactos del prototipo

1. **Diccionario de datos:** nombre del atributo, definición, formato, obligatoriedad, ejemplo, fuente, responsable y regla de validación.
2. **Ficha maestra:** familia, marca/proveedor, referencia original, SKU interno propuesto, nombre comercial, composición, color, ancho, unidad de venta, aplicación, mantenimiento, ubicación, estado de stock, fecha de actualización, responsable y observaciones.
3. **Matriz de normalización:** valor original, valor normalizado, regla aplicada, excepción, evidencia de respaldo y aprobación.
4. **Matriz de calidad:** completitud, duplicidad, consistencia de unidad, trazabilidad y fecha de actualización.

### Flujo de uso del prototipo

1. El responsable selecciona una muestra de una familia priorizada.
2. Copia la referencia original sin modificarla.
3. Completa los atributos obligatorios y marca los que no están disponibles.
4. Propone el SKU interno y la unidad de venta.
5. Registra la regla de normalización y la excepción, si aplica.
6. El responsable de comercial o almacén valida la ficha.
7. La ficha queda con estado `validada`, `observada` o `pendiente_campo`.

### Restricciones del prototipo

- No sustituye el sistema actual ni modifica stock real.
- No declara disponibilidad cuando no existe registro verificable.
- No fuerza equivalencias entre materiales o unidades distintas.
- No se extiende a todo el histórico ni a todas las marcas.

## 5. Test — después de RAT

El test se ejecuta sobre la misma muestra usada para los RAT. El evaluador entrega una ficha sin explicar el orden de los campos y observa si el usuario puede identificar la variante, su unidad y su estado.

| RAT | Actividad de test                                                                           | Umbral                                                                                                                           | Resultado esperado                                         |
| --- | ------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------- |
| R1  | Comercial y almacén comparan 20 registros con ficha, fuente original y evidencia disponible | Al menos 18/20 registros tienen familia, referencia, unidad y estado de validación identificables sin completar datos de memoria | Si no se alcanza, revisar taxonomía y obligatoriedad       |
| R2  | Dos usuarios buscan 10 variantes usando la ficha y el SKU propuesto                         | Al menos 8/10 búsquedas llegan al mismo registro sin duplicidad                                                                  | Si no se alcanza, simplificar el código y registrar alias  |
| R3  | Un usuario completa 10 fichas siguiendo la plantilla sin guía oral                          | Al menos 8/10 fichas quedan completas en atributos obligatorios y con responsable                                                | Si no se alcanza, ajustar formulario y capacitación        |
| R4  | El responsable revisa 10 normalizaciones                                                    | 10/10 conservan valor original, regla aplicada y estado de aprobación                                                            | Si no se alcanza, bloquear publicación de la normalización |

### Preguntas al equipo

- ¿Qué dos o tres familias se pueden entregar con una muestra real sin exponer información comercial sensible?
- ¿Qué rol tiene autoridad para aprobar una normalización de nombre, medida o unidad de venta?
- ¿Qué fuente externa al equipo del proyecto servirá para contrastar cada registro: sistema actual, etiqueta, conteo, catálogo o documento de proveedor?
- ¿Qué dato mínimo permite distinguir disponible, reservado, agotado y pendiente de verificación?
- ¿Qué hallazgo obligaría a reabrir Empatizar o Definir en una iteración posterior?
