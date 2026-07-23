# Examen Costos — Febrero 2023 (26/01/2023)

Verificado contra solución oficial (planilla de cálculo incluida en `Examen Costos 02-2023 - Preg. I,II,III.pdf` — cubre I, II y III). Las Partes IV y V (teóricas) no vienen con solución oficial en el repo — se responden con el criterio de la Guía.

---

## I – Metraje (25 pts)

**Enunciado:** volumen de hormigón, tenor de encofrado y cuantía de hierro del conjunto de 4 vigas de fundación (VF028, VF029, VF086, VF087) del Anexo 1. Recubrimientos despreciados; ganchos según croquis; varilla comercial 12m. **Observación clave del enunciado oficial:** "se considera viga hasta borde interno de pilares" — el largo L de cada viga ya viene dado directo en la planilla de armado (no hace falta descontar el ancho de los pilares de las cotas del plano).

**Volúmenes y encofrado** (b×h×L; encofrado = 2 caras laterales + cara inferior, tratadas como viga suspendida pese al nombre "de fundación" — regla de oro #2 de la Guía):

| Viga | L (m) | b (m) | h (m) | V (m³) | Encof (m²) |
|---|---|---|---|---|---|
| VF028 | 3,20 | 0,25 | 0,35 | 0,280 | 3,04 |
| VF029 | 3,20 | 0,25 | 0,35 | 0,280 | 3,04 |
| VF086 | 5,00 | 0,25 | 0,35 | 0,4375 | 4,75 |
| VF087 | 5,00 | 0,25 | 0,35 | 0,4375 | 4,75 |
| **Total** | | | | **1,435** | **15,58** |

*Encof = (2h+b)×L (ej. VF028: (2×0,35+0,25)×3,20=0,95×3,20=3,04).*

**Armadura** (cada viga tiene: barras longitudinales "A" de la familia principal (± una 2ª familia de refuerzo puntual en las vigas de 5,00m), barras inferiores "E", y estribos):

| Viga | Tipo | Ø (mm) | Cant. | L unit. (m) | L tot (m) | kg (c/desp) |
|---|---|---|---|---|---|---|
| VF028 | A | 12 | 3 | 3,44 | 10,32 | 10,10 |
| VF028 | E | 8 | 2 | 3,36 | 6,72 | 2,75 |
| VF028 | Estribo (paso 0,25, perímetro 1,20+2 ganchos 10Ø=1,32) | 6 | 14 | 1,32 | 18,48 | 4,27 |
| VF029 | *(idéntica a VF028, mismas dimensiones y armadura)* | | | | | 17,12 |
| VF086 | A (familia 1) | 16 | 2 | 5,32 | 10,64 | 19,33 |
| VF086 | A (familia 2, refuerzo puntual) | 12 | 1 | 5,24 | 5,24 | 5,13 |
| VF086 | E | 8 | 2 | 5,16 | 10,32 | 4,23 |
| VF086 | Estribo (paso 0,20, perímetro 1,20+2 ganchos 10Ø(Φ8)=1,36) | 8 | 26 | 1,36 | 35,36 | 14,48 |
| VF087 | *(idéntica a VF086)* | | | | | 43,17 |
| **TOTAL** | | | | | | **120,59** |

*Cantidad de estribos = redondeo hacia arriba(tramo/paso)+1 (ej. VF028: 3,20/0,25=12,8→13+1=14; VF086: 5,00/0,20=25+1=26). Verificado con Python: todos los kg y totales coinciden exactamente con la planilla oficial.*

**Resultados finales:**
- Total Vol. hormigón: **1,435 m³**
- Total encofrado: **15,58 m²**
- Total acero (con desperdicio): **120,59 kg**
- **Tenor de encofrado = 15,58/1,435 = 10,86 m²/m³**
- **Cuantía de acero = 120,59/1,435 = 84,03 kg/m³**

---

## II – Costo Financiero (25 pts)

**a) Definición:** el Valor Neto Actualizado (VNA) de una inversión a una tasa de descuento es la suma de los valores presentes de todos los flujos (ingresos y egresos) que la componen, traídos a valor presente con esa tasa. Da el monto que, en el momento presente, resulta equivalente a la totalidad del flujo considerado, por encima de los intereses ya descontados a esa tasa. Si VNA=0, la tasa usada ES la TIR del proyecto; si VNA>0, la inversión rinde una TIR mayor a la tasa de descuento; si VNA<0, rinde menos.

**b) Deuda de $3.000.000, 3 alternativas de pago, tasa trimestral 10%:**

| Trimestre | trim1 | trim2 | trim3 | trim4 | trim5 | Total nominal | **VNA (i=10%/trim)** |
|---|---|---|---|---|---|---|---|
| Deuda (referencia) | | | | | | 3.000 | **3.000** |
| Alternativa 1 | 1.100 | 1.100 | 500 | 500 | 500 | 3.700 | **2.937** |
| Alternativa 2 | 800 | 800 | 800 | 800 | 800 | 4.000 | **3.033** |
| Alternativa 3 | 0 | 0 | 0 | 0 | 5.000 | 5.000 | **3.105** |

*(montos en miles de $, VNA = Σ pago_t/(1,1)ᵗ)*

