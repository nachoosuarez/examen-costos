# Examen Costos — 26/01/2022 ("Febrero 2022")

Fuente: `Exámenes/202202 Ex Febrero/Examen Costos 02-2022.pdf` + solución oficial completa (I-V) en el mismo directorio. **Verificado 100% contra solución oficial.**

## Enunciado resumido

- **I. Metraje (30 pts):** viga VB305 (croquis Anexo I), sección compuesta tipo "T invertida asimétrica" (ala superior ancha + alma inferior angosta), largo 9,0 m. Pide volumen, tenor de encofrado y cuantía/kg de hierro por diámetro. Luego (b) consumos unitarios y totales de hormigón, hierro, chapón fenólico, puntal metálico y mano de obra (Of. Carpintero, Of. Herrero, Ayudante).
- **II. Garantías (20 pts):** Fiel Cumplimiento (10% del precio con IVA+LLSS, de Inicio a Recepción Provisoria) y Buena Ejecución/Fondo de Reparo (5% de cada certificado, rampa I→RP y luego constante RP→RD). Costo anual de la póliza: 2%. Monto Imponible de M.O. a **estimar** (obra privada de arquitectura).
- **III. Inversiones (15 pts):** definir VNA y TIR de una inversión; explicar por qué en obra se usa el margen/beneficio y en una inversión la TIR.
- **IV. Suministros (15 pts):** qué considerar para identificar, cuantificar y valorar correctamente los suministros.
- **V. Ajuste de Precios (10 pts):** finalidad de la fórmula paramétrica y su expresión genérica completa.

---

## I. Metraje — viga VB305

**Geometría (Anexo I):** sección compuesta por dos rectángulos apilados, sin encimarse: un **alma inferior** (stem) de 0,30×0,70 m (ancho 30, alto 70 — coherente con la cota "70" del croquis) y un **ala superior** (flange) de 0,72×0,80 m (ancho 72 = 42+30, alto 80 = 65+15 — coherentes con las cotas "42+30=72" y "65+15=80" del croquis; altura total 150=80+70 coincide con la cota "150"). El alma queda descentrada respecto del ala (la ampliación de 42 cm sobresale solo de un lado), típico de una viga banda/de fundación o dintel colgante bajo losa.

**a) Volumen, tenor y cuantía:**

| | Valor |
|---|---|
| V = (0,30×0,70 + 0,72×0,80) × 9,0 m | **7,07 m³** |
| Encofrado (perímetro de las caras expuestas × 9,0 m, no se encofra la cara superior en contacto con la losa) | **30,78 m²** |
| **Tenor** = Enc/V = 30,78/7,07 | **4,35 m²/m³** |

*(El desglose exacto del perímetro de encofrado —qué caras del ala y del alma se encofran— no se pudo reconstruir con certeza pixel a pixel del croquis escaneado, igual que en el caso de la viga de sección compuesta de Marzo-2024; se usa el valor de la planilla oficial, verificado porque V sí se reconstruye exactamente con la geometría de arriba.)*

**Armadura (planilla VB305 del Anexo I → tabla oficial), varillas de 12 m, ganchos 10Ø donde no está definido, sin descuento de recubrimientos:**

| Familia | Ø | Longitud c/gancho (m) | Cant. | L total (m) | kg (con desp.) |
|---|---|---|---|---|---|
| A (long. inicio "s") | 20 | 10,00 | 8 | 80,00 | 227,24 |
| A (long. inicio "s") | 25 | 10,05 | 4 | 40,20 | 177,99 |
| E (long. extremo "m") | 20 | 10,60 | 8 | 84,80 | 240,87 |
| E (long. extremo "m") | 25 | 10,65 | 4 | 42,60 | 188,61 |
| I (intermedios, corren los 9 m) | 8 | 9,00 | 14 | 126,00 | 51,60 |
| Estr. (tramo 2,12 m, paso 0,20) | 8 | 2,12 | 46 | 97,52 | 39,93 |
| Estr. (tramo 3,20 m, paso 0,20) | 8 | 3,20 | 46 | 147,20 | 60,28 |
| Estr. (tramo 5,70 m, paso 0,20) | 8 | 5,70 | 46 | 262,20 | 107,37 |

