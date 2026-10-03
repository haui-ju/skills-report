# Informe académico — Capítulo 1 (reporte)

| Campo | Valor |
|-------|--------|
| Proyecto | ITD |
| Tema | Digitalización del inventario y estandarización de atributos de producto textil en Romantex S.A.C. |
| Versión | v1-capitulo-1 |
| Fecha | 2026-09-06 |
| Alcance | Capítulo 1 (presentación, diagnóstico situacional, modelo de negocio) |
| Base | `draft.md` (solo lectura); este archivo es la versión pulida |

---

## Capítulo 1: Presentación de la empresa

### 1.1. Presentación de la empresa

Romantex S.A.C. (RUC 20293975036) es una sociedad anónima cerrada peruana que comercializa telas decorativas, revestimientos murales, pasamanería y accesorios de interiorismo de alta gama. Opera como importador y casa de showroom en Lima —sede en Av. Paz Soldán 185 (San Isidro) y segundo local en Av. El Polo 376 (Surco)— y mantiene presencia digital en romantex.com.pe (Romantex, n.d.-a; UniversidadPeru, n.d.). El proyecto académico examina cómo se articulan inventario físico, catálogo multimarca y canales comerciales para proponer una fuente única de verdad del producto textil; la organización, no el piloto, es el sujeto de este capítulo.

#### 1.1.1. Reseña histórica

El directorio empresarial sitúa el inicio de actividades en octubre de 1995; la narrativa corporativa fija la apertura en San Isidro y la consolidación de la marca en 1996 (UniversidadPeru, n.d.; Romantex, n.d.-a). Desde entonces se especializó en telas finas y revestimientos importados para uso residencial y comercial, con curaduría de color, estilo y moda.

En las décadas siguientes amplió su modelo más allá del stock de sala. Hoy conviven tres capas visibles en su propuesta pública: showroom y almacén con miles de metros para entrega inmediata; pedidos por catálogo de firmas internacionales; y línea Contract para hoteles, restaurantes y espacios públicos con especificaciones técnicas del rubro (Romantex, n.d.-a). Esa combinación —stock propio, importación bajo catálogo y línea Contract— la aparta del retail de confección y explica la heterogeneidad de nomenclaturas, unidades (metro/rollo) y atributos técnicos que el informe toma como objeto de análisis.

Entre 2024 y 2025, cobertura especializada documentó la renovación de imagen y showrooms bajo el liderazgo público de Susana Balmaceda, situando a Romantex como referente del segmento deco premium en el Perú (Ellas Internacional, 2024). Mantiene esos dos locales limeños, canales de contacto y un catálogo en línea, junto con la atención consultiva en sala (Romantex, n.d.-b). La escala reportada en directorios ronda diecisiete trabajadores, coherente con una PYME especializada (UniversidadPeru, n.d.).

#### 1.1.2. Misión

No existe un enunciado formal de misión en el sitio web. La narrativa institucional describe, en la práctica, especializar la oferta limeña de telas y revestimientos importados de alta calidad mediante stock inmediato, pedidos por catálogo y asesoría de diseñadores de interiores para proyectos residenciales y comerciales (Romantex, n.d.-a).

#### 1.1.3. Visión

Tampoco hay visión formal publicada. Fuentes oficiales y cobertura reciente proyectan que Romantex se consolide como casa de referencia en decoración e interiorismo de vanguardia en el Perú, anticipando tendencias y tratando el showroom como espacio de consulta técnica, no solo de transacción (Romantex, n.d.-a; Ellas Internacional, 2024).

#### 1.1.4. Valores

Sin listado explícito de valores, la identidad comunicada enfatiza curaduría y exclusividad, atención personalizada, rigor técnico en Contract, mejora continua del conocimiento del rubro e inversión en operaciones y servicio (Romantex, n.d.-a). Cualquier digitalización de datos de producto debe preservar esa promesa consultiva.