**b1) Orden de conveniencia (mayor a menor VNA):**
1. **Alternativa 3** (VNA=3.105) — mayor Valor Neto Actualizado.
2. Alternativa 2 (VNA=3.033).
3. **Alternativa 1** (VNA=2.937) — menor Valor Neto Actualizado.

**b2) Indemnización vs. costo del dinero:** comparando cada VNA contra el monto nominal de la deuda ($3.000): la **Alternativa 1** (VNA=2.937 < 3.000) **no** reconoce una indemnización suficiente — no llega a compensar el interés. Las **Alternativas 2 (3.033) y 3 (3.105)** sí tienen VNA superior a $3.000, siendo **mayor en la Alternativa 3**.

**b3) Ajuste del pago del trim5 en la Alternativa 3 para que reconozca EXACTAMENTE el costo del dinero** (VNA = $3.000, ni más ni menos): como el único pago es en trim5, X/(1,1)⁵ = 3.000 → **X = 3.000×(1,1)⁵ = $4.832 (miles)** en vez de los $5.000 originales.

---

## III – Garantías (15 pts)

**Datos:** Costo total=$600.000.000; Beneficio=18% sobre venta (P); IVA=22%; Monto Imponible mano de obra=$40.000.000; Aporte unificado (privada)=75,8%. Plazo de ejecución=6 meses; plazo de garantía (RP→RD)=12 meses. Costo del seguro de fianza: 1,5% anual del monto a garantizar.

**Precio de venta:** P = Costo/(1−0,18) = 600.000.000/0,82 = **$731.707.317**. IVA=22%×P=$160.975.610 → Venta c/IVA=**$892.682.927**. Leyes sociales=40.000.000×0,758=$30.320.000 → **Venta total IVA+LLSS = $923.002.927** (base para ambas garantías, que piden incluir IVA y leyes sociales).

| Garantía | Base | Monto a garantizar | Período | Monto medio garantizado | Costo (1,5% anual × monto medio × período/12) |
|---|---|---|---|---|---|
| **a) Fiel cumplimiento** | 10% de $923.002.927 (constante, I→RP) | $92.300.293 | 6 meses | $92.300.293 (fijo) | **$692.252** |
| **b) Buena ejecución** — tramo I→RP | 5% de cada certificado, crece linealmente | final: $46.150.146 | 6 meses | $23.075.073 (prom. triangular) | $173.063 |
| **b) Buena ejecución** — tramo RP→RD | monto ya completo, constante | $46.150.146 | 12 meses | $46.150.146 (fijo) | $692.252 |
| **b) Buena ejecución — TOTAL** | | | | | **$865.315** |

**Costo Total de garantías = 692.252 + 865.315 = $1.557.567**

---

## IV – Régimen Salarial (10 pts) *(teórico, sin solución oficial en el repo)*

Ver Guía sección 6 y desarrollo idéntico en `Soluciones/202307 Ex Julio/` y `Soluciones/202312 Ex diciembre/` (parte VI):

**a) Sistema de remuneración (Ley 14.411):** el personal de la construcción se remunera por jornal/hora según categoría y laudo del Convenio Colectivo (Grupo 37); los aportes patronales y obreros se centralizan en un **Aporte Unificado de la Construcción**, calculado como % sobre el Monto Imponible (en vez de liquidarse tarea por tarea) — simplifica la gestión dada la rotación característica de la mano de obra de obra.

**b) Convenio Colectivo (Grupo 37) — partes y contenido:** tripartito — Cámaras empresariales, **SUNCA** y **MTSS/Poder Ejecutivo** (homologa). Trata: categorías/laudos salariales, ajuste salarial periódico, licencia y aguinaldo, condiciones de trabajo/seguridad, Fondos Sociales de la Construcción.

---

## V – Materiales (15 pts) *(teórico, sin solución oficial en el repo)*

Ver Guía sección 14 (mismo criterio usado en Suministros de exámenes previos):

**a) Identificados:** especificación técnica clara y sin ambigüedad (normas, memorias descriptivas), marca/calidad de referencia si corresponde.

**b) Cuantificados:** unidad de medida coherente con la forma de compra/certificación, desperdicio explícito, cantidad surgida de un metraje verificable, plazo de entrega acorde al cronograma.

**c) Valorados:** precio unitario acorde a la unidad definida, cotización vigente de proveedor representativo, condiciones de pago y entrega comparables entre cotizaciones.

---

## Resumen ejecutivo del examen

| Parte | Resultado clave |
|---|---|
| I – Metraje | Vol=1,435 m³; Encof=15,58 m²; Tenor=10,86 m²/m³; Acero=120,59 kg; Cuantía=84,03 kg/m³ (4 vigas de fundación) |
| II – Costo Financiero | VNA: Alt.3 (3.105) > Alt.2 (3.033) > Alt.1 (2.937). Solo Alt.1 no compensa. Ajuste b3: pago trim5 = $4.832 (miles) para VNA exacto |
| III – Garantías | Fiel cumplimiento $692.252 + Buena ejecución $865.315 = **$1.557.567** |
| IV – Régimen Salarial | Aporte Unificado Ley 14.411; Convenio Colectivo tripartito |
| V – Materiales | Identificados / Cuantificados / Valorados |
