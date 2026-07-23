# Examen Costos — Julio 2023 (26/07/2023)

Verificado contra solución oficial (planilla de cálculo incluida en `Examen Costos 07-2023 - Preg. I,II,III,IV y V.pdf` — cubre I, II, III, IV y V). La Parte VI (teórica) no viene con solución oficial en el repo — se responde con el criterio de la Guía.

---

## I – Metraje (20 pts)

**Enunciado:** volumen de hormigón, tenor de encofrado y cuantía de hierro del muro de contención del Anexo 1, longitud 20m. Ganchos=10Φ; empalme 50cm (Φ6/Φ8), 70cm (Φ12); varilla comercial 12m; recubrimientos despreciados.

**Perfil (ver Anexo 1):** muro de contención monolítico en forma de "L" — pantalla vertical + pie de zapata corrido, sin bloques (mismo tipo que Feb-2025, ver Guía sección 1). Se separa en 2 sub-elementos:

| Id | L (m) | b (m) | h (m) | V (m³) | Encof (m²) |
|---|---|---|---|---|---|
| Muro (pantalla) | 20 | 0,15 | 2,80 | **8,400** | 112,00 (2 caras × 2,80 × 20) |
| Pie de muro (zapata) | 20 | 1,75 | 0,15 | **5,250** | 6,00 (2 caras × 0,15 × 20 — solo cantos, apoya en el suelo) |
| **Total** | | | | **13,650** | **118,00** |

**Armadura** (planilla oficial, reconstruida fórmula a fórmula):

| Tipo (según croquis) | Ø (mm) | Tramo/Paso | Cant. | L unit. (m, c/ganchos) | Empalmes | L tot (m) | kg (c/desp) |
|---|---|---|---|---|---|---|---|
| "Estribo interior" — vertical Ø12 c/15, ancla en el pie (armadura principal a flexión de la pantalla) | 12 | 20,00 / 0,15 | 135 | 5,69 | 0 | 768,15 | **752,02** |
| "Long. muro" — horizontal Ø6 c/15 en la pantalla (repartición) | 6 | 2,80 / 0,15 | 19 | 20,00 | 19 (×0,50m) | 389,50 | **89,97** |
| "Long. inf pie" — longitudinal inferior del pie, Ø8 c/20 | 8 | 1,75 / 0,20 | 10 | 20,00 | 10 (×0,50m) | 205,00 | **83,95** |
| "Long. sup pie" — longitudinal superior del pie, Ø8 c/20 | 8 | 1,75 / 0,20 | 10 | 20,00 | 10 (×0,50m) | 205,00 | **83,95** |
| "Estribo inferior pie" — estribo transversal del pie (ata longitudinal inf+sup), Ø8 c/15 | 8 | 20,00 / 0,15 | 135 | 2,21 | 0 | 298,35 | **122,17** |
| **TOTAL** | | | | | | | **1132,06** |

*Método: Cant.=redondeo(tramo/paso)+1 (regla de oro #3 de la Guía). Las barras "longitudinales" del pie corren los 20m del muro → superan la varilla comercial de 12m, por eso llevan 1 empalme de 0,50m c/u (ant. empalm = cant., cada barra empalma 1 vez). Las barras "verticales" (Ø12, L=5,69m) y los "estribos" del pie (Ø8, L=2,21m) son piezas cortas prefabricadas por unidad → sin empalme, con sus ganchos ya incluidos en la L unitaria. Verificado con Python: todos los kg coinciden exactamente con la planilla oficial.*

**Resultados finales:**
- Total Vol. hormigón: **13,650 m³**
- Total encofrado: **118,00 m²**
- Total acero (con desperdicio): **1132,06 kg**
- **Tenor de encofrado = 118,00/13,650 = 8,64 m²/m³**
- **Cuantía de acero = 1132,06/13,650 = 82,93 kg/m³**

*(Tenor y cuantía bajos — coherente con un elemento macizo tipo muro, como ya se vio en Feb-2025: menos superficie de encofrado y menos densidad de armado relativos al volumen, comparado con una losa.)*

---

## II – Consumos (10 pts)

**Ojo — inconsistencia del enunciado:** el texto pide consumos "para la viga del Anexo 1", pero el Anexo 1 es el muro de contención de la Parte I (no hay ninguna viga en el examen) y la planilla de rendimientos, aunque en la letra dice "Vigas", en la solución oficial aparece re-etiquetada como "Muros" con los mismos valores. Se resuelve para el **muro** de la Parte I (tenor=8,64 m²/m³, cuantía=82,93 kg/m³), como hizo la solución oficial.

**Rendimientos:** Of.Carpintero/Ayudante 2,00 hs/m³ pasta c/u + 1,25 hs/m² encofrado c/u; Of.Herrero/Ayudante 0,04 hs/kg hierro c/u. Tabla de pino 2,40×0,15m (área=0,36 m²), desperdicio 10%, 3 reúsos. Desperdicio hormigón premezclado 5%.

| Insumo | Fórmula | Cons. Unitario /m³ | Consumo Total (×13,65 m³) |
|---|---|---|---|
| Ayudante (hs) | 2,00 + 8,64×1,25 + 82,93×0,04 | **16,12** | 220,08 |
| Oficial Carpintero (hs) | 2,00 + 8,64×1,25 | **12,81** | 174,80 |
| Oficial Herrero (hs) | 82,93×0,04 | **3,32** | 45,28 |
| Hormigón premezclado (m³) | 1×1,05 | **1,05** | 14,33 |
| Hierro (kg) | = Cuantía | **82,93** | 1132,06 |
| Tabla de pino (unid) | (8,64×1,10)/(0,36×3) | **8,80** | 120,19 |

**HH/m³ total:** 16,12+12,81+3,32 = **32,25 hs/m³**.

---

## III – Costo Financiero (20 pts)

**a) Definición:** el Valor Neto Actualizado (VNA) de una inversión a una tasa de descuento *i* es la suma de todos los flujos de fondos futuros de esa inversión, cada uno descontado (traído a valor presente) a la tasa *i*, más el flujo inicial (si lo hay): VNA = Σ CFₜ/(1+i)ᵗ. Permite comparar montos que ocurren en distintos momentos del tiempo en una única base comparable (ver Guía sección 12).

