# Auditoría de tema — ITD-V2

## CONTEXTO

- dominio: retail, decoración y textiles de interior
- pais_region: Perú — Lima, San Isidro y Surco
- fase_entregable: diagnóstico y diseño de propuesta
- restricciones: empresa real; evidencia pública; sin acceso presumido a sistemas internos; alcance acotado a una PYME; no pretender ERP/WMS enterprise ni un asistente autónomo
- modo: una_alternativa
- tipo_sujeto: empresa
- empresa: Romantex S.A.C.

## Tema propuesto (entrada)

**Tema:** Digitalización del inventario y estandarización de atributos de producto textil, con un asistente conversacional en lenguaje natural para la consulta de productos y toma de pedidos en Romantex S.A.C.

**Descripción:** ROMANTEX S.A.C., fundada en Lima en 1995 y registrada con RUC 20293975036, es una sociedad anónima cerrada peruana que comercializa telas decorativas, revestimientos murales, pasamanería y accesorios de interiorismo de alta gama. Opera como importador y casa de showroom, con sede en Av. Paz Soldán 185 (San Isidro), segundo local en Av. El Polo 376 (Surco) y presencia digital en romantex.com.pe. El proyecto examina cómo se articulan inventario físico, catálogo multimarca y canales comerciales para proponer una fuente única de verdad del producto textil. La organización, no el piloto, es el sujeto de este capítulo.

**Problema identificado:** La heterogeneidad potencial de atributos, nomenclaturas, unidades de venta y fuentes de información puede dificultar la consulta de productos, la confirmación de disponibilidad y la preparación de pedidos. Esta afirmación es una hipótesis de diagnóstico: no se presenta como un hecho cuantificado ni como un AS-IS interno demostrado. La investigación deberá contrastarla mediante entrevistas, observación y revisión de muestras de catálogo, inventario y flujo comercial.

**Alcance:** El tema comprende el diseño de una taxonomía mínima de productos textiles, un modelo conceptual de inventario y disponibilidad, y un asistente conversacional que permita consultar productos, comparar alternativas y preparar solicitudes de pedido sujetas a validación humana. Se priorizarán una o dos familias y un flujo acotado; quedan fuera la implementación de ERP/WMS/PIM empresarial, la promesa de inventario en tiempo real sin verificar integraciones, la confirmación autónoma de pedidos, pagos, reservas o descuentos, y la normalización de todo el catálogo histórico.

## Ficha de empresa (investigación)

**Identidad:** ROMANTEX S.A.C., RUC 20293975036, sociedad anónima cerrada peruana, activa desde octubre de 1995 e importadora registrada. Su actividad pública corresponde a la comercialización especializada de telas decorativas, tapicería, revestimientos murales y accesorios de interiorismo.

**Reseña histórica (pública):** Los registros empresariales sitúan el inicio de actividades en octubre de 1995; la narrativa corporativa presenta a Romantex desde 1996 como especialista en telas para decoración, revestimientos para paredes y accesorios importados de alta calidad. La empresa comunica una evolución desde el showroom y el stock para entrega inmediata hacia un modelo que también incluye pedidos por catálogo, atención de diseñadores y una línea Contract para hoteles, restaurantes y espacios públicos. La cobertura especializada reciente describe renovación de imagen y showrooms bajo el liderazgo público de Susana Balmaceda. No se infiere de esta historia ningún proceso operativo interno.

**Misión / visión / valores:** Romantex no publica una declaración formal completa de misión y visión en la fuente corporativa consultada. De su comunicación pública se desprenden como ejes: especialización y curaduría de productos importados, calidad, elegancia, atención personalizada, asesoría de diseñadores, actualización en tendencias, rigor técnico para proyectos Contract y mejora continua de operaciones y servicio. Estos ejes se tratan como propuesta de valor comunicada, no como declaraciones institucionales textuales.

**Oferta / sector relevante:** La empresa comunica:

- telas decorativas, de tapicería, cortinas y uso exterior;
- revestimientos para paredes;
- pasamanería, accesorios y cojines;
- productos en stock para entrega inmediata;
- pedidos por catálogo de marcas internacionales;
- soluciones Contract para hoteles, restaurantes y espacios públicos;
- atención personalizada de diseñadores de interiores;
- dos showrooms en San Isidro y Surco.

