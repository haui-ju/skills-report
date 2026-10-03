# Veredicto auditoría — ITD-V2

## Veredicto global

**GO_con_cambios**

## Detalle

Ver `theme-audit-debate.md`.

El tema es defendible como diagnóstico aplicado y diseño condicionado. Sus condiciones obligatorias son: validar el problema con evidencia primaria de Romantex, reducir el trabajo a una familia y un flujo, y tratar el asistente como una fase posterior y controlada, no como una implementación autónoma.

## Tema final

### Tema

**Digitalización del inventario y estandarización de atributos de producto textil mediante un asistente conversacional en lenguaje natural para la consulta de productos y la preparación de solicitudes de pedido en Romantex S.A.C.**

### Descripción

El proyecto examina si una familia piloto de productos textiles de Romantex puede consultarse de manera consistente en el catálogo, la disponibilidad y la atención comercial. A partir de evidencia primaria, propone un modelo mínimo y gobernado de atributos, fuentes, responsables y estados de disponibilidad. De forma condicionada, diseña un flujo conversacional para buscar y comparar productos, comunicar datos trazables y preparar solicitudes preliminares sujetas a validación humana. El objeto de estudio es la organización y su flujo comercial; no se plantea desarrollar un chatbot autónomo ni realizar una implementación empresarial.

### Problema identificado

La oferta pública de Romantex combina productos en stock, pedidos por catálogo, múltiples marcas, unidades como metro o rollo y atención residencial y Contract. Esta complejidad hace plausible la existencia de diferencias entre nombres, atributos, fuentes de inventario y respuestas comerciales; sin embargo, la existencia y magnitud de esa brecha no están demostradas. Por tanto, el problema interno se formula como una hipótesis verificable.

El diagnóstico comprobará si una familia piloto presenta inconsistencias, búsquedas cruzadas, datos incompletos o ambigüedad entre disponibilidad informada, reserva y pedido confirmado. La ficha pública permite conocer la identidad, la oferta y la presencia de la empresa, pero no prueba el AS-IS de sus procesos internos. El asistente solo sería pertinente si previamente se definen el modelo de datos, las fuentes y las responsabilidades correspondientes.

### Alcance

El trabajo se concentrará en una familia de productos y en un flujo acotado: consulta o comparación de producto → disponibilidad informada → solicitud preliminar → validación por asesor. El MVP inicial incluirá el mapa AS-IS, la selección justificada de la familia, una muestra trazable, un diccionario mínimo de atributos, reglas para tratar ausencias y conflictos, una matriz fuente–campo–responsable, un modelo TO-BE mínimo y un protocolo de validación.

Como fase condicionada, podrá especificarse una maqueta conversacional para la búsqueda, comparación y preparación de solicitudes. No se promete integración ni despliegue. Quedan fuera el ERP, WMS o PIM empresarial, la normalización total del catálogo, la sincronización en tiempo real no verificada, las recomendaciones estéticas autónomas, los precios, las reservas, los pagos y la confirmación automática de pedidos.

### Tipo de sujeto

empresa

### Ficha de empresa (para init-project → company.md)

**Identidad:** Romantex S.A.C. es una sociedad anónima cerrada peruana, con RUC 20293975036 e inicio de actividades registrado en octubre de 1995. La empresa se presenta corporativamente desde 1996 como especialista en telas para decoración, revestimientos para paredes y accesorios importados de alta calidad.

**Reseña histórica pública:** Los registros empresariales sitúan el inicio de actividades en 1995, mientras la narrativa corporativa utiliza 1996 como referencia de establecimiento y consolidación de la marca. Romantex comunica una evolución basada en showroom y stock para entrega inmediata, pedidos por catálogo de marcas internacionales, atención de diseñadores y una línea Contract para hoteles, restaurantes y espacios públicos. La cobertura especializada reciente documenta la renovación de imagen y showroom bajo el liderazgo público de Susana Balmaceda. Esta reseña es pública y no constituye evidencia del funcionamiento interno de sus procesos.

**Misión / visión / valores:** Romantex no publica una declaración formal completa de misión y visión en las fuentes consultadas. Su propuesta de valor comunicada enfatiza especialización y curaduría de productos importados, calidad, elegancia, atención personalizada, asesoría de diseñadores, actualización en tendencias, rigor técnico para proyectos Contract y mejora continua de operaciones y servicio.

**Oferta / sector relevante:** La empresa comercializa telas decorativas, de tapicería, cortinas y uso exterior; revestimientos para paredes; pasamanería, accesorios y cojines. Comunica productos en stock para entrega inmediata, pedidos por catálogo, soluciones Contract y atención personalizada de diseñadores de interiores. Opera públicamente en Av. Paz Soldán 185, San Isidro, y Av. El Polo 376, Surco, Lima.

**Evidencia_empresa:** suficiente para identidad, oferta, locales y propuesta pública; insuficiente para afirmar el AS-IS de inventario, catálogo, consultas, pedidos o sistemas internos.

**Fuentes de empresa:**

- Romantex — Empresa: https://www.romantex.com.pe/empresa
- Romantex — Company: https://www.romantex.com.pe/company
- Romantex — Inicio: https://romantex.com.pe/
- Romantex — Contacto: https://www.romantex.com.pe/contacto
- UniversidadPeru — Romantex S.A.C.: https://www.universidadperu.com/empresas/romantex.php
- Ubicania — Romantex S.A.C.: https://ubicania.com/empresas/romantex-s-a-c_id_143809909583B417
- Dossier de Arquitectura — nuevo showroom: https://dossierdearquitectura.com/romantex-nos-presenta-su-nuevo-showroom/
- Ellas Internacional — renovación y liderazgo: https://www.ellasinternacional.com/romantex-renueva-su-esencia-diseno-vanguardia-y-vision-innovadora-al-frente-del-sector-deco-en-peru/