**b) Deuda de $1.000.000, 3 alternativas de pago, tasa trimestral 20%:**

| Trimestre | trim1 | trim2 | trim3 | trim4 | trim5 | Total nominal | **VNA (i=20%/trim)** |
|---|---|---|---|---|---|---|---|
| Deuda (referencia) | | | | | | 1.000 | **1.000** |
| Alternativa 1 | 400 | 300 | 300 | 200 | 200 | 1.400 | **892** |
| Alternativa 2 | 350 | 350 | 350 | 300 | 300 | 1.650 | **1.003** |
| Alternativa 3 | 0 | 0 | 0 | 0 | 2.000 | 2.000 | **804** |

*(VNA = Σ pago_t/(1,2)ᵗ, montos en miles de $. Todos los pagos a fin de trimestre.)*

**b1) Orden de conveniencia para la constructora (mayor a menor VNA):**
1. **Alternativa 2** (VNA=1.003) — mayor Valor Neto Actualizado.
2. Alternativa 1 (VNA=892).
3. **Alternativa 3** (VNA=804) — menor Valor Neto Actualizado.

**b2) Indemnización vs. costo del dinero:** comparando cada VNA contra el monto nominal de la deuda ($1.000, la referencia "no descontada"): solo la **Alternativa 2** tiene un VNA (1.003) que iguala/supera los $1.000 — es la única que le reconoce a la constructora una indemnización que compensa aproximadamente el costo del dinero (el interés que dejó de percibir por cobrar tarde). Las **Alternativas 1 y 3** tienen VNA por debajo de $1.000 → no llegan a compensar el interés, la deuda se termina cobrando "desvalorizada" en términos financieros, con pérdida real para la constructora.

---

## IV – Garantías (15 pts)

**Datos:** Costo sin IVA=$100.000.000; Beneficio=12% sobre precio de venta (P); IVA=22%; Mano de obra imponible=$30.000.000; obra pública → coeficiente de leyes sociales (ley 14.411) = 71,8%. Plazo de ejecución=10 meses; plazo de garantía (RP→RD)=18 meses. Costo del seguro de fianza: 2,5% anual del monto a garantizar.

**Precio de venta:** como Beneficio=12%×P → P = Costo/(1−0,12) = 100.000.000/0,88 = **$113.636.364** (sin IVA). IVA=22%×P=$25.000.000 → Venta c/IVA=**$138.636.364**. Leyes sociales=30.000.000×0,718=$21.540.000 → **Venta total IVA+llss = $160.176.364** (base para las garantías a) y b), que piden incluir IVA y llss).

| Garantía | Base | Monto a garantizar | Período garantizado | Monto medio garantizado | Costo (2,5% anual × monto medio × período/12) |
|---|---|---|---|---|---|
| **a) Fiel cumplimiento** | 10% de $160.176.364 (constante desde el Inicio hasta la Recepción Provisoria) | $16.017.636 | 10 meses (I→RP) | $16.017.636 (monto fijo, no crece) | **$333.701** |
| **b) Buena ejecución** — tramo I→RP | 5% de cada certificado, certificación uniforme → crece linealmente de 0 al monto final durante la ejecución | final: $8.008.818 | 10 meses (I→RP) | $4.004.409 (promedio triangular) | $83.425 |
| **b) Buena ejecución** — tramo RP→RD | monto ya completo, se mantiene constante hasta la recepción definitiva | $8.008.818 | 18 meses (RP→RD) | $8.008.818 (monto fijo) | $300.331 |
| **b) Buena ejecución — TOTAL** | | | | | **$383.756** |
| **c) Anticipo** | 15% de $113.636.364 (sin IVA ni llss), se devuelve linealmente mes a mes durante la ejecución | $17.045.455 | 10 meses (I→RP) | $8.522.727 (promedio triangular decreciente) | **$177.557** |

