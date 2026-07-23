# Examen Costos — "Marzo 2023" (real 16/02/2023)

Verificado contra solución oficial (planilla de cálculo incluida en `Examen Costos 03-2023 - Preg. I,II,III.pdf` — cubre I, II y III). Las Partes IV, V y VI (teóricas) no vienen con solución oficial en el repo — se responden con el criterio de la Guía / conocimiento general de la materia.

---

## I – Metraje (20 pts)

**Enunciado:** volumen de hormigón, tenor de encofrado y cuantía de hierro de la viga del Anexo 1 (largo 3,40m, sección 20×30cm). Ganchos únicamente en estribos (10Φ); varilla comercial 12m.

**Volumen y encofrado:** V = 0,20×0,30×3,40 = **0,204 m³** (redondeado a 0,20 en la planilla, pero el tenor/cuantía se calculan con el valor sin redondear). Encofrado total = **2,84 m²** (viga aislada suspendida, encofrado en las caras expuestas del corte).

**Armadura** (2 familias longitudinales superiores "A" + 1 inferior "E" + 2 tipos de estribo):

| Tipo | Ø (mm) | Cant. | L unit. (m) | L tot (m) | kg (c/desp) | Nota |
|---|---|---|---|---|---|---|
| Longitudinal A, **con prolongación** en los extremos | 12 | 2 | 4,00 (3,40 + 0,60 de prolongación en apoyos) | 8,00 | **7,83** | bordes 2Φ12 que se extienden más allá del corte, hacia el apoyo |
| Longitudinal A, **sin prolongación** | 12 | 1 | 3,40 | 3,40 | **3,33** | barra recta, longitud = viga |
| Longitudinal inferior "E" | 10 | 2 | 3,60 (3,40 + 0,20 de anclaje) | 7,20 | **4,91** | pequeña extensión de anclaje en cada extremo |
| Estribo, zona de extremo (paso 10cm, 5 c/extremo × 2 extremos) | 6 | 10 | 1,12 (perímetro 2×(0,20+0,30)=1,00 + 2 ganchos×10Φ=0,12) | 11,20 | **2,59** | zona densificada junto a los apoyos |
| Estribo, zona central (paso 20cm) | 6 | 12 | 1,12 | 13,44 | **3,10** | tramo central, menor densidad de corte |
| **TOTAL** | | | | | **21,76** | |

*Cantidad de estribos: leída directamente del despiece del plano (5 estribos c/10cm a cada extremo = 10 en total; tramo central resuelto con la misma sección de estribo, cantidad de forma de no duplicar los estribos límite entre zonas). Longitud unitaria de estribo = perímetro completo (sin descontar recubrimiento, según dato del enunciado) + 2 ganchos de 10Φ.*

**Resultados finales:**
- Total Vol. hormigón: **0,204 m³**
- Total encofrado: **2,84 m²**
- Total acero (con desperdicio): **21,76 kg**
- **Tenor de encofrado = 2,84/0,204 = 13,92 m²/m³**
- **Cuantía de acero = 21,76/0,204 = 106,68 kg/m³**

*(Tenor y cuantía muy altos — esperable: viga muy chica (sección 20×30cm, 3,40m) con mucha densidad de armado relativa a su volumen; el mismo fenómeno visto en Jul-2025 con un pilar de sección delgada.)*

---

## II – Consumos (10 pts)

**Rendimientos:** Of.Carpintero 5,00 hs/m³ pasta + Ayudante 3,00 hs/m³ pasta; Of.Carpintero/Ayudante 0,90 hs/m² encofrado c/u; Of.Herrero/Ayudante 0,04 hs/kg hierro c/u. Tabla de pino 2,40×0,15m (área=0,36 m²), desperdicio 10%, 3 reúsos. Desperdicio hormigón premezclado 5%.

| Insumo | Fórmula | Cons. Unitario /m³ |
|---|---|---|
| Ayudante (hs) | 3,00 + 13,92×0,90 + 106,68×0,04 | **19,80** |
| Oficial Carpintero (hs) | 5,00 + 13,92×0,90 | **17,53** |
| Oficial Herrero (hs) | 106,68×0,04 | **4,27** |
| Hormigón premezclado (m³) | 1×1,05 | **1,05** |
| Hierro (kg) | = Cuantía | **106,68** |
| Tabla de pino (unid) | (13,92×1,10)/(0,36×3) | **14,18** |

