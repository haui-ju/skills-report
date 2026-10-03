# Brainstorm de auditoría — ITD-V2

## CONTEXTO

- dominio: retail, decoración y textiles de interior
- pais_region: Perú — Lima
- fase_entregable: diagnóstico y diseño de propuesta
- restricciones: empresa real; evidencia pública; sin acceso presumido a sistemas internos; alcance acotado a una PYME; no pretender ERP/WMS enterprise ni un asistente autónomo
- modo: una_alternativa
- tipo_sujeto: empresa
- empresa: Romantex S.A.C.

## Tema de entrada

**Tema:** Digitalización del inventario y estandarización de atributos de producto textil, con un asistente conversacional en lenguaje natural para la consulta de productos y toma de pedidos en Romantex S.A.C.

## Acta (`brainstorm-theme`)

### Supuestos de contexto

Romantex S.A.C. es un importador y showroom multimarca de telas decorativas, revestimientos murales, pasamanería y accesorios para interiorismo. Su propuesta pública combina stock físico, pedidos por catálogo, línea Contract y atención consultiva en dos locales limeños. No se presume qué sistemas, volúmenes, procesos, niveles de stock o problemas internos existen: deben verificarse mediante entrevistas, observación y revisión de muestras de datos.

El asistente se entiende como una interfaz de consulta y asistencia sobre datos estructurados, no como sustituto del personal comercial ni como autoridad autónoma para confirmar stock, precios, reservas o pedidos.

### Ángulos retenidos

#### 1. Fuente maestra de producto e inventario

El primer ángulo estudia cómo definir un lenguaje común para productos y variantes multimarca:

- marca, referencia y colección;
- color, composición, textura y ancho;
- aplicación residencial o Contract;
- unidad de venta y medición, como metro, rollo, pieza o muestra;
- ubicación, saldo, reserva y fecha de actualización;
- estado comercial: disponible, reservado, por confirmar, bajo pedido, catálogo o discontinuado.

La hipótesis es que la heterogeneidad de nomenclaturas y unidades puede dificultar la consulta comercial, pero debe comprobarse. El proyecto no debe afirmar que existe una falla cuantificada antes de estudiar el flujo real.

#### 2. Asistente conversacional para consulta y recomendación

El segundo ángulo estudia una interfaz en lenguaje natural que permita:

- buscar productos por atributos registrados;
- responder preguntas sobre composición, ancho, color, uso o unidad;
- comparar alternativas;
- orientar una recomendación cuando existan reglas y datos suficientes;
- informar disponibilidad con fuente y fecha;
- derivar al personal cuando haya ambigüedad, información incompleta, necesidad de muestra o criterio técnico.

Debe distinguirse entre consulta informativa, búsqueda filtrada y recomendación. Una recomendación no debe presentarse como garantía de idoneidad técnica ni basarse en atributos no documentados.

#### 3. Preparación controlada de pedidos

El tercer ángulo estudia la transición entre conversación, solicitud de cotización y pedido:

1. descubrir la necesidad;
2. identificar producto o alternativas;
3. comprobar variante, unidad y cantidad;
4. consultar disponibilidad;
5. recopilar datos del cliente y del proyecto;
6. generar una solicitud o pedido preliminar;
7. derivar a un asesor para validar stock, precio, condiciones y entrega.

“Registrar una intención de compra” no equivale a “confirmar un pedido”. La solución debe separar producto encontrado, producto recomendado, stock informado, solicitud preliminar y pedido confirmado.

### Hipótesis verificables

1. Los usuarios internos emplean nombres o atributos diferentes para describir productos equivalentes.
2. La información necesaria para responder consultas está distribuida entre catálogo, personal, almacén, showrooms y otros registros.
3. Las consultas pueden clasificarse en informativas, de búsqueda, de recomendación, de disponibilidad y de pedido.
4. La disponibilidad exige distinguir ubicación, reservas, unidad de venta y fecha de actualización.
5. Una taxonomía mínima puede reducir búsquedas manuales o respuestas inconsistentes.
6. Un asistente con límites explícitos puede apoyar al equipo sin sustituir la asesoría especializada.
7. La toma de pedidos requiere validaciones adicionales que no necesita una consulta informativa.
8. Los productos Contract pueden requerir atributos, cotizaciones o aprobaciones diferentes a los pedidos residenciales.
9. La calidad de las respuestas depende más de la completitud y actualización de los datos que de la sofisticación del modelo conversacional.
10. Es posible seleccionar una o dos familias y un flujo piloto sin representar todo el catálogo.

### Usuarios y necesidades