**Presencia geográfica:** Av. Paz Soldán 185, San Isidro, Lima, y Av. El Polo 376, Surco, Lima, según el sitio oficial.

**Evidencia_empresa:** suficiente para identidad, oferta, locales y propuesta pública; insuficiente para afirmar el AS-IS de inventario, catálogo, pedidos o sistemas internos.

**Fuentes de empresa:**

- Romantex — Empresa: https://www.romantex.com.pe/empresa
- Romantex — Company: https://www.romantex.com.pe/company
- Romantex — Inicio: https://romantex.com.pe/
- Romantex — Contacto: https://www.romantex.com.pe/contacto
- UniversidadPeru — Romantex S.A.C.: https://www.universidadperu.com/empresas/romantex.php
- Ubicania — Romantex S.A.C.: https://ubicania.com/empresas/romantex-s-a-c_id_143809909583B417
- Dossier de Arquitectura — nuevo showroom: https://dossierdearquitectura.com/romantex-nos-presenta-su-nuevo-showroom/
- Ellas Internacional — renovación y liderazgo: https://www.ellasinternacional.com/romantex-renueva-su-esencia-diseno-vanguardia-y-vision-innovadora-al-frente-del-sector-deco-en-peru/

## Brainstorm

Acta: `theme-audit-brainstorm.md`.

Ángulos retenidos:

1. fuente maestra de producto e inventario;
2. asistente conversacional para consulta y recomendación;
3. preparación controlada de pedidos con validación humana.

La relación central es:

**atributos maestros → inventario y disponibilidad → consulta conversacional → solicitud de pedido → validación comercial.**

## Benchmarking (`benchmark-theme`)

### Casos

1. **Andover Fabrics + BigCommerce + Acumatica** — directo, distribuidor textil B2B. Centraliza productos, atributos, inventario, precios y pedidos. Es comparable en unidades y catálogo textil, pero su plataforma empresarial excede el alcance de Romantex.
   - Fuente: https://www.bigcommerce.com/case-study/andover-fabrics/
   - Adaptación: atributos obligatorios por familia, unidad de venta, estados de disponibilidad y reglas de pedido sin exigir una plataforma equivalente.

2. **Aranda Textiles + Stock2Shop + Sage 300cloud** — directo, fabricante/distribuidor textil. Separa datos operativos de inventario, precios y clientes de datos enriquecidos como categorías, imágenes y descripciones.
   - Fuente: https://www.stock2shop.com/case-studies/aranda/
   - Adaptación: fuente maestra y capa de enriquecimiento consultivo para marca, colección, textura, aplicación, composición y reglas comerciales.

3. **West Marine + Skipper** — proxy directo de retail especializado. Muestra una interfaz conversacional capaz de responder consultas abiertas y transferir conocimiento de especialistas al canal digital.
   - Fuente: https://www.salesforce.com/blog/west-marine-customer-story/
   - Adaptación: búsqueda y recomendación respaldadas por catálogo; derivación a asesor cuando falte información o exista una decisión técnica.

4. **Boni / Bow Chat** — proxy de captura conversacional de pedidos. Convierte mensajes y pedidos informales en borradores estructurados con revisión humana antes de confirmar.
   - Fuente: https://bow.chat/customers/ai-ordering-food-distribution
   - Adaptación: solicitud preliminar con producto, código, variante, unidad, cantidad, disponibilidad y observaciones; confirmación final por un asesor Romantex.

### Mini-matriz

| Capacidad / eje | Andover | Aranda | West Marine | Boni / Bow Chat | Relevancia Romantex |
|---|---|---|---|---|---|
| Catálogo estructurado | presente | presente | presente | parcial | alta |
| Atributos y enriquecimiento | presente | presente | parcial | parcial | alta |
| Inventario y disponibilidad | presente | presente | parcial | presente | alta |
| Consulta en lenguaje natural | ausente | ausente | presente | presente | alta |
| Captura conversacional de pedido | parcial | portal/representante | parcial | presente | alta |
| Validación o escalamiento humano | no documentado | parcial | no documentado | presente | alta |

### Qué adaptar

