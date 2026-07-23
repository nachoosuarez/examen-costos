# Examen Costos — Diciembre 2023 (14/12/2023)

Verificado contra solución oficial (planilla de cálculo incluida en `Examen Costos 12-2023 - Preg. I,IIyIII.pdf` — cubre I, II y III). Las Partes IV, V y VI (teóricas) no vienen con solución oficial en el repo — se responden con el criterio de la Guía.

---

## I – Metraje (20 pts)

**Enunciado:** volumen de hormigón, tenor de encofrado y cuantía de hierro de la viga con alero del Anexo 1, largo 21m. Ganchos=10Φ; empalme 50cm (Φ6/Φ8), 70cm (Φ12); varilla comercial 12m.

**Perfil (ver Anexo 1, corte totalmente acotado — sin ambigüedad de "cruz" en este examen):** viga en forma de "L" con alero, dintel delgado y un relleno triangular (haunch) entre el alero y la viga. Se separa en 4 sub-elementos:

| Id | L (m) | b (m) | h (m) | V (m³) | Encof (m²) | Nota |
|---|---|---|---|---|---|---|
| Alero | 21 | 0,30 | 0,09 | **0,567** | 8,19 | ala horizontal delgada |
| Viga | 21 | 0,15 | 0,44 | **1,386** | 14,70 | alma vertical principal |
| Dintel | 21 | 0,10 | 0,07 | **0,147** | 1,47 | remate superior delgado |
| Triángulo | 21 | 0,10 | 0,17 | **0,180** | 4,14 | relleno de haunch, **volumen = ½×base×altura×L** (sección triangular, no rectangular) |
| **Total** | | | | **2,279** | **28,50** | |

**Armadura:**

| Tipo | Ø (mm) | Cant. | L unit. (m) | L tot (m) | kg (c/desp) |
|---|---|---|---|---|---|
| Long. viga (3Ø12 sup+3Ø12 inf) | 12 | 6 | 21,70 (21+0,70 empalme) | 130,20 | 127,47 |
| Long. dintel (2Ø6) | 6 | 2 | 21,50 (21+0,50 empalme) | 43,00 | 9,93 |
| Estribo viga (Ø8/15, perímetro 1,72m) | 8 | 141* | 1,72 | 265,08 | 108,55 |
| Estribo alero (Ø8/30, perímetro 0,97m) | 8 | 71* | 0,97 | 80,03 | 32,77 |

*Cantidad de estribos = redondeo hacia arriba(21/paso)+1: viga (paso 0,15) → 21/0,15+1=141; alero (paso 0,30) → 21/0,30+1=71. Los dos tipos de estribo cubren la misma longitud total (21m) con distinto paso y distinto perímetro (envuelven secciones distintas del corte).

**Resultados finales:**
- Total Vol. hormigón: **2,279 m³**
- Total encofrado: **28,50 m²**
- Total acero (con desperdicio): **278,72 kg**
- **Tenor de encofrado = 28,50/2,279 = 12,51 m²/m³**
- **Cuantía de acero = 278,72/2,279 = 122,33 kg/m³**

*(Tenor y cuantía altos, esperable: es una viga muy esbelta con dos zonas de estribo denso y varios sub-elementos delgados — mucha superficie de encofrado y hierro relativo a un volumen de hormigón chico.)*

---

## II – Consumos (10 pts)

**Rendimientos:** Of.Carpintero/Ayudante 2,00 hs/m³ pasta c/u + 1,25 hs/m² encofrado c/u; Of.Herrero/Ayudante 0,04 hs/kg hierro c/u. Tabla de pino 2,40×0,15m, desperdicio 10%, 3 reúsos.