**HH/m³ total:** 19,80+17,53+4,27 = **41,60 hs/m³** (alto, coherente con el tenor/cuantía de esta viga chica).

---

## III – Análisis Económico y Financiero (20 pts)

**Datos:** Costo Total=$5.000.000; Beneficio=20% sobre venta (P); Leyes Sociales=$1.000.000; Plazo de ejecución=5 meses, ejecución y venta uniformes. Distribución del costo: mano de obra 30% (pago vía convenio colectivo, sin desfase), materiales 50% + otros 20% (pago a 30 días). Cobro: 20% anticipo en el mes 1, 90% restante (venta sin anticipo) cobrado a 90 días de certificado. Certificación mensual, tasa de interés 5% mensual.

**Precio de venta:** Beneficio=20%×P → P = Costo/(1−0,20) = 5.000.000/0,80 = **$6.250.000**.

**a) Cronograma económico** (devengado, uniforme en 5 meses): venta=1.250.000/mes, costo=1.000.000/mes → **beneficio=250.000/mes**, acumulado 250k→1.250k (20% de la venta total, los 3 últimos meses de la tabla quedan planos porque la ejecución ya terminó).

**b) Cronograma financiero** (caja, según forma de pago):
- **Ingresos:** el 20% de anticipo ($1.250.000) se cobra íntegro en el **mes 1**. El 80% restante de cada mes se cobra 90 días (3 meses) después de certificado: lo certificado en el mes *n* (80%×1.250.000=$1.000.000) se cobra en el mes *n+3*. Así: mes1=$1.250.000 (solo anticipo); mes2=mes3=$0; mes4 a mes8=$1.000.000 c/u (los 5 meses certificados, corridos 3 meses). Total=$6.250.000.
- **Egresos mano de obra** (pago "convenio colectivo", con medio mes de desfase típico de jornales): mes1=$150.000 (mitad); mes2 a mes5=$300.000 c/u; mes6=$150.000 (la otra mitad del último mes). Total=$1.500.000 (30% del costo).
- **Egresos materiales y otros** (pago a 30 días, 1 mes de desfase): mes2 a mes6=$700.000 c/u (=70%×1.000.000, materiales 50%+otros 20%). Total=$3.500.000.

| mes | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 |
|---|---|---|---|---|---|---|---|---|
| Ingresos | 1.250.000 | | | 1.000.000 | 1.000.000 | 1.000.000 | 1.000.000 | 1.000.000 |
| Egr. mano obra | −150.000 | −300.000 | −300.000 | −300.000 | −300.000 | −150.000 | | |
| Egr. mat.+otros | | −700.000 | −700.000 | −700.000 | −700.000 | −700.000 | | |
| **Saldo mensual** | **1.100.000** | **−1.000.000** | **−1.000.000** | **0** | **0** | **150.000** | **1.000.000** | **1.000.000** |
| **Flujo acumulado** | **1.100.000** | **100.000** | **−900.000** | **−900.000** | **−900.000** | **−750.000** | **250.000** | **1.250.000** |

**c) Línea de crédito mínima necesaria = $900.000** (el peor momento de caja, sostenido en los meses 3, 4 y 5).

**d) Costo financiero, tasa 5% mensual — dos alternativas:**

El interés de cada mes se calcula sobre el flujo acumulado **sin interés** (de la tabla de arriba) de ese mismo mes, y se va sumando en forma acumulada al flujo original.

- **Alternativa A — "remunerando excedentes":** el banco paga interés también sobre los saldos **positivos** (no solo cobra sobre los negativos). Interés mensual = 5%×flujo acumulado (con signo) de ese mes: mes1=+55.000; mes2=+5.000; mes3=−45.000; mes4=−45.000; mes5=−45.000; mes6=−37.500. **Costo financiero total = −$112.500** (18,20% de beneficio final sobre venta, contra el 20% "puro").
- **Alternativa B — "remunerando solo necesidades":** el banco **no** paga interés sobre saldos positivos, solo cobra sobre los negativos: mes1=mes2=$0; mes3=−45.000; mes4=−45.000; mes5=−45.000; mes6=−37.500. **Costo financiero total = −$172.500** (17,24% de beneficio final sobre venta).

**La Alternativa A es más conveniente para la empresa** (menor costo financiero neto, $112.500 contra $172.500), porque compensa parte del costo de los meses deficitarios con el interés ganado en los meses de saldo positivo.

---

## IV – Seguros para las Obras (15 pts) *(teórico, sin solución oficial en el repo)*

