# Examen Costos (2240) — 03/12/2019

Fuente: `Exámenes/201912 Ex diciembre/Examen Costos 12-2019.pdf` (letra) + `Examen Costos 12-2019 Anexo I.pdf` (croquis) + `Examen Costos Dic-2019 Respuestas.pdf` (solución oficial de I, II y III). **Partes I, II y III verificadas exactas contra la solución oficial. Partes IV, V y VI son teóricas, sin solución oficial en el repo (respondidas con el criterio de la Guía).**

## Enunciado resumido

- **I. Metraje Hormigón (25 pts):** volumen, cuantía de hierro y tenor de encofrado de un muro de contención en "T invertida" (croquis Anexo I): pata de 3,00 m + pantalla vertical de 3,95 m, panel de 6,00 m de longitud.
- **II. Costo Componentes del Hormigón (15 pts):** costo del m³ de hormigón por dosificación en volumen (4:3:1, pedregullo:arena:cemento) + relación agua/cemento.
- **III. Garantías (15 pts):** costo de Fiel Cumplimiento, Buena Ejecución y Anticipo, con Leyes Sociales dadas como monto fijo (no %).
- **IV. Varios (15 pts):** actores del mercado de la construcción; TIR en dos casos particulares de flujo; partidas "Incentivo Asistencia" y "FOCER" de la Ley 14.411.
- **V. Suministros (10 pts):** información necesaria para identificar/cuantificar/valorar suministros.
- **VI. Estado Económico y Financiero (10 pts):** Cronograma Económico vs. Financiero de una obra.

---

## I. Metraje — Muro de contención en T invertida

**Geometría (Anexo I):** panel de 6,00 m de longitud (plan). Corte A-A: pata (zapata corrida) de sección 3,00×0,40 m (0,30+0,40+2,30 repartidos en el ancho); pantalla vertical de 0,40 m de espesor × 3,95 m de altura, centrada sobre la pata. A diferencia del muro "por trincheras" de Marzo-2020 (donde solo se encofra 1 cara porque la excavación genera taludes naturales continuos), acá **es un panel aislado de longitud finita** — se encofran **las 2 caras + los 2 extremos** (perímetro completo), no solo la cara vista.

**a) Volumen de hormigón:**

| Elemento | b/Ancho (m) | h/Espesor (m) | L (m) | V (m³) |
|---|---|---|---|---|
| Pata (3,00 de ancho total × 0,40 de alto) | 3,00 | 0,40 | 6,00 | 7,20 |
| Pantalla (0,40 de espesor × 3,95 de alto) | 0,40 | 3,95 | 6,00 | 9,48 |
| **Total** | | | | **16,68** |

**c) Encofrado — panel aislado, se encofra el perímetro completo (2 caras + 2 extremos) de cada elemento:**

| Elemento | Fórmula (perímetro×altura) | Encof (m²) |
|---|---|---|
| Pata | 2×(3,00+6,00)×0,40 | 7,20 |
| Pantalla | 2×(6,00+0,40)×3,95 | 50,56 |
| **Total** | | **57,76** |

**Tenor = 57,76 / 16,68 = 3,46 m²/m³** (bajo, típico de un elemento macizo tipo muro, ver Guía sección 1).

**b) Acero — planilla oficial** (recubrimiento 2 cm, ganchos en todos los hierros, varilla comercial 12 m, desperdicio 5-15% según diámetro de la tabla del examen):

| Ø | Cant. | Long. unitaria (m) | Long. total (m) | kg sin desp. | kg con desp. |
|---|---|---|---|---|---|
| 12 | 15 | 6,20 | 93 | 83 | 91 |
| 10 | 15 | 6,16 | 92 | 57 | 63 |
| 10 | 20 | 6,16 | 123 | 76 | 84 |
| 12 | 20 | 6,20 | 124 | 110 | 121 |
| 16 | 30 | 3,51 | 105 | 166 | 191 |
| 10 | 30 | 3,39 | 102 | 63 | 69 |
| 16 | 30 | 5,13 | 154 | 243 | 280 |
| 10 | 30 | 4,21 | 126 | 78 | 86 |
| **Total** | | | | **878** | **986** |

*(La "longitud unitaria" de cada barra = longitud recta + anclaje(s) en el plano − descuento por recubrimiento (2×2cm=0,04m); las familias con "Ø16/30" y "Ø10/30" corresponden a las barras horizontales de la pantalla —Ø10/20 y Ø12/20 horizontal en el croquis, contadas a lo largo de los 3,95m de altura, paso 20cm— y las de "Ø12/15,20" y "Ø10/15,20" a las longitudinales/verticales y de la pata. **Nota de la propia solución oficial:** con varillas de 12m para hierros de poco más de 6m sobra mucho material — en la práctica convendría replanificar el corte usando varillas de 6m para reducir desperdicio, aunque el examen pide usar 12m para todos los diámetros.)*

