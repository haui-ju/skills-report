# RAT — MVP 1: Taxonomía textil + SKU piloto

**Proyecto:** ITD · Romantex S.A.C.  
**SoT de supuestos y umbrales** para DT Test y brecha AS-IS→TO-BE.  
**Contraste externo (cupo RAT):** gobernanza y ownership previos a PIM/herramienta; fallo típico = maestro incompleto → “Excel sombra” (McFadyen; Start with Data; Innowinds MDM). `evidencia` sector — no prueba el caso Romantex.

---

## R1

- **ID:** R1
- **Supuesto:** En cotizaciones del alcance piloto, el asesor **necesita cruzar ≥3 fuentes** para responder qué es / composición / unidad de venta.
- **Etiqueta actual:** `hipótesis` / `pendiente_campo`
- **Impacto si falso:** alto (si ya hay ficha única usable, el MVP 1 pierde justificación)
- **Incertidumbre:** alta
- **Falsación:**
  - **observar:** shadowing de cotizaciones reales (O1); contar fuentes abiertas por episodio
  - **con_quien:** vendedor showroom (San Isidro o Surco)
  - **umbral:** en muestra ≥8 cotizaciones del piloto potencial, si **&lt;40 %** cruzan ≥3 fuentes → R1 falsado (dolor sobreestimado)
  - **ventana:** 2–3 turnos / 1 semana de observación
- **Dueño_entregable:** estudiante
- **Contraparte_campo:** vendedor showroom
- **Origen:** FODA-D (dolor no cuantificado) | DT Empathize | profile

---

## R2

- **ID:** R2
- **Supuesto:** Existe (o se designará en ≤2 semanas) un **data owner** con autoridad para rechazar altas incompletas del maestro.
- **Etiqueta actual:** `pendiente_campo`
- **Impacto si falso:** alto (sin steward, ≥90 % completitud no es gobernable; patrón sectorial de fallo PIM)
- **Incertidumbre:** alta
- **Falsación:**
  - **observar:** nombramiento escrito (mail/acta) + 1 rechazo documentado de ficha incompleta
  - **con_quien:** gerencia / responsable comercial u operaciones
  - **umbral:** binario — si en 14 días no hay owner nombrado **o** no hay ≥1 rechazo/gate aplicado → R2 falsado
  - **ventana:** primeras 2 semanas del piloto
- **Dueño_entregable:** estudiante
- **Contraparte_campo:** gerencia o encargado de operaciones/compras
- **Origen:** FODA-D | FODA-A (adopción) | DT Prototype roles | evidencia sector MDM

---

## R3

- **ID:** R3
- **Supuesto:** El vendedor **adoptará el maestro** como primera (y preferente) fuente en cotizaciones del piloto, sin volver al PDF/chat como SoT.
- **Etiqueta actual:** `hipótesis`
- **Impacto si falso:** alto (sin adopción, no hay “fuente única”)
- **Incertidumbre:** alta
- **Falsación:**
  - **observar:** en cotizaciones del piloto, qué abre primero el vendedor; captura de pantalla o checklist de sombra
  - **con_quien:** vendedor early adopter
  - **umbral:** en ≥10 cotizaciones del piloto con ficha “completo”, si el maestro **no** es la 1.ª fuente en ≥70 % → R3 falsado
  - **ventana:** tras ≥20 refs en estado completo
- **Dueño_entregable:** estudiante
- **Contraparte_campo:** vendedor showroom
- **Origen:** FODA-A (Excel sombra) | Lean métricas | evidencia sector PIM fail

---

## R4

- **ID:** R4
- **Supuesto:** La convención `RX-{FAM}-{MARCA3}-{SEQ4}` (o equivalente acordado) es **usable** por compras/ventas sin colisión grave con códigos ya usados.
- **Etiqueta actual:** `hipótesis`
- **Impacto si falso:** medio-alto (retrasa piloto; obliga a rediseñar identificador)
- **Incertidumbre:** media
- **Falsación:**
  - **observar:** workshop 60–90 min con compras + 1 vendedor; listar códigos actuales y conflictos
  - **con_quien:** compras / importaciones
  - **umbral:** si ≥30 % de una muestra de 20 refs piloto tienen conflicto irresoluble de mapeo proveedor→SKU interno → R4 falsado (hay que cambiar convención)
  - **ventana:** antes de cargar las primeras 20 refs “completo”
- **Dueño_entregable:** estudiante
- **Contraparte_campo:** compras
- **Origen:** FODA-A (choque nomenclaturas) | DT Prototype SKU

---

## R5

- **ID:** R5
- **Supuesto:** Los atributos obligatorios definidos (familia, composición estructurada, ancho, unidad, origen_disponibilidad, …) son **recuperables** desde fichas de proveedor / operación actual para ≥90 % del piloto.
- **Etiqueta actual:** `hipótesis`
- **Impacto si falso:** alto (criterio de éxito del profile imposible)
- **Incertidumbre:** media-alta
- **Falsación:**
  - **observar:** carga de 30 refs; checklist de campos faltantes por fuente
  - **con_quien:** compras + data owner
  - **umbral:** si &lt;90 % de las 30 primeras refs alcanzan estado “completo” en ≤15 días hábiles de carga → R5 falsado (hay que reducir obligatorios o cambiar familias)
  - **ventana:** fase de carga inicial del piloto
- **Dueño_entregable:** estudiante
- **Contraparte_campo:** data owner + compras
- **Origen:** profile criterio_exito | Lean métricas | FODA-D

---

## Cola no RAT

- Stack AS-IS exacto (ERP vs solo Excel/OpenCart): relevante para MVP 3; diferido — `contraste: diferido` hasta mapa de fuentes O5.
- Exactitud metros físicos vs registro: pertenece a MVP 2; no falsar aquí como supuesto central del MVP 1.