**Costo Total de garantías = 333.701 + 383.756 + 177.557 = $895.014**

*(Perfiles temporales: fiel cumplimiento = escalón constante que cae a cero en RP; buena ejecución = rampa ascendente durante la ejecución que se mantiene plana hasta RD; anticipo = rampa descendente desde el Inicio hasta RP. Ver Guía sección 7.)*

---

## V – Punto de Equilibrio (15 pts)

**a) Definición:** el Punto de Equilibrio de un sistema de producción es el nivel de producción/venta en el cual los Ingresos totales igualan a los Costos totales (fijos + variables) — el beneficio es nulo. Por debajo de ese nivel la operación da pérdida, por encima da ganancia (ver Guía sección 11).

**Datos:** Costo fijo=$250.000/mes → **$3.000.000/año**; Costo variable unitario=$15/u; Producción máxima=1.500.000 u/año.

**b) Precio de venta para que el equilibrio se dé al 50% de la capacidad:**
Producción de equilibrio = 50%×1.500.000 = **750.000 u/año**.
En el equilibrio: Ingresos = Costos → P×Q_eq = CF + CV×Q_eq → **P = CF/Q_eq + CV = 3.000.000/750.000 + 15 = 4 + 15 = $19,00/u**

**c) Margen máximo posible (vendiendo el 100% de la capacidad, al precio recién fijado):**
Beneficio = (Q_max − Q_eq) × (P − CV) = (1.500.000 − 750.000) × (19 − 15) = 750.000 × 4 = **$3.000.000/año**

*(Equivalente a: Ingresos totales 19×1.500.000=28.500.000 − Costos totales (3.000.000+15×1.500.000)=25.500.000 = 3.000.000.)*

---

## VI – Régimen Salarial (10 pts) *(teórico, sin solución oficial en el repo)*

Ver Guía sección 6 y desarrollo idéntico en `Soluciones/202312 Ex diciembre/` y `Soluciones/202402 Ex febrero/` (parte VI):

**a) Sistema de remuneración (Ley 14.411):** el personal de la construcción se remunera por **jornal/hora**, según categoría y laudo del Convenio Colectivo (Grupo 37); los aportes patronales y obreros a la seguridad social, seguro de accidentes, fondo de desempleo, etc. se centralizan en un **Aporte Unificado de la Construcción**, calculado como % sobre el Monto Imponible (jornales + beneficios sociales), en vez de liquidarse tarea por tarea como en otros sectores — simplifica la gestión dado el carácter transitorio/rotativo de la mano de obra de obra.

**b) Convenio Colectivo de la Construcción (Grupo 37) — partes y contenido:** es tripartito — **Cámaras empresariales**, **SUNCA** (sindicato de trabajadores) y **MTSS/Poder Ejecutivo** (convoca los Consejos de Salarios y homologa el acuerdo). Trata: categorías y laudos salariales por oficio, ajuste/actualización salarial periódica, licencia y aguinaldo, condiciones de trabajo y seguridad, y los Fondos Sociales de la Construcción (vivienda, salud, capacitación).

---

## Resumen ejecutivo del examen

| Parte | Resultado clave |
|---|---|
| I – Metraje | Vol=13,650 m³; Encof=118,00 m²; Tenor=8,64 m²/m³; Acero=1132,06 kg; Cuantía=82,93 kg/m³ (muro de contención monolítico en L) |
| II – Consumos | Ayudante 16,12 hs/m³; HH/m³ total=32,25. Ojo: enunciado dice "viga" pero corresponde al muro de la Parte I. |
| III – Costo Financiero | VNA: Alt.2 (1.003) > Alt.1 (892) > Alt.3 (804). Solo Alt.2 compensa el costo del dinero. |
| IV – Garantías | Fiel cumplimiento $333.701 + Buena ejecución $383.756 + Anticipo $177.557 = **$895.014** |
| V – Punto de Equilibrio | Precio equilibrio al 50% capacidad = $19,00/u; margen máximo al 100% capacidad = $3.000.000/año |
| VI – Régimen Salarial | Aporte Unificado Ley 14.411; Convenio Colectivo tripartito (Cámaras, SUNCA, MTSS) |
