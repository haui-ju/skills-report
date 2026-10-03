# Auditoría de tema — ITD

## CONTEXTO
- dominio: retail decoración / textiles de interior (importación, showroom, contract)
- pais_region: Perú (Lima — San Isidro, Surco)
- fase_entregable: diagnostico
- restricciones: empresa real; evidencia pública; sin acceso a sistemas internos; alcance acotado a PYME (~17 colaboradores); no pretender ERP enterprise ni omnicanal completo
- modo: una_alternativa
- tipo_sujeto: empresa
- empresa: Romantex S.A.C.

## Tema propuesto (entrada)
**Tema:** Digitalización del inventario y estandarización de tallaje en Calzados Romantex S.A.C.

**Descripción:** Romantex enfrenta el desafío de integrar y optimizar digitalmente sus procesos de gestión de productos, inventario, ventas y atención al cliente, debido a la amplitud de su catálogo y a la necesidad de atender diferentes tipos de clientes y proyectos. Aunque la empresa cuenta con presencia digital y una tienda virtual, existe una oportunidad de fortalecer la integración entre el inventario físico, la información de los productos, las ventas y la atención comercial. La variedad de telas, colores, composiciones, medidas y aplicaciones hace necesario disponer de información actualizada y centralizada para evitar inconsistencias, mejorar la disponibilidad de productos y facilitar la decisión de compra.

**Problema identificado:** Dificultades para conocer en tiempo real el stock disponible, responder rápidamente a consultas de clientes, gestionar pedidos de manera eficiente y aprovechar datos de ventas para identificar tendencias. El reto central es integrar canales y sistemas de información para construir una gestión basada en datos.

**Alcance:** (no acotado por el usuario en la entrada)

## Ficha de empresa (investigación)
**Identidad:** ROMANTEX S.A.C., RUC 20293975036, sociedad anónima cerrada, activa desde octubre de 1995 (operaciones comerciales desde 1996). Sede legal: Av. Paz Soldán 185, San Isidro, Lima. Segundo showroom: Av. El Polo 376, Surco. Importador registrado; ~17 trabajadores (fuente pública de directorio empresarial). Sector: comercialización de telas decorativas, revestimientos murales, pasamanería y accesorios de decoración de interiores.

**Reseña histórica (pública):** Fundada en 1996 en San Isidro como casa especializada en telas finas y decoración. Se ha posicionado como referente peruano en telas y revestimientos de alta gama, con presencia en ferias internacionales del rubro y renovaciones recientes de showrooms (2024–2025). Liderazgo público asociado a Susana Balmaceda.

**Misión / visión / valores:** No publica misión/visión formales en sitio web; la propuesta de valor declarada en fuentes oficiales enfatiza: especialización en telas y revestimientos importados de alta calidad; vanguardia en moda decorativa; servicio integral con diseñadores de interiores; stock amplio para entrega inmediata; línea Contract para hoteles, restaurantes y espacios públicos; mejora continua técnica y de servicio.

**Oferta / sector relevante:**
- Showroom + almacén con miles de metros de telas y revestimientos en stock.
- Pedidos por catálogo de marcas internacionales.
- Línea Contract (hospitalidad, restaurantes, áreas públicas).
- Cojines propios, pasamanería y accesorios complementarios.
- Presencia digital: romantex.com.pe (catálogo/consulta en línea).
- Atención personalizada B2C y B2B (diseñadores, proyectos residenciales y comerciales).

**Evidencia_empresa:** suficiente

**Fuentes de empresa:**
- https://www.romantex.com.pe/empresa
- https://www.romantex.com.pe/
- https://linkedin.com/company/romantex-sac
- https://www.universidadperu.com/empresas/romantex.php
- https://www.ellasinternacional.com/romantex-renueva-su-esencia-diseno-vanguardia-y-vision-innovadora-al-frente-del-sector-deco-en-peru/

## Brainstorm
Acta: theme-audit-brainstorm.md — ángulos retenidos:
1. **PIM ligero + taxonomía textil** para consultas de showroom (fuente única de atributos: ancho, composición, color, metro/rollo, aplicación).
2. **Visibilidad multicanal** almacén ↔ showrooms (Paz Soldán, El Polo) ↔ canal web — disponibilidad consultable.
3. **Estandarización SKU/medidas** como habilitador de analítica comercial y reposición.

**Nota de corrección:** "Calzados Romantex" no corresponde al giro real; Romantex S.A.C. es empresa de telas decorativas. "Tallaje" se reinterpreta como estandarización de atributos y medidas de producto textil (ancho, metro/rollo, composición, uso residencial/contract).

