# Debate utilidad — bibliography-auto — ITD

**Modo:** `bibliography_auto_utilidad`  
**Profile:** Romantex S.A.C. — taxonomía textil + SKU/maestro producto piloto; DQ de atributos; showroom/almacén/web; PYME; exclusiones ERP enterprise / RFID / IA / omnicanal completo.

**Fuentes OA consultadas:** OpenAlex, Semantic Scholar (429 parcial), arXiv (ruido alto), verificación DOI/PDF.  
**Queries:** product information management / product data; master data product SKU SME; product data quality completeness; inventory digitalization textile retail; datos/maestro producto inventario PYME.

## Veredictos por candidato

| ID | Candidato | Crítico | Defensor | Orquestador |
|----|-----------|---------|----------|-------------|
| C1 | Božić et al. 2024 — Product master data quality → logistics | GO | GO | **GO — descargar** |
| C2 | Ghosh 2026 — Footwear taxonomy / attribute standardization | GO | GO | **GO — descargar** |
| C3 | Günther et al. 2019 — DQ assessment methodology SMEs | GO_con_cambios | GO | **GO_con_cambios — descargar** (citar método DQ, no ERP) |
| C4 | Carreño et al. 2019 — Inventarios PYME alimentos UNMSM | NO_GO | GO_con_cambios | **NO_GO** (duda → no descargar) |
| C5 | Keinänen 2018 — Assessment of Product Data Quality (thesis) | GO | GO | **GO — descargar** |
| C6 | McCormick et al. 2014 — Fashion retailing ICT/omnichannel | NO_GO | GO_con_cambios | **NO_GO** |
| C7 | Spruit & Pietzka 2014 — MD3M maturity | GO_con_cambios | GO_con_cambios | **GO_con_cambios — descargar** (solo Data Model/DQ) |
| C8 | Müller et al. 2020 — I4.0 SME BM | NO_GO | NO_GO | **NO_GO** |
| C9 | Abbate et al. 2023 — TAF sustainability | NO_GO | NO_GO | **NO_GO** |
| C10 | Sarder & Biswas 2026 — Textile retail SCM Bangladesh | NO_GO | NO_GO | **NO_GO** |

## Ataques (crítico) — síntesis
- C2 único casi-alineado a taxonomía/atributos, pero calzado ≠ textil metro/rollo.
- C1 justifica impacto de master data, no diseña taxonomía.
- C3/C7 huelen a ERP/MDM enterprise — filtrar citas.
- C4/C6/C8–C10 fuera del núcleo MVP1.

## Defensas — síntesis
- Ensamble: impacto PMDQ (C1) + taxonomía catálogo (C2) + método DQ PYME (C3/C5) + madurez MDM acotada (C7).
- Hueco: no hay paper gemelo “textil LATAM showroom SKU”.

## Prioridad de descarga (≤5)
1. Božić 2024  
2. Ghosh 2026  
3. Günther 2019  
4. Keinänen 2018  
5. Spruit 2014  

## Rechazos / pendiente_oa
- Rechazados: C4, C6, C8, C9, C10 (y ruido OpenAlex/arXiv: YOLO defectos, e-textiles, etc.).
- **Descargados OK:** C1 Božić, C2 Ghosh, C7 Spruit (UU Repository).
- **`pendiente_oa` (GO pero PDF bloqueado 403 / sin bitstream usable):**
  - C3 Günther et al. 2019 — DOI 10.1016/j.promfg.2019.02.114 (ScienceDirect / Fraunhofer sin PDF directo).
  - C5 Keinänen 2018 — Theseus handle 10024/143064 (403).
- No se inventaron fichas en `docs.md` para pendientes.
