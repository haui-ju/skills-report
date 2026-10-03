# Informe de proyecto — IRD-2

## Capítulo 1. Presentación de la empresa

**Tema:** Digitalización del inventario y estandarización de atributos y medidas de producto textil en Romantex S.A.C.

**Versión:** 1 — capítulo 1

**Fecha:** 6 de septiembre de 2026

### 1.1. Presentación de la empresa

#### 1.1.1. Reseña histórica

Romantex S.A.C. es una empresa peruana dedicada a la comercialización de productos para la decoración textil y de interiores. Su sitio institucional señala que se estableció en 1996 y que se especializa en telas decorativas, revestimientos murales y accesorios importados para usos residenciales y comerciales (Romantex, s. f.-a). La empresa articula su oferta alrededor del diseño, los materiales y la asesoría para ambientaciones domésticas y proyectos profesionales.

La ficha registral pública identifica a ROMANTEX S.A.C. como sociedad anónima cerrada, con RUC 20293975036, condición activa e inicio de actividades registrado el 1 de octubre de 1995. También registra como dirección legal la avenida Paz Soldán 185, San Isidro, Lima, y vincula la empresa con su sitio web corporativo (UniversidadPeru, s. f.). La fecha registral y la referencia institucional a 1996 se conservan como datos de fuentes distintas: la primera corresponde al inicio de actividades registrado y la segunda a la historia comercial comunicada por la marca.

Actualmente, Romantex publica dos puntos de atención en Lima: la sede de San Isidro y el local de la avenida El Polo 376, Surco. Su sitio ofrece además catálogo, solicitud de muestras y datos de contacto, lo que configura una operación que combina showroom, asesoría y comunicación digital (Romantex, s. f.-a, s. f.-b). Esta combinación vuelve relevante que la información de producto sea suficientemente precisa para relacionar una variante con su aplicación, unidad de venta y disponibilidad.

La oferta pública comprende telas decorativas, revestimientos murales, pasamanería, cojines y accesorios, con productos importados y marcas internacionales. También incluye atención de proyectos comerciales mediante una línea Contract (Romantex, s. f.-a; UniversidadPeru, s. f.). El proyecto estudia cómo representar esa diversidad mediante un lenguaje común de producto e inventario; no presume que los procesos internos actuales estén desintegrados.

#### 1.1.2. Misión

Romantex no publica un enunciado formal identificado como misión en las fuentes consultadas. Su comunicación institucional, sin embargo, presenta una orientación consistente hacia la especialización en telas decorativas, revestimientos y accesorios de calidad para aplicaciones residenciales y comerciales (Romantex, s. f.-a). En ese posicionamiento, el conocimiento del producto y la asesoría son parte de la relación con el cliente.

Para el proyecto, esta orientación significa que la información de producto cumple una función comercial, no solo administrativa. La propuesta se limita a ordenar los atributos de dos o tres familias prioritarias antes de recomendar una integración tecnológica.

#### 1.1.3. Visión

Tampoco se encontró una declaración pública formal de visión. La proyección observable en la comunicación de Romantex combina una oferta especializada de productos importados, variedad de diseños y atención de proyectos. Sus showrooms de San Isidro y Surco, junto con el catálogo y la solicitud de muestras en línea, conectan la experiencia física con el contacto digital (Romantex, s. f.-b).

El proyecto traduce esa orientación en una capacidad operativa concreta: que comercial y almacén puedan consultar una misma representación de la variante, con referencia original, atributos normalizados, unidad de venta, ubicación y estado de validación. Esta es una decisión del proyecto, no una declaración institucional atribuida a Romantex.

#### 1.1.4. Valores

Las fuentes públicas no presentan un listado formal de valores corporativos. Sí permiten reconocer principios observables de especialización, variedad, atención personalizada, calidad decorativa y aplicación de los productos a proyectos residenciales y comerciales. La línea Contract amplía esa propuesta hacia hoteles, restaurantes y espacios públicos, donde las especificaciones del material deben acompañar a su valor estético (Romantex, s. f.-a).

