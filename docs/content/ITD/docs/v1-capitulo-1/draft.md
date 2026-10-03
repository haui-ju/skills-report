# Informe académico — Capítulo 1

| Campo | Valor |
|-------|--------|
| Proyecto | ITD |
| Tema | Digitalización del inventario y estandarización de atributos de producto textil en Romantex S.A.C. |
| Versión | v1-capitulo-1 |
| Fecha | 2026-09-06 |
| Alcance de esta versión | Capítulo 1 (presentación, diagnóstico situacional, modelo de negocio) |

---

## Capítulo 1: Presentación de la empresa

### 1.1. Presentación de la empresa

Romantex S.A.C. es una sociedad anónima cerrada peruana dedicada a la comercialización de telas decorativas, revestimientos murales, pasamanería y accesorios de interiorismo de alta gama. Opera como importador y casa de showroom en Lima, con sede en Av. Paz Soldán 185 (San Isidro) y un segundo punto de atención en Av. El Polo 376 (Surco), y mantiene presencia digital en romantex.com.pe (Romantex, n.d.-a; UniversidadPeru, n.d.). El presente informe se sitúa en ese contexto empresarial: el proyecto académico examina la articulación entre inventario físico, catálogo multimarca y canales comerciales, con el fin de proponer una fuente única de verdad del producto textil; la presentación de la organización, no obstante, precede y condiciona cualquier diseño de solución.

#### 1.1.1. Reseña histórica

La actividad comercial de Romantex se asocia a la segunda mitad de los años noventa. El directorio empresarial público registra el inicio de actividades en octubre de 1995, mientras la narrativa corporativa sitúa la apertura del local en San Isidro y la consolidación de la marca en 1996 (UniversidadPeru, n.d.; Romantex, n.d.-a). Desde entonces, la empresa se posicionó como especialista en telas finas y revestimientos importados para uso residencial y comercial, con énfasis en curaduría de color, estilo y moda.

En las décadas siguientes, el modelo de negocio se amplió más allá del stock exhibido en sala. Romantex articuló tres capas comerciales que hoy siguen visibles en su propuesta pública: (1) un showroom y almacén con miles de metros disponibles para entrega inmediata; (2) un área de pedidos por catálogo de firmas internacionales; y (3) una línea Contract orientada a hoteles, restaurantes y espacios públicos, con productos sujetos a especificaciones técnicas del rubro (Romantex, n.d.-a). Esa combinación —stock propio, importación bajo catálogo y proyectos de hospitalidad— diferencia a la firma de un simple retail de confección y explica la heterogeneidad de nomenclaturas, unidades de venta (metro/rollo) y atributos técnicos que el proyecto académico toma como objeto de análisis.

En el período reciente (2024–2025), medios especializados han documentado la renovación de imagen y showrooms bajo el liderazgo público de Susana Balmaceda, presentando a Romantex como referente del segmento deco de alto nivel en el Perú (Ellas Internacional, 2024). La empresa comunica dos locales limeños, canales telefónicos y correo institucional, y un catálogo en línea que convive con la atención consultiva en sala (Romantex, n.d.-b). La escala pública reportada en directorios empresariales ronda los diecisiete trabajadores, coherente con una PYME especializada más que con un retailer masivo (UniversidadPeru, n.d.).

#### 1.1.2. Misión

Romantex no publica en su sitio web un enunciado formal de misión corporativa. A partir de la narrativa institucional disponible, su propósito operativo se resume en especializar la oferta limeña de telas y revestimientos importados de alta calidad, combinando stock inmediato, pedidos por catálogo internacional y asesoría de diseñadores de interiores para proyectos residenciales y comerciales (Romantex, n.d.-a).

#### 1.1.3. Visión

Tampoco se halla una visión formal publicada. La proyección implícita en fuentes oficiales y cobertura reciente apunta a consolidarse como casa de referencia en decoración e interiorismo de vanguardia en el Perú, anticipando tendencias internacionales y elevando la experiencia de showroom como espacio de inspiración y consulta técnica, no solo de transacción (Romantex, n.d.-a; Ellas Internacional, 2024).