## MVP entregables

### MVP de arranque (recomendado al equipo)

**MVP 1 — Diagnóstico y modelo mínimo de datos para una familia piloto.** Gana el debate porque permite verificar si existe una brecha real y si hay condiciones de gobernanza antes de diseñar una interfaz conversacional. Si no se identifican fuentes, responsables y atributos suficientemente completos, el resultado válido será un diagnóstico de preparación de datos, no un chatbot.

### Secuencia

| MVP | Objetivo | Entregables | Criterio de éxito | Estado |
|-----|----------|-------------|-------------------|--------|
| 1 | Verificar el AS-IS y definir el modelo mínimo gobernado para una familia | Mapa AS-IS; criterio de selección; muestra trazable; diccionario de atributos; reglas de identificación, ausencia y conflicto; matriz fuente–campo–responsable; modelo TO-BE mínimo de producto, variante y disponibilidad; protocolo y roadmap condicionado | Cada atributo obligatorio tiene fuente, responsable y tratamiento definido; los registros conservan trazabilidad; la familia y el flujo quedan confirmados o refutados por evidencia | se trabaja ahora |
| 2 | Diseñar una asistencia conversacional limitada sobre datos validados | Maqueta o especificación funcional; intenciones de búsqueda, comparación, disponibilidad y solicitud preliminar; fuente y fecha del dato; advertencias; derivación humana; casos de prueba anonimizados o ficticios | El flujo no presenta como confirmado un dato sin respaldo, distingue disponibilidad de solicitud y deriva conflictos o autorizaciones a un asesor | condicionado a MVP 1 |
| 3 | Evaluar una prueba controlada y decidir continuidad | Protocolo con usuarios internos; registro de incidencias; comparación entre respuesta y validación del responsable; decisión de continuar, ajustar o detener | Las respuestas y solicitudes pueden verificarse; las excepciones quedan trazadas; el esfuerzo de adopción no supera el beneficio observado | opcional posterior |

### Fuera de secuencia / descartado

- chatbot autónomo o canal productivo de ventas;
- ERP, WMS o PIM empresarial;
- sincronización de inventario en tiempo real sin arquitectura verificada;
- normalización de todo el catálogo histórico;
- recomendación estética autónoma;
- precios, descuentos, reservas, pagos o confirmación automática de pedidos;
- afirmaciones de ROI, aumento de ventas o reducción de tiempos sin línea base y piloto;
- sustitución de vendedores, almacén o asesoría especializada.

## Tesis de valor (inversor)

El informe no propone vender un chatbot, sino convertir una hipótesis operativa en una decisión verificable sobre datos, gobernanza y asistencia comercial. Su valor inmediato consiste en delimitar el problema, identificar fuentes y responsables, establecer reglas de disponibilidad y determinar si resulta justificable probar una interfaz conversacional en una familia piloto.

Una implementación posterior podría reducir búsquedas repetitivas, solicitudes incompletas y el riesgo de comunicar una disponibilidad incorrecta. Sin embargo, esos beneficios son hipótesis que requieren línea base, piloto, adopción y mantenimiento del maestro; no deben presentarse como retorno de inversión ni como resultados actuales. Los indicadores sugeridos son completitud de atributos, tiempo mediano de búsqueda, número de fuentes consultadas, solicitudes completas, discrepancias entre disponibilidad informada y validada, correcciones humanas y derivaciones apropiadas.

## Marco PICOCT (para bibliography)

| Componente | Definición | Criterios / descripción del caso |
| :---: | :--- | :--- |
| **P** | Population / Problem | Romantex S.A.C. y los roles que participan en una familia piloto de productos textiles: ventas, almacén, catálogo y validación comercial; hipótesis de desalineación entre atributos, fuentes de disponibilidad y preparación de solicitudes. |
| **I** | Intervention | Diagnóstico AS-IS y diseño de un modelo mínimo gobernado de atributos, producto, variante y disponibilidad, con una asistencia conversacional condicionada para consulta y preparación de solicitudes preliminares con validación humana. |
| **C** | Comparison | Práctica actual que se observe en Romantex: consulta manual, fuentes separadas, catálogos, hojas de cálculo, mensajería u otros registros; si no se confirma, se documentará como hipótesis y no como hecho. |
| **O** | Outcome | Completitud y trazabilidad de atributos; claridad de unidad y variante; disponibilidad con fuente, fecha y estado; solicitudes preliminares completas; discrepancias y derivaciones; tiempo de búsqueda solo si se establece una línea base. |
| **C** | Context | Perú, Lima; PYME importadora y showroom de textiles de decoración; catálogo multimarca; productos en stock y por catálogo; atención residencial, de diseñadores y Contract. |
| **T** | Time / Type of study | **2026**; artículos, informes, casos de implementación y tesis académicas sobre calidad de datos de producto, inventario textil, gobernanza de datos, asistencia conversacional y pedidos con validación humana. |

## Listo para

`init-project` (espejar tema final, ficha, MVP y Marco PICOCT en `profile.md`) → `init-project-mvp mvp-1` → `bibliography-picoct`.
