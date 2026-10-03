# FODA — MVP 1: Taxonomía textil + SKU piloto

**Proyecto:** ITD · Romantex S.A.C.  
**Movimiento del MVP:** pasar de fuentes dispersas a un maestro gobernado (30–50 refs) antes de sync multicanal.

## FODA

| Fortalezas | Debilidades |
|------------|-------------|
| - Catálogo premium y showrooms públicos verificables (San Isidro + Surco) dan contexto concreto al piloto. `evidencia` <br>- Alcance acotado a 2–3 familias y 30–50 refs reduce explosión de variantes. `evidencia` profile <br>- Prototipo Sheets/Airtable barato y reversible (I1). `hipótesis` DT | - Dolor operativo (cruzar ≥3 fuentes) aún no cuantificado en campo. `pendiente_campo` → R1 <br>- Sin data owner designado ni autoridad de rechazo de altas incompletas. `pendiente_campo` → R2 <br>- AS-IS de sistemas (ERP/Excel/OpenCart) desconocido; riesgo de diseñar maestro paralelo. `pendiente_campo` → (cola O5; no R#) |

| Oportunidades | Amenazas |
|---------------|----------|
| - Práctica PIM/MDM: gobernanza y taxonomía **antes** de herramienta (reduce “basura amplificada”). `evidencia` sector <br>- Diferenciar deco metro/rollo + Contract frente a matriz talla-color Gamarra/Cerna. `evidencia` contrastiva <br>- Early adopters showroom pueden validar HMW-1 en días. `hipótesis` | - Adopción fallida: equipos vuelven a “Excel sombra” si el maestro está incompleto. `evidencia` sector → R3 <br>- Commodity ERP local (Kaypi/Odoo) tienta a saltarse taxonomía. `evidencia` mercado PE <br>- Convenciones de N marcas importadas chocan con SKU interno propuesto. `hipótesis` → R4 |

## TOWS

| | Oportunidades (O) | Amenazas (A) |
|--|-------------------|--------------|
| **Fortalezas (F)** | **FO:** Usar el piloto acotado (2–3 familias, 30–50 refs) para demostrar ficha única al showroom premium antes de cualquier ERP. → Prototype | **FA:** Anclar el piloto a criterio ≥90 % completitud y gate de data owner para no copiar el fallo “PIM sin gobernanza”. → R2 · R5 |
| **Debilidades (D)** | **DO:** Fase 0 (shadowing cotizaciones + mapa de fuentes) convierte debilidades de evidencia en baseline medible. → R1 · DT Test | **DA:** No abrir MVP 2/3 ni comprar stack hasta falsar adopción del maestro y viabilidad del SKU interno. → R3 · R4 |

## Amarre post-RAT

| Candidato (texto corto) | R# |
|-------------------------|----|
| Dolor ≥3 fuentes no cuantificado | R1 |
| Data owner / autoridad de rechazo | R2 |
| Adopción maestro vs Excel sombra | R3 |
| Choque convención SKU / nomenclaturas | R4 |
| Completitud ≥90 % atributos recuperables | R5 |

**Implicación de la semana:** cerrar designación de data owner (R2) + agenda de shadowing cotizaciones (R1) mientras se prueba la convención SKU con compras (R4) antes de declarar “completo” masivo (R5/R3).