### 1.2. Diagnóstico situacional

El diagnóstico se basa en información pública y referentes sectoriales; no sustituye un AS-IS interno auditado. Las fricciones de datos se plantean como tensiones organizacionales plausibles (stock vs catálogo, multisede, venta consultiva), no como magnitudes medidas en Romantex.

#### 1.2.1. Análisis del microentorno (fortalezas y debilidades)

**Fortalezas.** Cuenta con casi tres décadas en el segmento premium de telas y revestimientos en Lima, con marca reconocible y propuesta de stock amplio más servicio integral (Romantex, n.d.-a). Dos showrooms en San Isidro y Surco concentran demanda residencial y profesional cerca de los puntos de contacto (Romantex, n.d.-b). La tríada stock inmediato / pedido por catálogo / Contract permite compra rápida y proyectos de hospitalidad con requisitos técnicos (Romantex, n.d.-a). Ya existe presencia digital; el reto es alinear lenguaje de producto e inventario con esa vitrina, no crear un canal desde cero (Romantex, n.d.-b).

**Debilidades.** El catálogo multimarca importa nomenclaturas distintas de composición, ancho y presentación, lo que tensiona la consistencia entre showroom, almacén y web. La distinción pública entre productos “en stock” y “por catálogo” exige claridad de atributos y de origen de disponibilidad para no prometer plazos incorrectos (Romantex, n.d.-a; Romantex, n.d.-b). En venta consultiva, confirmar qué es el material, su composición y la unidad de venta (metro o rollo) suele apoyarse en varios artefactos. En la misma línea, la literatura vincula maestros de producto incompletos o inconsistentes con peor desempeño logístico y comercial (Božić et al., 2024), sin que ello implique una medición ya realizada en Romantex. No hay indicadores públicos de madurez de datos maestros; la gobernanza del registro oficial de producto no es visible desde fuentes abiertas (Spruit & Pietzka, 2015).

**Implicación para el proyecto / MVP.** Conviene priorizar un maestro gobernado (taxonomía deco mínima, SKU interno y atributos obligatorios) antes que un ERP enterprise o un omnicanal en tiempo real. El piloto de unas 30–50 referencias en dos o tres familias busca demostrar que el asesor responde qué es, composición y unidad sin cruzar tres fuentes; la escala PYME hace manejable ese recorte, pero no constituye por sí sola una “fortaleza de mercado”.

#### 1.2.2. Análisis del macroentorno (oportunidades y amenazas)

**Oportunidades.** En distribución textil, el caso Andover Fabrics muestra inventario y atributos (incluidas unidades tipo yarda/rollo) sincronizados hacia un catálogo digital B2B con un stack de distribución y comercio electrónico (Acumatica, n.d.; BigCommerce, n.d. — un mismo referente, no dos casos independientes). En Perú, la digitalización multitienda documentada en Textil Inversiones y Negocios Cerna S.A.C. (Gamarra) prueba que codificación por variante y herramientas locales son viables a escala PYME, aunque el patrón talla–color debe adaptarse a metro/rollo y atributos deco (Ñañez Palomino, 2024). Suites locales como Kaypi o Invy cubren variantes e inventario con sesgo de confección o POS; ello deja espacio a diferenciarse con taxonomía deco (composición estructurada, ancho, uso residencial/Contract) antes de elegir software (Kaypi, n.d.; Invy, n.d.). La estandarización de taxonomía y atributos es condición de consistencia de catálogo también en verticales moda-adyacentes —p. ej. calzado (Ghosh, 2026)—; el Global Textile Scheme ofrece vocabulario sectorial para adopción incremental sin certificación plena en un piloto (Global Textile Scheme, n.d.).