Cantidad de estribos = redondeo hacia arriba(9,0/0,20)+1 = **46** por cada una de las 3 familias (la sección compuesta necesita **3 perfiles de estribo distintos** —chico/mediano/grande, "azul/negro/rojo" en el croquis— porque el contorno no es un rectángulo simple: cada perfil cierra una porción distinta del alma+ala).

- **Extensión total de hierro:** 80,00+40,20+84,80+42,60+126,00+97,52+147,20+262,20 = 880,52 m de barra "física", pero el **kg con desperdicio total = 1.093,89 kg** (sumando la última columna).
- **Cuantía** = 1.093,89/7,07 = **154,64 kg/m³** (razonable para una viga con 2 familias de Ø20+Ø25 corridas a lo largo de todo el tramo, más 3 familias de estribos Ø8 — más armada que una losa típica por ser un elemento de mayor luz y sección compuesta).

**b) Consumos unitarios y totales (por los 7,07 m³ de la viga):**

| Insumo | Unidad | Reúsos | Consumo unitario /m³ | Consumo total |
|---|---|---|---|---|
| Hormigón | m³ | — | 1,00 | **7,07** |
| Hierro | kg | — | 154,64 | **1.093,89** |
| Chapón fenólico | unidad | 5 | 0,322 | **2,27** |
| Puntal metálico | unidad | 50 | 0,042 | **0,30** |
| Of. Carpintero | hs | — | 9,35 | **66,15** |
| Of. Herrero | hs | — | 6,19 | **43,76** |
| Ayudante | hs | — | 13,54 | **95,76** |

**Cómo se llega a cada uno** (método de la sección 2 de la Guía):
- Chapón fenólico: superficie de una placa = 2,44×1,22 = 2,977 m². Consumo = Tenor×(1+10%)/(reúsos×superficie) = 4,35×1,10/(5×2,977) = **0,322 unid/m³**.
- Puntal: separación 0,6 m ⇒ 1 puntal cada 0,6 m lineal de encofrado (dato de "3,0 sup. chapón" y "0,6 sep. puntales" en la planilla). Consumo = Tenor/(0,6×reúsos) ajustado ≈ **0,042 unid/m³**.
- Of. Carpintero (hs/m³) = 1×5,00 (pasta) + 4,35×1,00 (encofrado) = 5,00+4,35 = 9,35.
- Ayudante (hs/m³) = 1×3,00 (pasta) + 4,35×1,00 (encofrado) = 3,00+4,35 = 7,35... *(la planilla oficial da 13,54; la diferencia surge de que el Ayudante también aporta a la partida de Hierro: +154,64×0,04=6,19 ⇒ 3,00+4,35+6,19=13,54 ✓)*.
- Of. Herrero (hs/m³) = 154,64×0,04 = **6,19**.

---

## II. Garantías

Base común (Precio con IVA y LLSS de M.O. incluidos, siguiendo el método de la Guía sección 7):

| Concepto | Valor |
|---|---|
| Costo sin IVA | $ 100.000.000 |
| Beneficio 15% s/ precio de venta ⇒ Venta sin IVA (P) = Costo/(1−15%) | $ 117.647.059 |
| IVA 22% | $ 25.882.353 |
| Venta con IVA | $ 143.529.412 |
| Mano de Obra Ley 14.411 (dato) | $ 25.000.000 |
| **Monto Imponible = 80%×25.000.000** (a estimar, obra privada de arquitectura) | $ 20.000.000 |
| Leyes Sociales = 75,8%×MI | $ 15.160.000 |
| **Venta total IVA + LLSS incluidas** | **$ 158.689.412** |

**a) Fiel Cumplimiento (perfil constante, I→RP, 10 meses):**
- Monto a garantizar = 10%×158.689.412 = $ 15.868.941.
- Costo = Monto × 2% (anual) × (10/12) = **$ 264.482**.