- taxonomía común para telas, revestimientos y productos Contract;
- separación entre código, variante, atributos enriquecidos, precio, unidad y stock;
- alias comerciales y vocabulario de clientes y vendedores;
- distinción entre consulta, recomendación, cotización, solicitud preliminar y pedido confirmado;
- reglas de derivación para stock incierto, productos por catálogo, pedidos Contract, compras por volumen y diferencias de lote;
- trazabilidad de la fuente, fecha y responsable de cada respuesta o confirmación.

### Diferenciador posible

Un asistente consultivo específico para textiles de decoración que combine atributos normalizados, disponibilidad con nivel de certeza y conocimiento de showroom, pero que prepare pedidos para validación humana. El valor no estaría en añadir un chatbot genérico, sino en hacer reproducible y trazable parte del conocimiento comercial de Romantex.

### Límites de la evidencia

La evidencia benchmark es suficiente, con límites. Los casos provienen principalmente de proveedores tecnológicos o integradores y demuestran patrones de solución, no resultados independientes en Romantex ni en el mercado peruano. No prueban que el asistente pueda interpretar correctamente colores físicos, medidas complejas, lotes, muestras o requisitos Contract sin datos locales y supervisión.

**Evidencia:** suficiente con límites.

## Tema afinado (pre-polish)

**Tema:** Digitalización del inventario y estandarización de atributos de producto textil mediante un asistente conversacional en lenguaje natural para la consulta de productos y la preparación de pedidos en Romantex S.A.C.

**Descripción:** El proyecto analiza cómo Romantex S.A.C. podría articular el inventario físico de sus showrooms y almacén, el catálogo multimarca y la atención comercial mediante una fuente única de verdad del producto textil. Sobre esa base, propone el diseño de un asistente conversacional capaz de buscar y comparar productos, responder atributos documentados, orientar consultas de disponibilidad y preparar solicitudes de pedido. La confirmación de stock, precio, condiciones y pedido permanece bajo responsabilidad del personal autorizado.

**Problema identificado:** En una operación que combina productos en stock, pedidos por catálogo, múltiples marcas, unidades como metro o rollo y atención residencial y Contract, pueden existir diferencias entre la forma en que se nombran los productos, se registra su disponibilidad y se responde a los clientes. Esa posible desalineación debe verificarse en el diagnóstico y podría dificultar la consulta, generar retrabajo y limitar la preparación confiable de pedidos. El asistente no resolvería por sí solo el problema: depende de atributos completos, fuentes identificables, reglas de disponibilidad y gobernanza de datos.

**Alcance:** El diagnóstico y diseño se concentrarán en una o dos familias de producto y en el flujo búsqueda o recomendación → disponibilidad → solicitud preliminar → validación por asesor. Incluirán mapa AS-IS con supuestos validables, taxonomía y diccionario de atributos, modelo conceptual de producto e inventario, reglas de disponibilidad, diseño TO-BE conversacional, guion de intenciones y excepciones, requisitos de trazabilidad, criterios de derivación humana y roadmap condicionado. Se excluyen la implementación de ERP/WMS/PIM, la normalización exhaustiva del catálogo, el chatbot productivo autónomo, pagos, reservas automáticas, confirmación automática de pedidos e inventario en tiempo real no sustentado por integraciones verificadas.

## Fuentes

- Romantex — Empresa: https://www.romantex.com.pe/empresa
- Romantex — Company: https://www.romantex.com.pe/company
- Romantex — Inicio: https://romantex.com.pe/
- Romantex — Contacto: https://www.romantex.com.pe/contacto
- UniversidadPeru — Romantex S.A.C.: https://www.universidadperu.com/empresas/romantex.php
- Ubicania — Romantex S.A.C.: https://ubicania.com/empresas/romantex-s-a-c_id_143809909583B417
- Dossier de Arquitectura — nuevo showroom: https://dossierdearquitectura.com/romantex-nos-presenta-su-nuevo-showroom/
- Ellas Internacional — renovación y liderazgo: https://www.ellasinternacional.com/romantex-renueva-su-esencia-diseno-vanguardia-y-vision-innovadora-al-frente-del-sector-deco-en-peru/
- BigCommerce — Andover Fabrics: https://www.bigcommerce.com/case-study/andover-fabrics/
- Stock2Shop — Aranda Textiles: https://www.stock2shop.com/case-studies/aranda/
- Salesforce — West Marine: https://www.salesforce.com/blog/west-marine-customer-story/
- Bow Chat — AI ordering case: https://bow.chat/customers/ai-ordering-food-distribution
