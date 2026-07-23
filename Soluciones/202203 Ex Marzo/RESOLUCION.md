# Examen Costos — "Marzo 2022" (real 15/02/2022)

Verificado contra solución oficial (planilla de cálculo incluida en `Examen Costos Marzo 2022- Preg A,B,CyD.pdf` — cubre A, B, C y D). La Parte E (teórica) no viene con solución oficial en el repo — se responde con el criterio de la Guía.

**Ojo:** este examen usa un plano de estructura "real" (numeración de vigas/pilares de un edificio), más complejo que el Anexo esquemático habitual. La geometría exacta de la viga V2545 (sección variable "semi invertida") no se pudo re-derivar 100% desde la imagen del plano — se presentan los resultados verificados exactamente contra la planilla oficial, con la lógica general explicada.

---

## A-1 – Metraje Hormigón: Losa (dos paños L1+L2) (parte de 25 pts)

**Vano libre de cada paño** (idénticos): horizontal=6,81m, vertical=6,62m, espesor=0,16m.
- V (cada paño) = 6,81×6,62×0,16 = **7,21 m³** → **Total Losa (L1+L2) = 14,426 m³**
- Encof (cada paño, losa suspendida → solo cara inferior) = 6,81×6,62 = 45,08 m² → **Total = 90,164 m²**
- Armadura: familia "A" de fondo (positiva) con barra vertical Φ8/0,18 y horizontal Φ10/0,20, más familia "F" horizontal Φ12/0,18 — cada paño con 374,31 kg → **Total acero = 748,62 kg**

**Resultados A-1:**
- **Tenor de encofrado = 90,164/14,426 = 6,25 m²/m³**
- **Cuantía de acero = 748,62/14,426 = 51,89 kg/m³**

---

## A-2 – Metraje Hormigón: Viga N°2545 (parte de 25 pts)

**Sección:** "(17×144) semi invertida" según el plano de planta (el detalle en hoja aparte la rotula como 17×114, probable inconsistencia entre plano y detalle en el propio examen — se usa 17×144, que es el valor consistente con el volumen de la planilla oficial). Largo=5,24m (entre los pilares P43 y P47, columna derecha de la estructura).

- V (cuerpo principal V2545) = 0,17×1,44×5,24 = **1,28 m³**
- V\* (ajuste por sección variable, franja adicional 0,12×0,06×7,04m, asociada a la definición de un pretil sobre los pilares 43 y 47 — la nota oficial aclara que si NO se considera ese pretil, V\*=0,038 en vez de 0,051) = **0,05 m³**
- **Total Viga = 1,28+0,05 = 1,333 m³**
- **Total Encofrado = 16,096 m²**

**Armadura** (según "DETALLE VIGA 2545": 1Φ6 corrido superior, 6Φ6 corridos secundarios, estribos Φ6/25, 2Φ19 corrido inferior — armadura principal a flexión de una viga invertida, con la barra traccionada abajo):

| Barra | Ø (mm) | kg (c/desp) |
|---|---|---|
| 1Φ6 corrido (sup.) | 6 | 4,88 |
| 6Φ6 corridos (secundarios) | 6 | 9,76 |
| 2Φ19 corrido (inf., principal) | 19 (≈20 tabla) | 43,40 |
| Estribos Φ6/25 | 6 | 17,58 |
| **TOTAL** | | **75,62 kg** |

**Resultados A-2:**
- **Tenor de encofrado = 16,096/1,333 = 12,07 m²/m³**
- **Cuantía de acero = 75,62/1,333 = 56,71 kg/m³**

---

## B – Costo Componentes del Hormigón (15 pts)

**Enunciado:** costo de los componentes de 1 m³ de hormigón, dosificación 4:2:1 (Pedregullo:Arena Gruesa:Cemento), a/c=0,50, densidad aparente cemento=1.400 kg/m³.