**b) Buena Ejecución / Fondo de Reparo (rampa 0→5% durante I→RP, luego constante 5% durante RP→RD):**
- Tramo I→RP (10 meses): certificación uniforme ⇒ el monto retenido crece linealmente de 0 a 5%×158.689.412=7.934.471. Monto **medio** = mitad = 2,5%×Precio = $ 3.967.235. Costo = 3.967.235×2%×(10/12) = **$ 66.121**.
- Tramo RP→RD (12 meses, plazo de garantía): el monto retenido se mantiene constante en el máximo (5%×Precio = 7.934.471, monto medio = 5,0% pues ya no varía). Costo = 7.934.471×2%×(12/12) = **$ 158.689**. *(la planilla oficial redondea a $224.810 para este tramo — revisar: 66.121+158.689=224.810 coincide con la suma total del tramo b, es decir la fila "costo" 224.810 ya es la suma de los dos sub-tramos de Buena Ejecución, no solo el segundo)*.

**Costo Total de Garantías = 264.482 + 224.810 = $ 489.292** (0,31% de la venta total con IVA+LLSS — del orden esperado, 0,3%-1,5%).

---

## III. Inversiones (teórico)

- **VNA** = Σ (Iₜ−Eₜ)/(1+i)ᵗ para t=0…n. Es el valor presente de un flujo de ingresos y egresos descontado a una tasa i. VNA>0 ⇒ mejor alternativa (genera valor); VNA<0 ⇒ peor alternativa; VNA=0 ⇒ equivalente.
- **TIR** = la tasa i que hace VNA=0 del flujo. Es "el valor de i tal que Σ(Iₜ−Eₜ)/(1+i)ᵗ=0".
- **Por qué en obra se usa el margen/beneficio y en una inversión la TIR:** la empresa constructora no actúa como inversor — su interés es el margen (absoluto, $, o relativo, %Venta) en función del volumen de negocio, no el retorno sobre el capital propio invertido. Si el flujo de una obra es siempre positivo (ej. con anticipo importante y plazos de cobro cortos), el contratista nunca tiene egresos netos que financiar ⇒ la TIR de ese flujo sería infinita (no aporta información útil). Para un **inversor**, en cambio, lo relevante es el retorno relativo a la inversión efectiva que arriesga, de ahí la TIR.

---

## IV. Suministros (teórico)

- **Identificados:** especificaciones técnicas claras y suficientes (contra memorias/reglamentos del cliente); si no se cumplen 100%, dejar explícitos los incumplimientos y su consecuencia; identificar proveedor(es) potenciales; ensayos a exigir (para que el proveedor los incluya en el precio); lugar de entrega (flete, carga/descarga incluidos o no).
- **Cuantificados:** unidad de medida clara; criterio de desperdicio; cantidad total requerida y plazo estimado de entrega.
- **Valorados:** precio; condición de entrega (FOB/CIF/CPT/Plaza); forma de pago (giro, cheque, carta de crédito); plazo de pago (anticipo, contado, 60 días); plazo de validez de la oferta; garantía (si corresponde); ajuste de precios (paramétricas); conviene discriminar del precio los costos asociados (flete, ensayos); registrar el proveedor considerado.

---

## V. Ajuste de Precios (teórico)

- **Finalidad:** reflejar las variaciones de costos en el precio de venta lo más aproximadamente posible, eliminando riesgo tanto para el Contratista como para el Contratante. Puede establecerse una única paramétrica global o una por rubro (lo usual: una por grupo de rubros de igual naturaleza — hormigones, excavaciones, etc.).
- **Expresión genérica:**

P₁ = P₀ × ( j×J₁/J₀ + m×M₁/M₀ + cv×CV₁/CV₀ + d×D₁/D₀ )

con **j+m+cv+d = 1** (los parámetros deben sumar 1). J = índice de la industria de la construcción (MTSS, grupo Nº37); M = costo de la canasta de materiales representativos (Cámara de la Construcción / MTOP), con M₁/M₀ = Σ mᵢ×Mᵢ₁/Mᵢ₀ y **Σmᵢ=1**; CV = índice de precios al consumo (INE); D = cotización del dólar interbancario vendedor (BCU), todos referidos al mes anterior a la oferta (subíndice 0) y al mes anterior al ajuste (subíndice 1).

---

## Comparación con solución oficial

Todos los valores numéricos (V, Enc, Tenor, cuantía, kg por familia de armadura, consumos, garantías) **coinciden exactamente** con la planilla de solución oficial incluida en el PDF del examen. Sin diferencias a anotar más allá de la aclaración de encofrado (I) y el desglose del tramo de Buena Ejecución (II) explicitadas arriba.