**Cuantía = 986 / 16,68 = 59,1 kg/m³** (sin desperdicio: 878/16,68 = 52,6 kg/m³).

---

## II. Costo de Componentes del Hormigón

**Datos:** relación en volumen 4(pedregullo):3(arena):1(cemento). Relación agua/cemento = 0,50 lt/kg. Densidad aparente del cemento = 1.400 kg/m³.

**Paso a paso:**
1. **Volumen real de cada árido** = Volumen aparente (de la relación) × Coeficiente de Aporte: Pedregullo = 4×0,55 = 2,200; Arena = 3×0,57 = 1,710; Cemento = 1×0,47 = 0,470.
2. **Volumen de agua:** 1 m³ aparente de cemento pesa 1.400 kg (densidad aparente) → agua = 1.400 kg × 0,50 lt/kg = 700 lt = **0,700 m³** por cada unidad de la relación de cemento (coeficiente de aporte del agua = 1, no reduce volumen).
3. **Suma de volúmenes reales** = 2,200+1,710+0,470+0,700 = **5,08** — este es el volumen aparente total (de todos los componentes juntos) que, al mezclarse (los finos rellenan los huecos de los gruesos), produce **1 m³ de hormigón compactado real** (por eso se usa como divisor).
4. **Volumen aparente de cada componente necesario para 1 m³ real de hormigón** = Volumen aparente de la relación (paso 1, ej. 4 para pedregullo) / Suma (5,08): Pedregullo = 4/5,08 = 0,787 m³; Arena = 3/5,08 = 0,591 m³; Cemento = 1/5,08 = 0,197 m³ → en kg: 0,197×1.400 = **276 kg**; Agua = 0,700/5,08 = 0,138 m³ = **138 lt**.
5. **Verificación:** los volúmenes REALES (no aparentes) de cada componente sobre la Suma deben sumar 1: 2,2/5,08+1,71/5,08+0,47/5,08+0,7/5,08 = 0,433+0,337+0,093+0,138 = 1,00 ✓.
6. **Costo** = cantidad necesaria por m³ (paso 4) × costo unitario:

| Componente | Cantidad /m³ | Costo unitario | Costo |
|---|---|---|---|
| Pedregullo | 0,787 m³ | 600 $/m³ | 472,20 |
| Arena Gruesa | 0,591 m³ | 500 $/m³ | 295,50 |
| Cemento | 276 kg (=11,04 bolsas de 25kg) | 10 $/kg (250$/bolsa÷25kg) | 2.760,00 |
| Agua | 138 lt | — (sin costo) | 0,00 |
| **Costo total del m³ de hormigón** | | | **$ 3.527,70** |

---

## III. Garantías

**Datos de base:** Costo=$200.000.000; Beneficio=15% **sobre venta** ⇒ `P = Costo/(1−0,15) = $235.294.118`; IVA 22% = $51.764.706; **Leyes Sociales dadas directamente como monto fijo = $30.000.000** (a diferencia de otros exámenes, acá NO hay que estimar un Monto Imponible ni aplicar un % — se suma tal cual). **Precio total (IVA y LLSS incl.) = $317.058.824.** Costo de constitución (Fianza BSE): **2,0% anual** del monto a garantizar (más alto que el 1,5% visto en otros exámenes — leer siempre el dato del examen, no asumir el valor de memoria).

**a) Fiel Cumplimiento** — 5% del precio final, fijo, 12 meses (I→RP):
`Monto = 5%×317.058.824 = $15.852.941` → `Costo = 15.852.941×2,0% = **$317.059**`.

**b) Buena Ejecución (fondo de reparo)** — 5% de cada certificado (rampa 0→5% durante los 12 meses de obra), luego constante al 5% durante los 12 meses de garantía (RP→RD, **acá el plazo de garantía es 12 meses, no 24 como en Marzo-2020** — leer el dato de cada examen):
- Tramo I→RP: monto medio = 5%/2×317.058.824 = $7.926.471 → costo = ×2,0% = **$158.529**.
- Tramo RP→RD: monto medio = 5%×317.058.824 = $15.852.941 → costo = ×2,0%×1 año = **$317.059**.
- **Costo total Buena Ejecución = $475.588.**

**c) Anticipo** — 100% del anticipo (10% del precio sin IVA), garantizado con **4 documentos de 25% cada uno**, devueltos a medida que se desacopia cada 25% (mismo patrón "escalonado por tramos" de Marzo-2020):
Anticipo = 10%×235.294.118 = $23.529.412. Monto pendiente por tramo trimestral: 10%/7,5%/5%/2,5% del precio → monto medio mensual = promedio de los 4 tramos = **$14.705.882**. Costo = 14.705.882×2,0% (12 meses) = **$294.118**.

**Costo total de garantías = 317.059+475.588+294.118 = $1.086.765** (el 0,54% del costo de obra — dentro del rango esperable 0,5%-1,5%, ver Guía sección 7).