**Amenazas.** Otras casas deco en Lima pueden ofrecer consulta más ágil si Romantex no cierra la brecha entre promesa de stock inmediato y confirmación confiable de variantes. La oferta commodity de ERP/POS textil (Kaypi, Odoo/partners, Invy, entre otros) puede empujar a comprar sistema antes de ordenar el maestro, amplificando inconsistencias (Božić et al., 2024; Spruit & Pietzka, 2015). La dependencia de marcas internacionales expone a cambios de colección, nomenclatura y plazos de importación. Arquitecturas DOM de gran escala (p. ej. Pittarello/OneStock) son desproporcionadas para una PYME de showroom y, tomadas como plantilla, inducen sobreingeniería.

**Implicación para el proyecto / MVP.** Gobernanza de datos primero (modelo y calidad, en la línea de MD3M), con Andover y Cerna como contraste de escala —no como copia de stack—. Quedan fuera RFID, IA predictiva y la estandarización del histórico completo de marcas.

### 1.3. Modelo de negocio

#### 1.3.1. Lienzo Lean Canvas

El lienzo describe el **modelo de negocio de Romantex S.A.C.** con información pública. Donde faltan estados financieros, las celdas son inferencias cautelosas.

| PROBLEMA (del cliente) | SOLUCIÓN (oferta Romantex) | PROPUESTA DE VALOR ÚNICA | VENTAJA ESPECIAL | SEGMENTO DE CLIENTES |
|------------------------|----------------------------|---------------------------|------------------|----------------------|
| Telas/revestimientos de alta gama con asesoría; especificación para proyectos residenciales u hoteleros; stock inmediato o pedido internacional con plazos claros. | Showrooms San Isidro y Surco; almacén con metros en stock; pedidos por catálogo; Contract; diseñadores en sala; catálogo web de consulta/cotización (Romantex, n.d.-a; Romantex, n.d.-b). | Para diseñadores, hogares exigentes y proyectos Contract que requieren materiales importados con criterio estético y técnico, Romantex combina stock inmediato, catálogo internacional y asesoría en showroom, frente a retail genérico o pedido online sin curaduría. | Marca premium y red de firmas internacionales; relación consultiva en Lima; doble showroom en distritos clave — capital reputacional difícil de replicar en el corto plazo. | Primario: diseñadores y residencial alto ticket en Lima. Secundario: hoteles, restaurantes y espacios públicos (Contract). Early adopters digitales: quien explora la web antes de visitar sala. |

| MÉTRICAS CLAVE (negocio) | CANALES |
|--------------------------|---------|
| Rotación de metros/familias; mix stock vs pedido catálogo; ticket y cierre en showroom; proyectos Contract; tráfico y cotizaciones web (no publicados; a contrastar con la empresa). | Showrooms; asesoría presencial; teléfono/email; romantex.com.pe; ferias y networking deco. |

| ESTRUCTURA DE COSTOS | FLUJO DE INGRESOS |
|----------------------|-------------------|
| Importación y capital de trabajo en stock; operación de showrooms y almacén; personal comercial y técnico; marketing digital; cumplimiento Contract. | Margen sobre telas, revestimientos y accesorios por metro/rollo o proyecto; pedidos especiales por catálogo; asesoría asociada a la venta consultiva. |

**Tesis de valor (para la empresa).** Estandarizar atributos y un SKU piloto convierte el activo ya vendible —stock, catálogo y Contract— en dato confiable que acelera cotizaciones y reduce promesas inconsistentes, sin crear un nuevo modelo de ingresos.

**Encaje del proyecto (contraste con el MVP académico).** El Lean del piloto no sustituye el lienzo anterior: se limita a un maestro de producto (taxonomía + SKU de 30–50 referencias) para alinear el lenguaje interno entre almacén, showrooms y web. Sus indicadores (completitud ≥90 % de atributos; respuesta de ficha sin tres fuentes) miden gobernanza de datos al servicio del negocio, no un P&L nuevo. En madurez MDM, equivale a reforzar primero modelo de datos y calidad antes de integrar canales de forma agresiva (Spruit & Pietzka, 2015).

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
