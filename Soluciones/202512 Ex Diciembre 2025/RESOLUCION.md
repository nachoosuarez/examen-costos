# Examen Costos (2240) — 20/12/2025

Este examen tiene solución oficial en el repositorio ("...Rev1 - solucion.docx.pdf"). Se resuelve mostrando el criterio y se **verifica contra la oficial** (coincide salvo una observación puntual anotada en la parte II).

---

## I – Metraje (20 pts) — muro de contención con bloque vibrado (20 m lineales)

Elementos del corte (Anexo I): hormigón de limpieza (ancho 1,55m), pie de muro/zapata (ancho 1,55m, espesor 0,15m), muro de bloques vibro-prensados 39x19x19 (altura ≈ 2,05m), viga de coronamiento 20x30cm. Armaduras: 2Φ10 en viga de coronamiento (long. total con 2 capas), 5Φ8 y 8Φ10 en la zapata, 2Φ6 en cada hilada del muro (armadura horizontal), pata tipo "L" Φ12/10 y pata con rulo Φ8/10 (armadura vertical dentro de los bloques).

| Ítem | Cálculo (ancho × espesor × long) | **Resultado** |
|---|---|---|
| a) Vol. H° limpieza | 1,55 × 0,05 × 20 | **1,55 m³** |
| c) Vol. H° pie del muro | 1,55 × 0,15 × 20 | **4,65 m³** |
| d) Vol. H° viga coronamiento | 0,30 × 0,20 × 20 | **1,20 m³** |

**b) Cantidad de bloques:** área de muro a cubrir = 20 m (largo) × 1,60 m (altura de bloques, sin viga ni zapata) = 32 m². Cantidad = 12,5 bloques/m² × 32 m² = **400 bloques**.

**e) Volumen de H° interior a los bloques:** volumen bruto de un bloque = 0,19×0,19×0,39 = 0,01407 m³; hueco a rellenar = 45% → 0,00634 m³/bloque. Vol. = 400 bloques × 0,00634 = **2,53 m³**.

**f) Tenor de encofrado (viga y pie del muro):**

| Elemento | Encofrado lateral (m/m lineal) | Long | Encofrado (m²) | Volumen (m³) | Tenor (m²/m³) |
|---|---|---|---|---|---|
| Viga | 0,60 | 20 | 12,0 | 1,20 | **10,00** |
| Zapata (pie) | 0,30 | 20 | 6,0 | 4,65 | **1,29** |
| **Total** | | | **18,0** | **5,85** | (usado en consumos) |

*(Los bloques no llevan encofrado: quedan a la vista/autoportantes; por eso el volumen de "interior a los bloques" no entra en este tenor.)*

**g) Kilogramos de acero por diámetro** (barra 12m, empalme 50Φ, gancho 10Φ donde no está especificado en el detalle):

| Elemento | Φ (mm) | Long. barra (m) | Cantidad | Empalme | Gancho | L total (m) | kg (sin desp.) | **kg con desperdicio** |
|---|---|---|---|---|---|---|---|---|
| Zapata (long.) | 10 | 20 | 8 | sí | sí | 21,2 | 104,6 | 115,0 |
| Zapata (long.) | 8 | 20 | 5 | sí | sí | 21,0 | 41,4 | 43,4 |
| Viga coronamiento | 10 | 20 | 4 (2Φ10+2Φ10) | sí | sí | 21,2 | 52,3 | 57,5 |
| Horizontales en muro (2Φ6/hilada) | 6 | 20 | 14 | sí | sí | 20,7 | 64,4 | 67,6 |
| Pata tipo "L" (vertical en bloques) | 12 | 3,3 | 200 (paso 10cm×20m) | no | no | 3,3 | 593,1 | 652,4 |
| Pata con rulo (vertical en bloques) | 8 | 4,3 | 200 (paso 10cm×20m) | no | no | 4,3 | 339,3 | 356,3 |

**Totales por diámetro (kg con desperdicio):**

| Φ (mm) | **kg** |
|---|---|
| 6 | **67,6** |
| 8 | **399,7** (43,4+356,3) |
| 10 | **172,5** (115,0+57,5) |
| 12 | **652,4** |
| **TOTAL** | **1.292,2 kg** |

---

## II – Consumos y Dosificación del Hormigón (15 pts)

**Tenor y cuantía del muro** (a partir de la parte I):
- Tenor de encofrado = 18 m² (viga+zapata) / 5,85 m³ (viga+zapata) = **3,08 m²/m³**
- Cuantía de acero = 1.292,2 kg / 8,38 m³ (viga+zapata+relleno de bloques = 1,20+4,65+2,53) = **154,13 kg/m³**

**Consumos unitarios por m³ de hormigón:**