---

## IV. Varios (sin solución oficial — teórico, criterio de la Guía)

**a) Actores del mercado de la construcción:** Cliente/Comitente (público o privado); Contratista principal (empresa constructora); Subcontratistas (por especialidad: instalaciones, estructura, terminaciones); Proveedores de materiales y equipos; Proyectista/Diseñador (arquitecto, ingeniero); Dirección de Obra (supervisión técnica, en representación del comitente); Organismos de contralor y financiamiento (BSE, BPS, bancos que otorgan garantías/créditos); Trabajadores/Mano de obra (amparados por SUNCA y la Ley 14.411).

**b) TIR en dos casos particulares:**
- **b1) Flujo acumulado (sin descontar) al último período = 0:** la TIR de ese flujo es **0%**. Por definición, la TIR es la tasa `i` para la cual `VNA(i)=Σ Flujo_t/(1+i)^t = 0`. Si con `i=0%` (sin descuento, `(1+i)^t=1` para todo t) la suma simple de los flujos ya da 0, entonces `i=0%` cumple exactamente la condición de la TIR.
- **b2) Ingresos ≥ Egresos en TODOS los períodos (con el primer período exactamente en 0):** en este caso **la TIR no existe (es indefinida)**. Como nunca hay un período con flujo neto negativo (no hay una "inversión" que recuperar), el VNA(i) es **siempre ≥ 0 para cualquier tasa i≥0** — no hay ninguna tasa que lo lleve a 0 (salvo el caso trivial de que todos los flujos sean nulos). Es un caso típico de "trampa teórica": un proyecto sin desembolso neto no tiene una TIR calculable en el sentido usual.

**c) Partidas de la Ley 14.411 (régimen salarial de la construcción):**
- **c1) Incentivo por Asistencia:** partida adicional al jornal básico, pagada como premio por presentismo/asistencia perfecta del trabajador durante el período (no falta ni llega tarde); se cuantifica como un % adicional sobre el jornal básico de las categorías amparadas, integrando el monto imponible igual que el resto de la remuneración.
- **c2) FOCER (Fondo de Cesantía de la Industria de la Construcción):** aporte patronal adicional dentro del régimen de la Ley 14.411, destinado a financiar una prestación/fondo de cesantía específico para los trabajadores del sector — compensa la alta rotación e intermitencia propia de la actividad (los trabajadores cambian de obra en obra y suelen quedar cesantes al finalizar cada una), a diferencia del seguro de paro común administrado por BPS.

## V. Suministros (sin solución oficial — teórico, criterio de la Guía)

Para que los suministros de una obra estén correctamente:
- **Identificados:** especificación técnica precisa (marca/tipo/norma exigida en planos y pliego), evitando ambigüedad en qué se está cotizando/comprando.
- **Cuantificados:** metraje/cómputo a partir de planos y planillas, incluyendo desperdicios y mermas de manipuleo/colocación — nunca el metraje neto de proyecto sin más.
- **Valorados:** cotización a precio de mercado vigente (varios proveedores), incluyendo todos los costos hasta disponibilidad en obra (flete, seguro, impuestos/aranceles si es importado, acopio, mermas de estadía).

## VI. Estado Económico y Financiero (sin solución oficial — teórico, criterio de la Guía)

**a) Cronograma Económico** = distribución en el tiempo de los **ingresos y costos devengados** (lo que se certifica/incurre según el avance real de obra, independientemente de cuándo se cobra/paga). **Cronograma Financiero** = distribución en el tiempo de los **ingresos y egresos de caja** (cuándo efectivamente se cobra y se paga, considerando plazos de pago, anticipos, retenciones — ver Guía sección 12, variante "Marzo"-2023).

**b) Importancia y qué controla cada uno:** el Cronograma Económico controla la **rentabilidad** del contrato (si el margen/beneficio previsto se está cumpliendo a medida que avanza la obra, comparando lo devengado contra lo presupuestado). El Cronograma Financiero controla la **liquidez** (si la empresa cuenta con caja suficiente en cada momento para afrontar sus compromisos, y cuánto financiamiento externo —línea de crédito— necesita en los meses de descubierto). Ambos son necesarios porque una obra puede ser económicamente rentable y sin embargo tener problemas financieros de caja (o viceversa) — son controles de naturaleza distinta y complementaria.

---

## Resumen de resultados

| Parte | Resultado |
|---|---|
| I.a Volumen hormigón | **16,68 m³** |
| I.b Acero | **986 kg** — Cuantía **59,1 kg/m³** |
| I.c Encofrado | **57,76 m²** — Tenor **3,46 m²/m³** |
| II Costo del m³ de hormigón | **$3.527,70/m³** |
| III.a Fiel Cumplimiento | **$317.059** |
| III.b Buena Ejecución | **$475.588** |
| III.c Anticipo | **$294.118** |
| III Total garantías | **$1.086.765** (0,54% del costo) |