#### 1.1.4. Valores

En ausencia de un listado explícito de valores, la identidad de gestión comunicada enfatiza: curaduría y exclusividad de producto; atención personalizada; rigor técnico en la línea Contract; mejora continua del conocimiento del rubro; e inversión sostenida en operaciones y servicio al cliente (Romantex, n.d.-a). Esa identidad de “casa exclusiva de telas decorativas” es el marco cultural en el que cualquier digitalización de datos de producto debe preservar la promesa consultiva, sin reducir la relación comercial a un catálogo transaccional genérico.

### 1.2. Diagnóstico situacional

El diagnóstico siguiente se elabora con base en información pública de la empresa y referentes del sector; no sustituye un AS-IS operativo interno auditado en campo. Las fricciones de datos de producto se formulan como tensiones organizacionales plausibles a la luz del modelo publicado (stock vs catálogo, multisede, venta consultiva), no como magnitudes ya medidas.

#### 1.2.1. Análisis del microentorno (fortalezas y debilidades)

**Fortalezas.** Romantex acumula casi tres décadas de posicionamiento en el segmento premium de telas y revestimientos en Lima, con marca reconocible y propuesta de valor explícita en stock amplio y servicio integral (Romantex, n.d.-a). Opera dos showrooms en distritos de alto poder adquisitivo (San Isidro y Surco), lo que concentra la demanda residencial y profesional (diseñadores) cerca de sus puntos de contacto (Romantex, n.d.-b). La coexistencia de stock inmediato, pedidos por catálogo y línea Contract le permite atender tanto compra rápida como proyectos de hospitalidad con requisitos técnicos (Romantex, n.d.-a). La presencia digital (sitio y catálogo en línea) ya existe; el reto no es “crear web desde cero”, sino alinear lenguaje de producto e inventario con esa vitrina (Romantex, n.d.-b). La escala PYME facilita, en principio, gobernar un piloto acotado de datos de producto sin depender de un programa enterprise de transformación.

**Debilidades.** El catálogo multimarca importado implica nomenclaturas heterogéneas de proveedores; cada firma trae códigos, descripciones y convenciones distintas de composición, ancho y presentación, lo que tensiona la consistencia del lenguaje comercial entre showroom, almacén y canal digital. La propia empresa distingue públicamente productos “en stock” frente a productos “por catálogo”, señal de una arquitectura comercial dual que exige claridad de atributos y de origen de disponibilidad para no prometer plazos incorrectos (Romantex, n.d.-a; Romantex, n.d.-b). En venta consultiva, la confirmación de qué es el material, de qué está compuesto y en qué unidad se vende (metro o rollo) tiende a depender de múltiples artefactos (fichas de marca, memoria operativa, catálogo web), patrón documentado en la literatura de calidad de datos maestros de producto como factor que degrada el desempeño logístico y comercial cuando el maestro es incompleto o inconsistente (Božić et al., 2024). La ausencia de un enunciado formal de misión/visión y de indicadores públicos de madurez de datos sugiere que la gobernanza del “golden record” de producto aún no está institucionalizada de forma visible (Spruit & Pietzka, 2015).

**Implicación para el proyecto / MVP.** El microentorno justifica priorizar un maestro de producto gobernado (taxonomía deco mínima + SKU interno + atributos obligatorios) sobre un ERP enterprise o un omnicanal en tiempo real. El piloto propuesto (aproximadamente 30–50 referencias en dos o tres familias) apunta a demostrar que el asesor puede responder qué es, composición y unidad de venta sin cruzar tres fuentes, como condición previa a visibilidad multisede o alineación fina del catálogo web.

#### 1.2.2. Análisis del macroentorno (oportunidades y amenazas)