| Insumo | Fórmula | Cons. Unitario /m³ | Consumo Total (×2,279 m³) |
|---|---|---|---|
| Ayudante (hs) | 2,00 + 12,51×1,25 + 122,33×0,04 | **22,53** | 51,33 |
| Oficial Carpintero (hs) | 2,00 + 12,51×1,25 | **17,64** | 40,18 |
| Oficial Herrero (hs) | 122,33×0,04 | **4,89** | 11,15 |
| Hormigón premezclado (m³) | 1×1,05 | **1,05** | 2,39 |
| Hierro (kg) | = Cuantía | **122,33** | 278,72 |
| Tabla de pino (unid) | (12,51×1,10)/(0,40×3) | **12,74** | 29,03 |

**HH/m³ total:** 22,53+17,64+4,89 = **45,06 hs/m³** (el más alto de todos los exámenes vistos hasta ahora, consistente con el tenor/cuantía altos de esta viga).

---

## III – Costo Financiero (20 pts)

**Enunciado:** presupuesto/cronograma de una obra (ingresos $20.000.000 totales, egresos $17.000.000 totales, en miles de $ en la tabla). El cliente entrega un **anticipo del 10%** del precio total (mes 0), que el contratista devuelve como quita del 10% en cada cobro posterior. Se pide el flujo con anticipo, elegir entre 2 líneas de crédito (Línea 1: $4.000.000 al 4%/mes; Línea 2: $8.000.000 al 5%/mes) y calcular intereses y monto máximo usado.

**a) Flujo con anticipo, sin costo financiero (miles $):**

| | mes0 | mes1 | mes2 | mes3 | mes4 | mes5 | mes6 | Total |
|---|---|---|---|---|---|---|---|---|
| Ingresos sin anticipo | | | 4.100 | 4.100 | 4.100 | 4.100 | 3.600 | 20.000 |
| Anticipo 10% (recibido mes0, devuelto como quita en cada cobro) | +2.000 | | −410 | −410 | −410 | −410 | −360 | 0 |
| Ingresos netos | 2.000 | 0 | 3.690 | 3.690 | 3.690 | 3.690 | 3.240 | 20.000 |
| Egresos | −1.000 | −2.500 | −4.000 | −4.000 | −5.500 | | | −17.000 |
| **Flujo mensual** | 1.000 | −2.500 | −310 | −310 | −1.810 | 3.690 | 3.240 | 3.000 |
| **Flujo acumulado** | **1.000** | **−1.500** | **−1.810** | **−2.120** | **−3.930** | −240 | 3.000 | |

*(Todos los valores se toman a fin de mes, según lo indicado en el enunciado.)*

**b) Elección de línea de crédito:** a simple vista, el máximo déficit acumulado sin intereses (−3.930, mes4) queda **por debajo** del límite de la Línea 1 ($4.000), así que en principio alcanzaría. **Pero al incorporar el costo financiero de usar la línea, el propio interés hace crecer el déficit acumulado por encima de los $4.000** (llega a −4.147 en el mes4 con la Línea 1) — la línea 1 termina no alcanzando para cubrirse a sí misma. Por eso **hay que usar la Línea 2** ($8.000, 5%/mes), que sí tiene margen suficiente.

**Costo financiero con Línea 1 (4%/mes, interés = 4%×|déficit acumulado del mes anterior|):**

| | mes1 | mes2 | mes3 | mes4 | mes5 | mes6 | Total |
|---|---|---|---|---|---|---|---|
| Costo financiero | 0 | −60 | −72 | −85 | −157 | −10 | **−384** |
| Flujo acumulado (con interés) | 1.000 | −1.870 | −2.252 | **−4.147** ⚠ (supera $4.000) | −614 | 2.616 | |

**Costo financiero con Línea 2 (5%/mes):**

| | mes1 | mes2 | mes3 | mes4 | mes5 | mes6 | Total |
|---|---|---|---|---|---|---|---|
| Costo financiero | 0 | −75 | −91 | −106 | −197 | −12 | **−480** |
| Flujo acumulado (con interés) | 1.000 | −1.885 | −2.286 | **−4.202** | −708 | 2.520 | |