| Insumo | Fórmula | **Resultado** |
|---|---|---|
| Of. Carpintero | 4,00×1 (pasta) + 2,00×3,08 (encofrado) | **10,2 hs/m³** |
| Of. Herrero | 0,04×154,13 (hierro) | **6,2 hs/m³** |
| Ayudante | 2,00×1 + 1,00×3,08 + 0,04×154,13 | **11,2 hs/m³** |
| Hormigón premezclado | 1×(1+5%) | **1,05 m³/m³** |
| Acero | cuantía | **154,1 kg/m³** ⚠️ ver nota |
| Tabla de pino | (3,08×1,15)/3 reúsos /0,495 m² (3,30×0,15 área unitaria) | **2,38 unid/m³** |

⚠️ **Nota de estudio:** la solución oficial en su tabla resumen final muestra "Acero: 1.292,23 kg" (el total del muro, copiado de la parte I‑g) en lugar de la cuantía por m³ (154,13 kg/m³) que la misma solución calculó unas líneas antes como "Tenor Armadura". Como el enunciado pide **consumos unitarios por m³**, el valor correcto y consistente con el resto de la tabla es **154,1 kg/m³** — probablemente un desliz de copiado en la planilla del docente. Al estudiar, usar siempre cuantía = kg totales / m³ totales, nunca el kg total suelto.

**Dosificación y costo del m³ de hormigón** (relación en volumen 3,5:2:1, a/c=0,50, dens. cemento 1.400 kg/m³):

| Componente | Vol. aparente | Coef. aporte | Vol. real (m³) | Unidad comercial | Costo unitario | **Costo** |
|---|---|---|---|---|---|---|
| Agregado grueso | 3,50 | 0,55 | 1,93 | 0,83 m³ | 1.250 $/m³ | 1.033 $ |
| Agregado fino | 2,00 | 0,57 | 1,14 | 0,47 m³ | 850 $/m³ | 401 $ |
| Cemento Portland | 1,00 | 0,47 | 0,47 | 330,58 kg → 13,22 bolsas | 220 $/bolsa 25kg | 2.909 $ |
| Agua (a/c=0,50) | 0,70 | 1,00 | 0,70 | 165,29 lt | — | — |
| **TOTAL materiales / m³ hormigón** | | | | | | **≈ 4.344 $/m³** |

---

## III – Fórmulas Paramétricas (15 pts)

**a) Objetivo:** reflejar las variaciones de costos en el precio de venta lo más aproximadamente posible, eliminando riesgos tanto para el Contratista como para el Contratante (ni el contratista pierde por inflación de insumos, ni el contratante paga de más).

**b) Listados de referencia más comunes:** 1) MTOP – Dirección Nacional de Vialidad; 2) MTOP – Dirección Nacional de Arquitectura; 3) Cámara de la Construcción del Uruguay.

**c) Cálculo — Viga de hormigón armado** (10m × 0,20 × 0,50 = 1,00 m³; armadura 80 kg/m³; encofrado 12 m²/m³; M.O. 30 hs/m³):

| Ítem | Cantidad | Precio unit. | Precio total | % incidencia |
|---|---|---|---|---|
| Hormigón | 1,00 m³ | 6.000 $/m³ | 6.000 | 19,42% → **20%** |
| Acero | 80 kg | 60 $/kg | 4.800 | 15,53% → **16%** |
| Madera (encofrado) | 12 m² | 300 $/m² | 3.600 | 11,65% → **11%** |
| Mano de obra | 30 hs | 550 $/hora | 16.500 | 53,40% → **53%** |
| **TOTAL** | | | **30.900 $** | 100% |

**Fórmula paramétrica:**

Precio_n = Precio_0 × (0,53×MO_n/MO_0 + 0,20×Cemento_n/Cemento_0 + 0,16×Acero_n/Acero_0 + 0,11×Madera_n/Madera_0)

*(el ítem de hormigón se referencia con el índice de Cemento; también es válido usar una combinación cemento+áridos — ambas opciones se consideran correctas según la solución oficial).*

---

## IV – Costo de la mano de obra de la construcción (15 pts)

**a) Dos formas de retribuir a los obreros:**
- **Por tiempo trabajado**: valor por unidad de tiempo (mes → "mensuales"; jornal/día → "jornaleros", 44 hs/semana: lunes a jueves 9 hs, viernes 8 hs). Encargados y capataces se contratan mensuales, el resto jornaleros.
- **Por producción ("destajo")**: valor por unidad de producción (ej. m² de muro o revoque). Requiere control exhaustivo de lo ejecutado; poco usado en presupuestaciones convencionales.

**b) Ítems que se pagan al obrero jornalero:** hora común; ropa/transporte/herramientas; incentivo por presentismo semanal (10,42%) y mensual (5%); media hora de descanso; incentivos por producción; horas extra (+100%); feriados (7 no laborables al año); horas de lluvia/barro/crecidas; tickets de alimentación ($200 c/8hs); vestimenta (ropa de invierno/verano + campera bianual); suplemento por trabajo en altura (10% jornal Cat. V c/8hs, >6m); suplemento por acarreo a plataformas voladas (30%); horas nocturnas (+30%/+50%).