**Oportunidades.** En distribución textil, casos como Andover Fabrics ilustran la integración de inventario y atributos (incluidas unidades tipo yarda/rollo) hacia un catálogo digital B2B mediante plataformas de distribución y comercio electrónico (Acumatica, n.d.; BigCommerce, n.d.). En Perú, la experiencia documentada de digitalización de inventario multitienda en Textil Inversiones y Negocios Cerna S.A.C. (Gamarra) muestra que codificación por variante, trazabilidad y herramientas locales son alcanzables a escala PYME, aunque el patrón talla–color de confección debe adaptarse al metro/rollo y a atributos deco (Ñañez Palomino, 2024). El mercado local ofrece suites orientadas a textil y decoración (por ejemplo, Kaypi e Invy) que pueden cubrir matriz de variantes e inventario, pero suelen partir de supuestos de confección o POS; ello abre espacio a una diferenciación basada en taxonomía deco (composición estructurada, ancho, aplicación residencial/Contract) antes de seleccionar stack (Kaypi, n.d.; Invy, n.d.). A nivel de diseño de catálogo, la estandarización de taxonomía y atributos se reconoce como condición de discoverability y consistencia omnicanal incluso en verticales moda-adyacentes (Ghosh, 2026). Referentes de vocabulario textil como el Global Textile Scheme aportan marco de atributos sectoriales para una adopción incremental, sin exigir certificación plena en un piloto PYME (Global Textile Scheme, n.d.).

**Amenazas.** La competencia de casas de telas y distribuidores deco en Lima puede ofrecer consulta digital más ágil si Romantex no cierra la brecha entre promesa de stock inmediato y confirmación confiable de variantes. La oferta commodity de ERP/POS textil en Perú (Kaypi, Odoo/partners, Invy, entre otros) puede empujar a “comprar sistema” antes de ordenar el maestro de datos, amplificando inconsistencias si el modelo de atributos no está definido (Božić et al., 2024; Spruit & Pietzka, 2015). La dependencia de marcas internacionales expone a cambios de colección, nomenclatura y lead times de importación. Architectures omnicanal de gran escala (p. ej. DOM tipo Pittarello/OneStock) resultan desproporcionadas para una PYME de showroom y pueden inducir sobreingeniería si se toman como plantilla literal.

**Implicación para el proyecto / MVP.** El macroentorno refuerza un camino de gobernanza de datos primero (madurez de modelo y calidad, en la línea de MD3M) y referentes de distribución textil (Andover) y PYME peruana (Cerna) como contraste de escala, no como copia de stack. Quedan fuera del alcance inmediato RFID, IA predictiva y estandarización del histórico completo de marcas.

### 1.3. Modelo de negocio

#### 1.3.1. Lienzo Lean Canvas

El lienzo principal describe el **modelo de negocio de Romantex S.A.C.** según información pública. Las celdas se interpretan con cautela donde no hay estados financieros publicados.

| PROBLEMA (del cliente) | SOLUCIÓN (oferta Romantex) | PROPUESTA DE VALOR ÚNICA | VENTAJA ESPECIAL | SEGMENTO DE CLIENTES |
|------------------------|----------------------------|---------------------------|------------------|----------------------|
| Encontrar telas/revestimientos de alta gama con asesoría experta; especificar materiales para proyectos residenciales u hoteleros; obtener stock inmediato o pedido de marca internacional con plazos claros. | Showrooms San Isidro y Surco; almacén con metros en stock; pedidos por catálogo de firmas mundiales; línea Contract; diseñadores de interiores en sala; catálogo web de consulta/cotización (Romantex, n.d.-a; Romantex, n.d.-b). | Para diseñadores, hogares exigentes y proyectos Contract que necesitan telas y revestimientos importados con criterio estético y técnico, Romantex es la casa deco premium que combina stock inmediato, catálogo internacional y asesoría en showroom, a diferencia de retail genérico o solo pedido online sin curaduría. | Posicionamiento de marca premium y red de representación de firmas internacionales; relación consultiva consolidada en Lima; doble showroom en distritos clave. Difícil de copiar en el corto plazo sin capital reputacional equivalente. | Primario: diseñadores de interiores y clientes residenciales de alto ticket en Lima. Secundario: hoteles, restaurantes y espacios públicos (Contract). Early adopters digitales: clientes que exploran catálogo web antes de visitar sala. |