**c) Monto total de intereses previstos a pagar (con la Línea 2, la efectivamente usada): $ −480 (miles)**

**d) Monto máximo a utilizar de la Línea 2, incluyendo intereses: $ −4.202 (miles)** — el peor momento de caja, en el mes 4. *(De ese monto, $272 mil corresponden a intereses acumulados hasta ese punto — el resto, $3.930 mil, es el déficit operativo puro.)*

---

## IV – Varios (15 pts) *(teórico, sin solución oficial en el repo)*

**a) Fórmulas paramétricas** — ver Guía sección 8 (finalidad y expresión genérica `Pₙ=P₀×[a₀+a₁(Jₙ/J₀)+a₂(M1ₙ/M1₀)+…]`, con Σaᵢ=1).

**b) Los 3 coeficientes de movimiento de tierra y su relación** — ver Guía sección 13: Esponjamiento (Ce)=Vol.suelto/Vol.banco (>1); Compactación (Cc)=Vol.compactado/Vol.banco (<1); Aporte (Ca)=Vol.compactado/Vol.suelto. Relación: **Ca = Cc/Ce**.

**c) Grupos de costos por Naturaleza** — ver Guía sección 15: Costos Directos (Mano de Obra, Materiales, Equipos, Suministros y Subcontratos, Varios) + Costos Indirectos (dirección de obra, administración, obrador, seguros/garantías, gastos generales prorrateados).

---

## V – Materiales (15 pts) *(teórico, sin solución oficial en el repo)*

**Qué debe tenerse presente para que los materiales estén correctamente…**

**a) Identificados:** especificación técnica clara y sin ambigüedad (normas, memorias descriptivas), marca/calidad de referencia si corresponde, y los incumplimientos posibles ya previstos y valorados contractualmente.

**b) Cuantificados:** unidad de medida bien definida (coherente con cómo se compra/certifica el insumo), criterio de desperdicio explícito, cantidad total surgida de un metraje verificable, y plazo de entrega necesario acorde al cronograma de obra.

**c) Valorados:** precio unitario acorde a la unidad de medida definida, con cotización vigente (no desactualizada) y de un proveedor real/representativo, considerando condiciones de pago y entrega comparables entre cotizaciones.

*(Ver Guía sección 14 — mismo criterio ya usado para Suministros.)*

---

## VI – Régimen Salarial (10 pts) *(teórico, sin solución oficial en el repo)*

Ver Guía sección 6 y desarrollo idéntico en `Soluciones/202402 Ex febrero/` (parte VI): Aporte Unificado de la Construcción (Ley 14.411), remuneración por categorías/laudos del Convenio Colectivo, Monto Imponible, Fondos Sociales de la Construcción. Convenio Colectivo (Grupo 37) tripartito: Empresas, Trabajadores (SUNCA), MTSS/Poder Ejecutivo (homologa); trata categorías/laudos, ajuste salarial, licencias, condiciones de trabajo y Fondos Sociales.

---

## Resumen ejecutivo del examen

| Parte | Resultado clave |
|---|---|
| I – Metraje | Vol=2,279 m³; Encof=28,50 m²; Tenor=12,51 m²/m³; Acero=278,72 kg; Cuantía=122,33 kg/m³ |
| II – Consumos | Ayudante 22,53 hs/m³; HH/m³ total=45,06 (el más alto visto hasta ahora) |
| III – Costo Financiero | Línea 1 insuficiente (el interés la hace superar su propio límite) → usar **Línea 2**: intereses totales $480 mil, uso máximo $4.202 mil (mes 4) |
| IV – Varios | Fórmula paramétrica, coeficientes Ce/Cc/Ca (Ca=Cc/Ce), costos por naturaleza |
| V – Materiales | Identificados / Cuantificados / Valorados |
| VI – Régimen Salarial | Aporte Unificado Ley 14.411; Convenio Colectivo tripartito |