**Paso 1 — volumen real de cada componente** (rel.aparente × Coef. de Aporte): Pedregullo=4×0,55=2,20; Arena Gruesa=2×0,57=1,14; Cemento=1×0,47=0,47.

**Paso 2 — volumen de agua** (a partir del cemento "sin escalar" tal como está en la relación 4:2:1): Cemento aparente=1 m³ → kg=1×1.400=1.400 kg → Agua=0,50×1.400=700 lt=**0,700 m³** (Ca del agua=1, aparente=real).

**Paso 3 — sumar TODOS los volúmenes reales (agregados+cemento+agua) → este es el volumen de hormigón que rendiría la receta tal cual está escrita:**
Suma = 2,20+1,14+0,47+0,70 = **4,51 m³** (no da 1 m³ exacto, hay que escalar toda la receta).

**Paso 4 — escalar cada componente dividiendo por 4,51 (para que el total dé exactamente 1 m³):**

| Componente | Vol. aparente original | Escalado (÷4,51) | Unidad comercial | Costo unit. | Costo total |
|---|---|---|---|---|---|
| Pedregullo | 4 m³ | 0,887 m³ | 0,887 m³ | $1.460/m³ | **$1.295,02** |
| Arena Gruesa | 2 m³ | 0,443 m³ | 0,443 m³ | $1.110/m³ | **$491,73** |
| Cemento | 1 m³ | 0,222 m³ | 0,222×1.400=**310 kg** | $8,40/kg (=210$/bolsa 25kg) | **$2.604,00** |
| Agua | — | — | 310×0,50=**155 lt** | — | $0 |
| **TOTAL** | | | | | **$4.390,75/m³** |

---

## C – Costos Fijos, Variables (15 pts)

**Enunciado:** el comitente pide **reducir** el plazo en 3 meses (20→17), manteniendo certificación uniforme; el contratista tiene holgura para no aumentar el costo variable, y el costo fijo (proporcional al plazo, con costo fijo mensual constante) se reduce proporcionalmente. **Es el caso inverso al de Dic-2022** (allá se extendía el plazo, acá se reduce).

**Datos (base 100=costo total original):** Costo fijo=20% (20,00), Costo variable=80% (80,00, sin cambios porque no aumentan las cantidades ni los rendimientos empeoran), Beneficio original=15% **sobre el costo** → Venta=100×1,15=**115,00**.

**Costo fijo nuevo** (proporcional a la reducción de meses, 17/20): 20,00×(17/20) = **17,00**
**Costo total nuevo** = 17,00+80,00 = **97,00**

**Como no hay revisión de presupuesto, la venta se mantiene en 115,00:**
- Beneficio nuevo = 115,00−97,00 = **18,00** → variación = (18−15)/15 = **+20,0%** (el beneficio AUMENTA, al revés que en Dic-2022, porque acá el costo fijo BAJA en vez de subir)
- Benef/costo nuevo = 18,00/97,00 = 18,6% → variación = (18,6−15)/15 = **+23,7%**
- Beneficio/venta nuevo = 18,00/115,00 = **15,65%** (contra 13,04% original)

**Conclusión: al reducirse el plazo sin revisión de presupuesto ni aumento de costo variable, el contratista sale beneficiado — su margen aumenta un 20% en valor absoluto** (mecanismo idéntico al de Dic-2022 pero con signo opuesto: el costo fijo total es proporcional al plazo, así que cualquier cambio de plazo sin cambio de alcance mueve el beneficio en la dirección contraria al cambio de plazo).

---

## D – Proyecto de Inversión (20 pts)

**Enunciado:** comparar depósito a plazo fijo (U$S2.000.000, 6 años, interés bancario ib=5% anual, sin capitalizar) contra una inversión edilicia con flujo dado, aplicando una tasa de riesgo adicional tr=7% (tasa total ib+tr=12% para la inversión riesgosa).