La estandarización propuesta respeta esos principios porque no elimina las particularidades del catálogo. Conserva la referencia del proveedor y documenta las reglas utilizadas para normalizar familia, composición, color, medidas y unidad de venta.

### 1.2. Diagnóstico situacional

#### 1.2.1. Análisis del microentorno (fortalezas y debilidades)

El microentorno de Romantex reúne equipos comerciales y de almacén, proveedores o marcas internacionales, diseñadores, compradores residenciales y responsables de proyectos Contract. La relación se desarrolla en los showrooms y mediante canales digitales, alrededor de telas, revestimientos y accesorios.

| Fortalezas | Debilidades o fricciones a diagnosticar |
|---|---|
| Especialización pública en decoración textil, revestimientos y accesorios para usos residenciales y comerciales (Romantex, s. f.-a). | La variedad de marcas, composiciones, colores, anchos y unidades puede dificultar la descripción uniforme de las variantes; debe comprobarse con una muestra de fichas y registros. |
| Presencia física en San Isidro y Surco, catálogo digital y solicitud de muestras (Romantex, s. f.-b). | La coexistencia de showroom, almacén y canal web puede crear puntos distintos de consulta o actualización; se trata de una brecha a observar, no de una falla demostrada. |
| Atención B2C, B2B y de proyectos Contract, que relaciona atributos del producto con aplicaciones concretas (Romantex, s. f.-a). | Si no existe una autoridad clara para aprobar nombres, unidades y normalizaciones, el modelo maestro puede perder vigencia. |
| Catálogo importado y marcas internacionales, base de una propuesta diferenciada de diseño y variedad (Romantex, s. f.-a; UniversidadPeru, s. f.). | Las convenciones del proveedor pueden no coincidir con la nomenclatura interna o con la búsqueda del cliente; deben distinguirse alias, referencia original y SKU interno. |

La cuestión operativa es si comercial, almacén y canal digital pueden reconocer una misma variante mediante atributos suficientes y una unidad de venta inequívoca. El MVP 1 aborda esa cuestión con un diccionario de datos, una taxonomía, una ficha maestra, una propuesta de SKU y una matriz de calidad y responsabilidades para dos o tres familias.

#### 1.2.2. Análisis del macroentorno (oportunidades y amenazas)

La digitalización del comercio textil aumenta la importancia de que los datos de producto puedan reutilizarse entre proveedores, catálogos, puntos de venta y canales digitales. Global Textile Scheme describe un estándar para intercambiar datos de productos entre fabricantes, proveedores, marcas y retailers, con integración posible a sistemas PDM, PLM, PIM y ERP (Global Textile Scheme, s. f.). El referente no implica que Romantex deba adoptarlo, pero muestra que la traducción y calidad de datos son problemas reconocidos del sector.

Andover Fabrics documenta el uso de Acumatica Distribution integrado con BigCommerce para inventario, pedidos y catálogo digital en un distribuidor textil estadounidense (Acumatica, 2026). Pittarello documenta, por su parte, el uso de OneStock y Shopify Plus para activar inventario de tiendas, organizar pedidos y conectar puntos físicos con demanda digital (OneStock, 2026). Son patrones de referencia, no soluciones que puedan trasladarse automáticamente a la escala o necesidades de Romantex.

| Oportunidades | Amenazas |
|---|---|
| Ordenar los datos maestros puede mejorar la reutilización de fichas en showroom, canal digital y proyectos Contract. | Integrar antes de ordenar los datos puede automatizar duplicidades, equivalencias incorrectas o estados desactualizados. |
| Una taxonomía orientada a aplicación, composición, medidas y mantenimiento puede reforzar la venta consultiva. | Las nomenclaturas de marcas internacionales pueden elevar el costo de consolidación y mantenimiento del catálogo. |
| Andover Fabrics, Pittarello y Global Textile Scheme ofrecen patrones concretos para estudiar inventario, catálogo e intercambio de datos (Acumatica, 2026; Global Textile Scheme, s. f.; OneStock, 2026). | Una plataforma enterprise puede introducir complejidad y dependencia tecnológica desproporcionadas para el alcance actual. |
| Los canales físicos y digitales permiten probar el modelo con una muestra antes de ampliar la integración. | Sin un responsable de validación y actualización, la información perderá vigencia. |

