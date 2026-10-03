# Brainstorm de auditoría — IRD-2

## CONTEXTO

- modo: una_alternativa
- tipo_sujeto: empresa
- empresa: Romantex S.A.C., importador-showroom de telas decorativas, revestimientos y accesorios

## Tema de entrada

Digitalización del inventario y estandarización de atributos y medidas de producto textil en Romantex S.A.C.

Romantex enfrenta el desafío de integrar y optimizar digitalmente sus procesos de gestión de productos, inventario, ventas y atención al cliente, debido a la amplitud de su catálogo y a la necesidad de atender diferentes tipos de clientes y proyectos. Aunque la empresa cuenta con presencia digital y una tienda virtual, existe una oportunidad de fortalecer la integración entre el inventario físico, la información de los productos, las ventas y la atención comercial. La variedad de telas, colores, composiciones, medidas y aplicaciones hace necesario disponer de información actualizada y centralizada para evitar inconsistencias, mejorar la disponibilidad de productos y facilitar la decisión de compra.

## Acta (brainstorm-theme)

## Rol: Brainstorm theme

### Supuestos de CONTEXTO

- La entidad es **Romantex S.A.C.**, dedicada a telas decorativas, revestimientos y accesorios; el foco se formula como **atributos, SKU y medidas textiles** (ancho de rollo, color, composición y unidad de venta).
- Evidencia pública: showrooms San Isidro/Surco, catálogo multimarca importado, línea Contract, stock en almacén, tienda web y ~17 colaboradores — empresa mediana con venta consultiva y catálogo muy heterogéneo.
- Fase **init-theme-audit**: informe diagnóstico académico; no se exige implementación ni acceso a sistemas internos.

### Modo

una_alternativa

### Lente problema/usuario

- **Quién sufre el dolor:** asesores de showroom, equipo comercial Contract y clientes (diseñadores de interiores, decoradores, hotelería) que consultan disponibilidad, variantes y plazos antes de comprar.
- **Dolor concreto:** catálogo amplio (telas, colores, composiciones, anchos, aplicaciones) sin **fuente única de verdad** → respuestas lentas o inconsistentes sobre stock, equivalencias entre marcas y medidas; riesgo de prometer material no disponible o duplicar esfuerzo entre showroom, almacén y canal digital.
- **Por qué importa en Perú (Lima premium):** el cliente B2B/B2C de decoración exige rapidez y precisión; la competencia (showrooms y distribuidores de telas en Lima) ya ofrece consulta digital; Romantex compite por asesoría + variedad importada, pero la fricción operativa erosiona la experiencia consultiva que es su diferencial.
- **Datos de ventas infrautilizados:** sin atributos estandarizados, difícil detectar tendencias (colores, fibras, anchos) para reposición y negociación con proveedores internacionales.

### Lente viabilidad de curso

- **Cabe en diagnóstico:** mapeo AS-IS de procesos (recepción importación → etiquetado/almacén → consulta showroom → pedido → despacho), evaluación de madurez digital, propuesta TO-BE acotada (PIM ligero + visibilidad de inventario + taxonomía de producto), benchmark sectorial y recomendaciones priorizadas — sin pretender un ERP completo ni integración en tiempo real de todos los canales.
- **Riesgos de vacío:** sin acceso a ERP/WMS interno, el informe debe apoyarse en observación pública (web, showrooms, LinkedIn, catálogos), entrevistas simuladas o marco teórico, y declarar límites explícitos.
- **Riesgos de inabarcable:** evitar "transformación digital total"; el catálogo multimarca con miles de referencias importadas hace inviable estandarizar todo el histórico en un semestre — acotar a **familias prioritarias** (p. ej. telas para tapicería/cortinas + línea Contract) o a **proceso núcleo** (consulta-disponibilidad-venta).
- **Encaje con escala (~17 personas):** soluciones proportionadas (hoja maestra de producto, códigos internos, integración web-showroom básica) más realistas que IoT en almacén o IA predictiva avanzada.

### Lente oportunidad/ángulo

- **Giro defendible:** el problema no es "falta de web" (ya existe presencia digital) sino **desalineación entre catálogo comercial, atributos de producto e inventario físico** — la digitalización empieza por estandarizar el "lenguaje del producto" antes que automatizar ventas.
- **Oportunidad diferenciada:** Romantex mezcla importación multimarca + stock propio + proyectos Contract; un modelo de datos unificado les permitiría escalar la línea Contract sin multiplicar errores operativos.
- **Qué no perseguir:** reemplazo total de ERP, trazabilidad RFID, predicción de demanda con ML, ni estandarización exhaustiva de todo el catálogo histórico internacional en fase diagnóstico.