- **Clientes residenciales:** encontrar productos por estilo, ambiente, color o uso y solicitar atención.
- **Diseñadores e interioristas:** comparar alternativas, revisar atributos técnicos, solicitar muestras y consultar disponibilidad.
- **Clientes Contract:** identificar opciones para proyectos, revisar requerimientos y solicitar cotización.
- **Vendedores y asesores:** responder con información uniforme y controlar compromisos comerciales.
- **Personal de almacén:** identificar referencias, unidades, ubicaciones y saldos según la información disponible.
- **Responsables de catálogo o compras:** corregir atributos, incorporar referencias y resolver equivalencias.
- **Supervisión:** revisar solicitudes, reservas, precios y autorizaciones.

### Dependencias

1. La taxonomía permite identificar productos y variantes.
2. El inventario requiere reglas sobre ubicación, reservas, unidad y frescura del dato.
3. El asistente solo debe responder automáticamente con datos que tengan fuente y estado de actualización.
4. La conversación puede preparar un pedido, pero la confirmación depende de validaciones comerciales y operativas.
5. La gobernanza y la designación de responsables determinan la sostenibilidad del modelo.
6. La promesa de tiempo real solo sería válida después de conocer sistemas, interfaces, frecuencia de sincronización y manejo de fallos.

### Datos necesarios para validar el diagnóstico

- catálogo y variantes de las familias seleccionadas;
- marcas, colecciones, referencias y equivalencias;
- atributos usados actualmente;
- unidades de venta y medición;
- ubicación, reservas, muestras y saldos;
- fuentes actuales: hojas de cálculo, sistema comercial, web, mensajería o registros físicos;
- consultas frecuentes y flujo de cotización;
- reglas de precios, mínimos y condiciones Contract, si son accesibles;
- responsables de validar producto, stock y pedido;
- ejemplos de errores o retrabajo, sin asumir su frecuencia.

### Límites del asistente

El asistente podría buscar, comparar, responder atributos documentados, informar disponibilidad con advertencias y preparar solicitudes. No debería inventar productos, stock, precios, plazos o certificaciones; confirmar pedidos, descuentos o reservas; resolver conflictos entre registros; ni sustituir la revisión de muestras o la validación de un asesor.

### Entregables posibles

- mapa AS-IS de producto, inventario, consulta y pedido;
- taxonomía mínima viable y diccionario de atributos;
- modelo conceptual de producto, variante, ubicación, stock, reserva y pedido;
- matriz de fuentes y responsables;
- diseño TO-BE del flujo conversacional;
- guion de intenciones, respuestas, excepciones y derivaciones;
- reglas de trazabilidad y validación humana;
- prototipo conceptual o especificación funcional;
- piloto acotado y roadmap condicionado a los hallazgos.

### Criterios de éxito propuestos

- atributos obligatorios definidos para las familias piloto;
- cada respuesta automática vinculada a una fuente identificable;
- distinción entre stock confirmado, stock por verificar y producto no disponible;
- solicitudes de pedido con producto, variante, unidad, cantidad y datos mínimos;
- derivación explícita de casos ambiguos o que requieren autorización;
- responsables y frecuencia de actualización identificados;
- métricas formuladas como objetivos a validar: completitud de atributos, tiempo de respuesta, coincidencia entre stock informado y validado, consultas derivadas y solicitudes completas.

### Riesgos y preguntas críticas

- datos incompletos o desactualizados;
- ambigüedad entre metros, rollos, muestras y piezas;
- diferencias entre marcas y equivalencias no comprobadas;
- recomendaciones subjetivas difíciles de formalizar;
- pedidos Contract con requisitos adicionales;
- exposición de precios o datos de clientes;
- falta de un responsable de gobernanza;
- expectativas de implementar un chatbot productivo sin acceso a sistemas;
- riesgo de convertir un diagnóstico acotado en un ERP, PIM y canal de ventas completo.

### Descartados

- chatbot autónomo que cierre ventas;
- promesa de inventario en tiempo real sin verificar la arquitectura;
- digitalización completa del histórico;
- ERP, WMS o PIM empresarial como entregable obligatorio;
- predicción de demanda sin datos históricos confiables;
- recomendación basada solo en lenguaje natural;
- medición de impacto comercial definitivo sin línea base ni piloto.

### Síntesis

El ángulo más defendible es la dependencia entre gobierno de datos, inventario confiable y asistencia conversacional. El flujo demostrable recomendado es:

**búsqueda de productos → comparación o recomendación → consulta de disponibilidad → solicitud preliminar → validación por asesor.**

El asistente es una capa de acceso y apoyo; el núcleo del proyecto sigue siendo una base maestra de producto e inventario con reglas explícitas.