| MÉTRICAS CLAVE (negocio) | CANALES |
|--------------------------|---------|
| Rotación de metros/familias; mix stock vs pedido catálogo; ticket y tasa de cierre en showroom; proyectos Contract ganados; tráfico y cotizaciones web (no publicados; a validar con la empresa). | Showrooms físicos; asesoría presencial; teléfono/email; sitio romantex.com.pe (descubrimiento y cotización); ferias y networking del rubro deco. |

| ESTRUCTURA DE COSTOS | FLUJO DE INGRESOS |
|----------------------|-------------------|
| Importación y capital de trabajo en stock; arriendo/operación de showrooms y almacén; personal comercial y técnico; marketing y presencia digital; cumplimiento Contract. | Margen sobre telas, revestimientos y accesorios vendidos por metro/rollo o proyecto; pedidos especiales por catálogo; eventuales servicios de asesoría asociados a la venta consultiva. |

**Encaje del proyecto (contraste con el MVP académico).** El Lean del piloto de curso no reemplaza el modelo anterior: se centra en un **maestro de producto** (taxonomía + SKU piloto de 30–50 referencias) para que el lenguaje comercial interno coincida entre almacén, showrooms y web. Sus métricas de éxito (completitud ≥90 % de atributos obligatorios; respuesta de ficha sin cruzar tres fuentes) son indicadores de gobernanza de datos al servicio del negocio descrito, no un nuevo modelo de ingresos. En madurez MDM, equivale a fortalecer primero las capacidades de modelo de datos y calidad antes de integrar canales de forma agresiva (Spruit & Pietzka, 2015).

---

## Referencias bibliográficas

Acumatica. (n.d.). *Andover Fabrics success story*. https://www.acumatica.com/success-stories/andover-fabrics/

BigCommerce. (n.d.). *Andover Fabrics case study*. https://www.bigcommerce.com/case-study/andover-fabrics/

Božić, D., Živičnjak, M., Stanković, R., & Ignjatić, A. (2024). Impact of the product master data quality on the logistics process performance. *Logistics, 8*(2), Article 43. https://doi.org/10.3390/logistics8020043

Ellas Internacional. (2024). *Romantex renueva su esencia: diseño, vanguardia y visión innovadora al frente del sector deco en Perú*. https://www.ellasinternacional.com/romantex-renueva-su-esencia-diseno-vanguardia-y-vision-innovadora-al-frente-del-sector-deco-en-peru/

Ghosh, S. (2026). Footwear catalog management in e-commerce: A study of product taxonomy, attribute standardization, and category hierarchy. *International Journal for Multidisciplinary Research, 8*(3). https://doi.org/10.36948/ijfmr.2026.v08i03.81995

Global Textile Scheme. (n.d.). *GTS standard*. https://www.globaltextilescheme.org/

Invy. (n.d.). *Control de inventario para tiendas de ropa*. https://www.invyperu.com/blog/inventario-tienda-ropa-tallas-colores

Kaypi. (n.d.). *Sistema ERP textil*. https://kaypi.pe/sistema-erp-para-textileria

Ñañez Palomino. (2024). *Implementación de un sistema digital para el control de inventarios… Textil Inversiones y Negocios Cerna SAC* [Trabajo de suficiencia profesional, USIL]. https://hdl.handle.net/20.500.14005/16335

Romantex. (n.d.-a). *Empresa*. https://www.romantex.com.pe/empresa

Romantex. (n.d.-b). *Inicio / contacto*. https://www.romantex.com.pe/

Spruit, M., & Pietzka, K. (2015). MD3M: The master data management maturity model. *Computers in Human Behavior, 51*(Pt. B), 1068–1076. https://doi.org/10.1016/j.chb.2014.09.030

UniversidadPeru. (n.d.). *Romantex S.A.C.* https://www.universidadperu.com/empresas/romantex.php