## Benchmarking (`benchmark-theme`)
**Casos (directo|proxy):**
1. **Andover Fabrics** (EE.UU.) — **directo** — Distribuidor B2B de telas; Acumatica Distribution + BigCommerce B2B; inventario y atributos (yardas/rollos) sincronizados al catálogo; búsqueda/filtros por atributos textil. Fuentes: https://www.acumatica.com/success-stories/andover-fabrics/ ; https://www.bigcommerce.com/case-study/andover-fabrics/
2. **Inversiones y Negocios Cerna SAC** (Lima — Gamarra) — **directo en Perú / proxy retail textil** — SKM Solución (inventario + POS multisede); SKU modelo–talla–color, QR, transferencias almacén↔tiendas, alertas stock. Fuente: tesis USIL 2024 — https://hdl.handle.net/20.500.14005/16335
3. **Fabric Sense** (textiles & furnishings) — **proxy deco/cortinería** — ERPNext a medida: inventario por rollos, pedidos por medidas/proyecto, flujo ventas–confección–despacho. Fuente: https://infintrixtech.com/case-studies/fabric-sense-curtain-order-management

**Mini-matriz:**

| Capacidad / eje | Andover | Cerna (Perú) | Fabric Sense | Relevancia Romantex |
|-----------------|---------|--------------|--------------|---------------------|
| Taxonomía/atributos (composición, ancho, uso) | parcial | parcial | parcial | alta |
| Matriz SKU / variantes complejas | presente | presente | presente | alta |
| Inventario tiempo real multi-ubicación | presente | presente | parcial | alta |
| Integración catálogo ↔ stock ↔ comercial | presente | parcial | presente | alta |
| Showroom con disponibilidad consultable | ausente | parcial | parcial | alta |
| Segmentación residencial vs. contract | desconocido | ausente | ausente | alta (diferenciador) |

**Qué adaptar:**
- Modelo maestro de producto tipo Andover, escala Cerna: SKU interno = marca + referencia + color + composición + ancho + unidad (m/rollo) + aplicación.
- Sincronización periódica (diaria o intradiaria) almacén ↔ showrooms ↔ web, con reservas para pedidos Contract.
- Taxonomía mínima viable para 2–3 familias (tapicería, cortinas, revestimientos).
- "Showroom conectado" simplificado: consulta unificada de stock por ubicación, inspirado en multisede/QR de Cerna.
- Unidades de medida explícitas (metros por rollo), análogo a yardas/bolts en Andover.

**Diferenciador posible:**
- Taxonomía deco-peruana orientada a venta consultiva (atributos residencial/Contract, ignífugo, mantenimiento embebidos en ficha comercial).
- Puente B2B2C para interioristas/Contract con visibilidad de lote/rollo.
- Gobernanza de datos antes que stack enterprise; alineación incremental con estándares GTS.

**Evidencia:** suficiente

## Tema afinado (pre-polish)
**Tema:** Digitalización del inventario y estandarización de atributos de producto textil en Romantex S.A.C.

**Descripción:** Diagnóstico de la integración entre inventario físico (almacén y dos showrooms en Lima), catálogo multimarca importado y canales comerciales (venta consultiva, línea Contract, presencia web) de Romantex S.A.C. El foco es construir una fuente única de verdad del producto — atributos textil estandarizados (composición, color, ancho, unidad metro/rollo, aplicación residencial/contract) — que habilite consultas de disponibilidad confiables, gestión eficiente de pedidos y uso básico de datos de venta, sin pretender una transformación ERP completa.

**Problema identificado:** Desalineación entre catálogo comercial heterogéneo (múltiples marcas internacionales con nomenclaturas distintas), registro de inventario y atención comercial multicanal, lo que dificulta confirmar stock en tiempo útil, genera inconsistencias en cotizaciones y limita el aprovechamiento de datos para reposición y tendencias.

**Alcance:**
- **Geográfico/operativo:** almacén central + showrooms San Isidro (Paz Soldán 185) y Surco (El Polo 376) + canal web romantex.com.pe.
- **Producto:** 2–3 familias prioritarias (p. ej. telas tapicería/cortinas, revestimientos murales, línea Contract).
- **Entregable:** mapeo AS-IS, benchmark sectorial, propuesta TO-BE (taxonomía + modelo de datos + sincronización inventario-catálogo-comercial), roadmap 12–18 meses con recomendaciones — sin implementación ni acceso a sistemas internos.
- **Exclusiones:** ERP/WMS enterprise, RFID, IA predictiva, estandarización exhaustiva de todo el histórico importado, digitalización de calzado/tallas.

## Fuentes
- Romantex — Empresa: https://www.romantex.com.pe/empresa
- Romantex — Contacto/locales: https://www.romantex.com.pe/
- Romantex SAC (LinkedIn): https://linkedin.com/company/romantex-sac
- Romantex S.A.C. (directorio): https://www.universidadperu.com/empresas/romantex.php
- Ellas Internacional — renovación Romantex: https://www.ellasinternacional.com/romantex-renueva-su-esencia-diseno-vanguardia-y-vision-innovadora-al-frente-del-sector-deco-en-peru/
- Andover Fabrics / Acumatica: https://www.acumatica.com/success-stories/andover-fabrics/
- Andover Fabrics / BigCommerce: https://www.bigcommerce.com/case-study/andover-fabrics/
- Textil Cerna SAC — tesis USIL 2024: https://hdl.handle.net/20.500.14005/16335
- Fabric Sense / Infintrix: https://infintrixtech.com/case-studies/fabric-sense-curtain-order-management
- Global Textile Scheme (referente estandarización): https://www.globaltextilescheme.org/