**Implicación para el proyecto / MVP.** La primera etapa debe ser el MVP 1, “Diagnóstico y modelo maestro de producto”. La consulta de disponibilidad por ubicación y los indicadores de reposición se dejan para fases posteriores, porque dependen de que los atributos y las variantes estén identificados de manera consistente.

### 1.3. Modelo de negocio

#### 1.3.1. Lienzo Lean Canvas

El siguiente lienzo describe el modelo de negocio de Romantex a partir de su oferta y presencia pública. Los costos, ingresos y métricas se formulan con prudencia porque la empresa no publica estados financieros ni una estructura detallada de precios.

| Problema | Solución | Propuesta de valor única | Ventaja especial | Segmentos de clientes |
|---|---|---|---|---|
| - Selección de materiales decorativos con criterios de diseño y aplicación.<br>- Proyectos que requieren coordinar muestras, especificaciones, medidas y disponibilidad.<br>- Complejidad de un catálogo multimarca para comparar alternativas. | - Showrooms y asesoría personalizada.<br>- Catálogo de telas, revestimientos y accesorios importados.<br>- Atención de proyectos residenciales, comerciales y Contract. | Para diseñadores, compradores residenciales y responsables de proyectos que buscan materiales decorativos diferenciados, Romantex es un especialista en telas, revestimientos y accesorios importados que combina variedad, asesoría y contacto físico/digital, frente a una compra basada solo en una ficha genérica. | Especialización en decoración textil, relación entre producto y aplicación, showrooms en Lima y atención de proyectos. La dificultad de copia no está cuantificada públicamente. | Diseñadores de interiores; clientes residenciales; responsables de hoteles, restaurantes y espacios públicos; compradores de proyectos comerciales; solicitantes de muestras. |

| Métricas clave | Canales |
|---|---|
| Solicitudes de muestras; consultas y cotizaciones por familia; conversión de consultas a pedidos; disponibilidad; recurrencia de clientes de proyectos. La empresa no publica valores de estas métricas. | Showrooms de San Isidro y Surco; sitio web; solicitud de muestras; teléfono, correo y redes sociales publicados por la empresa. |

| Estructura de costos | Flujo de ingresos |
|---|---|
| Importación y adquisición; almacenamiento; operación de showrooms; personal de asesoría; muestras; logística y atención de pedidos. La distribución exacta no es pública. | Venta de telas decorativas, revestimientos, pasamanería, cojines y accesorios; pedidos residenciales y comerciales; soluciones para línea Contract. Precios y márgenes no publicados. |

**Encaje del proyecto.** El Lean Canvas del MVP no sustituye este lienzo empresarial. Reduce un riesgo operativo concreto: si la propuesta depende de variedad y asesoría, una ficha inconsistente puede aumentar el tiempo de respuesta y dificultar la confirmación de una variante. El MVP 1 medirá completitud, duplicidad, tiempo de búsqueda y discrepancias entre registro y muestra para decidir si conviene avanzar hacia una consulta de disponibilidad por ubicación.

## Referencias bibliográficas

Acumatica. (2026). *Andover Fabrics doubles growth with modern cloud ERP*. https://www.acumatica.com/success-stories/andover-fabrics/

Global Textile Scheme. (s. f.). *What is GTS?* https://www.globaltextilescheme.org/gts-standard/

OneStock. (2026). *How Pittarello drove 58% growth with an omnichannel OMS for fashion retail*. https://www.onestock-retail.com/customer-story/omnichannel-oms-for-fashion-retail-pittarello/

Romantex. (s. f.-a). *Company*. https://www.romantex.com.pe/empresa

Romantex. (s. f.-b). *Romantex*. https://www.romantex.com.pe/

UniversidadPeru. (s. f.). *Romantex S.A.C.* https://www.universidadperu.com/empresas/romantex.php