**a) Finalidad general:** trasladar a un tercero (asegurador) el riesgo de eventos que pueden generar pérdidas patrimoniales significativas durante la ejecución de la obra (daños, accidentes, responsabilidad civil), a cambio de una prima cierta y conocida — protege tanto a la empresa constructora como al comitente y a terceros ajenos a la obra.

**b) Componentes principales de una póliza:** objeto/bien asegurado, riesgos cubiertos (y exclusiones), suma asegurada, prima, franquicia (deducible a cargo del asegurado), vigencia/plazo, beneficiario, y condiciones particulares y generales.

**c) Seguros más usuales en obra (ver Guía sección 10):**
- **Todo Riesgo Construcción / Obra Civil:** cubre daños materiales a la obra en ejecución (incendio, robo, fenómenos climáticos, errores de ejecución).
- **Responsabilidad Civil:** cubre daños a terceros (personas o bienes ajenos a la obra) originados por la ejecución de los trabajos.
- **Accidentes de trabajo (BSE):** cubre al personal obrero por accidentes y enfermedades laborales, obligatorio por ley.
- **Seguro de equipos/maquinaria:** cubre daño o rotura de los equipos propios usados en obra.
- **Seguro de Fianza / Garantías** (fiel cumplimiento, buena ejecución, anticipo): no cubre un siniestro físico sino el incumplimiento contractual — ver Guía sección 7.

---

## V – Suministros (15 pts) *(teórico, sin solución oficial en el repo)*

Ver Guía sección 14 (mismo criterio ya usado en exámenes previos):

**a) Identificados:** especificación técnica sin ambigüedad (norma, memoria descriptiva), marca/calidad de referencia si corresponde.

**b) Cuantificados:** unidad de medida coherente con cómo se compra/certifica, desperdicio explícito, cantidad surgida de un metraje verificable, plazo de entrega acorde al cronograma.

**c) Valorados:** precio unitario acorde a la unidad definida, cotización vigente de proveedor representativo, condiciones de pago y entrega comparables entre cotizaciones.

---

## VI – Generalidades (10 pts) *(teórico, sin solución oficial en el repo — respuesta con conocimiento general de la materia)*

**Principales características del Mercado de la Construcción en Uruguay:**
- **Fuerte dependencia de la obra pública** (vialidad, vivienda, infraestructura) como motor de demanda, junto con la obra privada (vivienda, comercial) — muy sensible al ciclo económico y a la inversión pública/extranjera.
- **Alta atomización de la oferta**: conviven pocas empresas grandes (con capacidad para obras de gran porte, licitaciones internacionales) con una gran cantidad de empresas medianas y pequeñas/informales.
- **Estacionalidad y volatilidad**: fuerte sensibilidad a la coyuntura económica, tasas de interés y financiamiento; históricamente ciclos de auge y caída marcados.
- **Mano de obra intensiva** y regulada específicamente (Ley 14.411, Convenio Colectivo Grupo 37, Aporte Unificado de la Construcción) — costo laboral con peso relevante en el costo total.
- **Regulación fuerte del sector público** (TOCAF para licitaciones y contrataciones públicas, normativa de seguridad e higiene, normas técnicas UNIT).
- **Dependencia de insumos importados** para ciertos materiales/equipos, con exposición al tipo de cambio.
- **Concentración geográfica** de la actividad y de las principales empresas en Montevideo y área metropolitana.

---

## Resumen ejecutivo del examen

| Parte | Resultado clave |
|---|---|
| I – Metraje | Vol=0,204 m³; Encof=2,84 m²; Tenor=13,92 m²/m³; Acero=21,76 kg; Cuantía=106,68 kg/m³ (viga chica, muy densa) |
| II – Consumos | Ayudante 19,80 hs/m³; HH/m³ total=41,60 |
| III – Análisis Económico-Financiero | Precio de venta $6.250.000; línea de crédito mínima $900.000 (meses 3-5); costo financiero Alt.A (remunera excedentes) $112.500 < Alt.B (solo necesidades) $172.500 → **conviene Alt.A** |
| IV – Seguros | Finalidad, componentes de póliza, seguros usuales (Todo Riesgo, RC, Accidentes BSE, Equipos, Fianza) |
| V – Suministros | Identificados / Cuantificados / Valorados |
| VI – Generalidades | Mercado uruguayo: dependencia obra pública, atomización, estacionalidad, mano de obra regulada, TOCAF, importación de insumos |