### Síntesis — Ángulos

#### 1

- **Tema:** Fuente única de producto (PIM ligero) y taxonomía textil para consultas de showroom
- **Descripción:** Diseñar un modelo de datos mínimo que unifique atributos textil (ancho de rollo, composición, color/código, unidad de venta metro/rollo, aplicación tapicería/cortina/revestimiento) como base para que asesores respondan consultas con información consistente, independientemente de la marca importada.
- **Problema:** Cada marca trae convenciones distintas de nomenclatura y medidas; los asesores dependen de memoria, fichas dispersas o catálogos PDF, lo que retrasa cotizaciones y genera inconsistencias frente al cliente.
- **Alcance:** Diagnóstico AS-IS del flujo consulta→cotización en showroom; propuesta de taxonomía y plantilla de ficha producto para 2–3 familias prioritarias; evaluación de herramientas PIM/ERP accesibles para PYME; roadmap TO-BE sin implementación.
- **tipo_sujeto tentativo:** empresa (importador-showroom textil decoración)
- **empresa nombrada:** Romantex S.A.C.

#### 2

- **Tema:** Visibilidad de inventario multicanal (almacén ↔ showroom ↔ tienda web) para disponibilidad confiable
- **Descripción:** Analizar cómo integrar, al menos a nivel conceptual y de procesos, el stock del almacén central con la consulta en showrooms (Paz Soldán, El Polo) y el canal e-commerce, priorizando **disponibilidad consultable** sobre automatización completa de pedidos.
- **Problema:** Clientes y asesores no pueden confirmar en tiempo útil si hay metros disponibles de una variante concreta; el desfase entre stock físico y lo publicado/consultado genera fricción, reprocesos y pérdida de confianza en compras de proyecto.
- **Alcance:** Mapa de canales y puntos de consulta de stock; identificación de cuellos de botella (actualización manual, doble registro); propuesta de sincronización periódica (no necesariamente tiempo real) y reglas de reserva para pedidos Contract; benchmark de prácticas en retail textil/HORECA.
- **tipo_sujeto tentativo:** empresa (retail B2B/B2C + Contract)
- **empresa nombrada:** Romantex S.A.C.

#### 3

- **Tema:** Estandarización de SKU y medidas como habilitador de datos de venta y reposición
- **Descripción:** Definir un **SKU interno Romantex** que cruce referencia de proveedor, atributos normalizados y unidad logística (rollo/metro), habilitando reportes básicos de rotación y tendencias sin proyectos de BI avanzado.
- **Problema:** Sin codificación coherente, las ventas se registran con descripciones libres; imposible agregar demanda por ancho, color o fibra, lo que limita decisiones de importación y negociación con marcas internacionales.
- **Alcance:** Diagnóstico de codificación actual (hipótesis desde procesos públicos observables); diseño de esquema SKU/atributos para familias de mayor rotación; propuesta de indicadores simples (top colores, anchos más vendidos, stock muerto); plan de adopción gradual en 12 meses.
- **tipo_sujeto tentativo:** empresa (importador con catálogo multimarca)
- **empresa nombrada:** Romantex S.A.C.

### Descartados / no perseguir

- Implementación de **ERP/WMS enterprise** o integración en tiempo real omnicanal completa — desproporcionado para escala y fase diagnóstico.
- **Estandarización total** del catálogo multimarca importado (miles de referencias) en un solo proyecto.
- **IA/ML predictivo**, RFID o automatización de almacén — sin evidencia de madurez digital previa ni datos limpios.
- Proyectos ajenos: CRM avanzado, marketplace propio, o transformación de la línea Contract sin resolver primero datos de producto e inventario.

### Notas

- Los tres ángulos son **variantes del mismo tema** (digitalización de inventario + estandarización de atributos/SKU textil); comparten núcleo ("fuente única de verdad del producto") pero enfatizan consulta comercial (1), disponibilidad multicanal (2) o analítica/reposición (3).
- Para **init-theme-audit**, el ángulo **1 o 2** suele ser más defendible con evidencia pública limitada; el **3** requiere inferir más sobre procesos de venta internos — conviene declararlo como hipótesis a validar en auditoría.
- Alcance curso recomendado transversal: **2 showrooms + almacén + canal web**, 2–3 familias de producto, horizonte TO-BE 12–18 meses, solo recomendaciones.