**a) VNA de cada alternativa:**
- **Depósito** (flujo: −2.000 en año0, +100 los años 1-5, +2.100 en año6, descontado a **ib=5%**): **VNA = 0,00** (por definición: el VNA de un depósito descontado a su propia tasa de interés siempre da 0).
- **Inversión edilicia** (flujo: −700,−700,−600,210,840,840,840, descontado a **ib+tr=12%**): **VNA = −217,80** (miles de U$S).

**b) Elección:** VNA(depósito, 0,00) > VNA(inversión edilicia, −217,80) → **es más conveniente el depósito a plazo fijo.**

**c) TIR del depósito (a):** **TIR(a) = 5%**, por definición — un depósito descontado a su propia tasa bancaria siempre da VNA=0, así que esa tasa ES la TIR.

**d) Rango de la TIR de la inversión edilicia (b):** se calcula el VNA(b) a una segunda tasa de referencia, **5%** (la tasa "sin riesgo"): **VNA(b);5% = +246,57** (miles). Como VNA(b) pasa de **positivo (+246,57 a 5%) a negativo (−217,80 a 12%)**, la TIR(b) está **estrictamente entre 5% y 12%** → cae en el rango **ii) 5% < TIR(b) ≤ 12%**.

**Aproximación de la TIR(b) por interpolación lineal** entre los dos puntos conocidos (tasa, VNA)=(5%, 246,57) y (12%, −217,80):
`TIR(b) ≈ 5% + [246,57/(246,57−(−217,80))]×(12%−5%) = 5% + 0,531×7% = 8,72%`

**⚠️ La interpolación lineal es solo una aproximación**, no el valor exacto — el VNA no es una función lineal de la tasa de descuento (es una suma de términos 1/(1+i)ᵗ, convexa). La TIR real (calculada con la función financiera exacta) da **8,34%**, cerca pero no igual al 8,72% aproximado por interpolación. Para un examen sin calculadora financiera, la interpolación lineal entre dos VNA de signo opuesto es el método esperado y da un resultado suficientemente cercano — pero hay que aclarar que es una aproximación si el enunciado no pide el valor exacto.

---

## E – Régimen Salarial (15 pts) *(teórico, sin solución oficial en el repo)*

Ver Guía sección 6 (mismo desarrollo que en exámenes anteriores, ej. `Soluciones/202302 Ex Febrero/`):

**a) Sistema de remuneración (Ley 14.411):** remuneración por jornal/hora según categoría y laudo del Convenio Colectivo (Grupo 37); aportes patronales/obreros centralizados en un Aporte Unificado de la Construcción, % sobre el Monto Imponible, en vez de liquidarse tarea por tarea.

**b) Convenio Colectivo (Grupo 37):** tripartito — Cámaras empresariales, SUNCA, MTSS/Poder Ejecutivo (homologa). Trata categorías/laudos salariales, ajuste salarial, licencia/aguinaldo, condiciones de trabajo/seguridad, Fondos Sociales de la Construcción.

---

## Resumen ejecutivo del examen

| Parte | Resultado clave |
|---|---|
| A-1 – Metraje Losa | Vol=14,426 m³; Tenor=6,25 m²/m³; Cuantía=51,89 kg/m³ |
| A-2 – Metraje Viga | Vol=1,333 m³; Tenor=12,07 m²/m³; Cuantía=56,71 kg/m³ |
| B – Costo Componentes Hormigón | $4.390,75/m³ (Pedregullo+Arena+Cemento; agua sin costo) |
| C – Costos Fijos/Variables | Reducción de plazo (20→17 meses) sin revisión de presupuesto: **beneficio sube +20,0%** (costo fijo baja proporcionalmente al plazo) |
| D – Proyecto de Inversión | Conviene el **depósito bancario** (VNA=0 > VNA edilicia=−217,80); TIR(a)=5% exacta; TIR(b) entre 5-12% (aprox. 8,72% por interpolación, real 8,34%) |
| E – Régimen Salarial | Aporte Unificado Ley 14.411; Convenio Colectivo tripartito |