**c) Costo horario — Medio Oficial Carpintero (Cat. VI), obra = reforma de baño en casa de familia, sin horas extra:**

| Concepto | Base | % / valor | **$/hora** |
|---|---|---|---|
| Hora común (Cat. VI) | — | — | 279,92 |
| Ropa (5% Cat. V) | 258,65 | 5,00% | 12,93 |
| Transporte (4,374% Cat. V) | 258,65 | 4,37% | 11,31 |
| Herramientas (2% Cat. V) | 258,65 | 2,00% | 5,17 |
| Presentismo semanal | 279,92 | 10,42% | 29,17 |
| Presentismo mensual | 279,92 | 5,00% | 14,00 |
| Media hora de descanso | 279,92 | 0,5 | 17,50 |
| Feriados (7/año) | 279,92 | 7/8 | 7,92 |
| Tickets alimentación ($200/8hs) | — | — | 25,00 |
| Incentivo por producción, horas extra, lluvia/barro/crecidas, altura, plataformas voladas, horas nocturnas | — | no aplica (baño interior, sin extras) | 0 |
| **TOTAL costo horario** | | | **≈ 402,9 $/hora** |

**d) Ítems que integran el Monto Imponible:** de acuerdo al ejercicio → **hora común, presentismo semanal, presentismo mensual y feriados**. Reglamentariamente se suman además: horas nocturnas, trabajo en altura y horas extra (ambas respuestas se toman como válidas). No integran el MI: ropa, transporte, herramientas, media hora de descanso, tickets de alimentación, horas de lluvia/barro/crecidas.

---

## V – Garantías (15 pts)

Edificio de viviendas en Maldonado. Costo total (neto, sin IVA/beneficio) $280.000.000; beneficio 15% sobre precio de venta; IVA 22%; plazo 15 meses; mano de obra imponible = 30% del costo total; garantía sobre certificado del BSE al 2% anual del monto a garantizar.

**Precio de venta con IVA y LLSS incluidos:**
- Precio de venta = Costo/(1-0,15) = 280.000.000/0,85 = 329.411.764,71 $ (antes de IVA/LLSS)
- LLSS de mano de obra: MI ≈ 30% del costo total = 84.000.000; LLSS ≈ 75,8% del MI (obra de arquitectura) ≈ 63.672.000 — la solución oficial llega a **Precio + IVA + LLSS = $ 465.554.352,94**

| Garantía | Monto a garantizar | Período | **Costo (2%/año)** |
|---|---|---|---|
| Fiel Cumplimiento (10% del precio c/IVA y LLSS, constante desde firma hasta Recepción Provisoria=fin de obra=15 meses) | $46.555.435,29 | 15 meses | **$1.163.885,88** |
| Buena Ejecución (5% de cada certificado; crece linealmente de 0 a 15 meses, luego se mantiene 18 meses hasta Recepción Definitiva) | monto medio 1º tramo $14.548.573,53 (15 meses) + monto medio 2º tramo $34.916.576,47 (18 meses) | 15+18 meses | $290.971,47 + $698.331,53 = **$989.303,00** |
| Anticipo (15% del precio sin IVA/LLSS, se devuelve linealmente en 15 meses → monto medio = 50%) | monto medio $24.705.882,35 | 15 meses | **$617.647,06** |
| **COSTO TOTAL DE GARANTÍAS** | | | **$2.770.835,94** |

**¿Es razonable?** El costo total de garantías representa **0,99% del costo de la obra** ($2.770.835,94 / $280.000.000) — del orden de 1%, lo cual es coherente con los valores de referencia de la Clase de Garantías (costos de pólizas entre 0,4% y 3% del monto garantizado, sumando históricamente ~0,5%-1% del precio de la obra). Es razonable.

---

## VI – Suministros (10 pts)

**a) Para que los suministros (materiales) estén correctamente...**
- **Identificados**: especificaciones técnicas claras y suficientes (normas/memorias técnicas); si no se cumple algún requisito, dejarlo explícito y valorar su consecuencia; identificar proveedores potenciales; ensayos a exigir al proveedor; lugar de entrega (con o sin flete/carga/descarga); necesidad o no de contrato.
- **Cuantificados**: definir con claridad la unidad de medida (ej. cemento por kg o por bolsa; arena por m³ o en bolsas; carpeta por m² o por m³); criterios de desperdicio a considerar; cantidad total requerida y plazo de entrega estimado.
- **Valorados**: obtener precio unitario acorde a la unidad definida, vigente y con cotización de al menos un proveedor confiable, considerando condiciones de pago y entrega.

**b) INCOTERMS:** términos comerciales internacionales utilizados en contratos de compraventa internacional que establecen con precisión las obligaciones, derechos y responsabilidades del exportador (vendedor) y del importador (comprador) respecto a la entrega de la mercadería (quién paga flete, seguro, en qué punto se transfiere el riesgo, etc.). Tipos habituales: EXW, FOB, CIF, CFR, FCA, DAP, DDP, entre otros.
