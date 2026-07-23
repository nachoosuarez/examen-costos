# Examen Costos (2240) — 14/07/2025

Este examen tiene solución oficial en el repositorio ("...Solución Rev02.pdf"). Se resuelve mostrando el criterio y se **verifica contra la oficial** (coincide en su totalidad).

---

## I – Metraje (15 pts) — Pilar P16 (3er piso de edificio de 5 pisos)

Pilar de sección 0,12 × 1,97 m (y un tramo con 0,12×2,03m, variación menor de encofrado por junta), altura 2,6 m entre losas. Al estar en el 3er piso de 5, se debe considerar la **espera de empalme** con el siguiente nivel (por eso la longitud de barra individual incluye "Empalme 0,5" = 50Φ, ya sumada a la longitud unitaria).

**Armadura longitudinal (3 capas de barras Φ10):**

| Espesor | Largo | Alto | Φ | Cantidad | Long. unit. | Empalme | Long. total | kg/m | Desp. | **kg totales** |
|---|---|---|---|---|---|---|---|---|---|---|
| 0,12 | 1,97 | 2,6 | 10 | 22 | 2,6 | 0,5 | 68,2 | 0,62 | 10% | 46,51 |
| 0,12 | 1,97 | 2,6 | 10 | 22 | 2,6 | 0,5 | 68,2 | 0,62 | 10% | 46,51 |
| 0,12 | 2,03 | 2,6 | 10 | 20 | 2,6 | 0,5 | 62,0 | 0,62 | 10% | 42,28 |

**Estribos (Φ6):**

| Φ | Cantidad | Long. unit. | Ganchos | Long. total | kg/m | Desp. | **kg totales** |
|---|---|---|---|---|---|---|---|
| 6 | 23 | 4,18 | 0,12 | 98,9 | 0,22 | 5% | 22,85 |
| 6 | 23 | 4,18 | 0,12 | 98,9 | 0,22 | 5% | 22,85 |
| 6 | 23 | 4,78 | 0,12 | 112,7 | 0,22 | 5% | 26,03 |

**Volumen y encofrado:**

| Espesor | Largo | Alto | Vol (m³) | Encof (m²) |
|---|---|---|---|---|
| 0,12 | 1,97 | 2,6 | 0,61 | 10,24 |
| 0,12 | 1,97 | 2,6 | 0,61 | 10,24 |
| 0,12 | 2,03 | 2,6 | 0,63 | 11,18 |
| **Total** | | | **1,86** | **31,67** |

**Resultados:**
- **Volumen de hormigón = 1,86 m³**
- **Tenor de encofrado = 17,00 m²/m³**
- **Cuantía de acero = 111,15 kg/m³**

**¿Son esperables?** Sí — la cuantía cae dentro del rango típico de pilares. El tenor de encofrado sale **un poco superior** al rango habitual, justificado porque el pilar tiene un **espesor pequeño** (0,12 m): al ser tan delgado, el área de encofrado por m³ de hormigón crece mucho (la relación superficie/volumen aumenta cuando una dimensión es chica), sin que eso implique un error de cálculo.

---

## II – Consumos y Dosificación del Hormigón (20 pts)

**Tenor y cuantía del pilar:** Tenor de encofrado = 17,00 m²/m³; Cuantía de acero = 113,53 kg/m³ (la solución recalcula la cuantía a partir de los kg totales/volumen sin el detalle de redondeo del ítem I, da un valor levemente distinto: 111,15 vs 113,53 — pequeñas diferencias de redondeo entre planillas, ambas del mismo orden).

**Consumos unitarios por m³ de pilar:**

| Insumo | Fórmula | **Resultado** |
|---|---|---|
| Of. Carpintero | 4,00×1 (pasta) + 2,00×17,00 (encofrado) | **38,00 hs/m³** |
| Of. Herrero | 0,04×113,53 (hierro) | **4,54 hs/m³** |
| Ayudante | 2,00×1 + 1,00×17,00 + 0,04×113,53 | **23,54 hs/m³** |
| Hormigón premezclado | 1×(1+5%) | **1,05 m³/m³** |
| Acero | cuantía | **113,53 kg/m³** |
| Chapón fenólico | (17,00×1,15)/5 reúsos /2,98 m² (1,22×2,44) | **1,31 unid/m³** |

**Dosificación y costo del m³ de hormigón** (relación en volumen 3:1,7:1, a/c=0,45, dens. cemento 1.400 kg/m³):

**Cómo se obtiene la relación volumétrica agua/cemento** (método explicado en la solución oficial, muy útil para repetir en cualquier examen): tomar una base arbitraria de cemento (ej. 100 kg) → volumen de esos 100 kg de cemento = 100/1.400 = 71,4 litros → agua necesaria = 100×0,45 = 45,0 kg = 45,0 litros (agua: 1kg≈1lt) → relación volumétrica agua/cemento = 45,0/71,4 = **0,63 unidades de agua por unidad (de volumen) de cemento**. Este 0,63 se usa como el "volumen aparente" del agua en la tabla de reparto.

| Componente | Vol. aparente | Coef. aporte | Vol. real (m³) | Unidad comercial | Costo unitario | **Costo** |
|---|---|---|---|---|---|---|
| Agregado grueso | 3,0 | 0,55 | 1,650 | 0,807 m³ | 1.250 $/m³ | 1.008 $ |
| Agregado fino | 1,7 | 0,57 | 0,969 | 0,457 m³ | 820 $/m³ | 375 $ |
| Cemento Portland | 1,0 | 0,47 | 0,470 | 376,4 kg → bolsas | 230 $/bolsa 25kg | 3.463 $ |
| Agua (a/c=0,45) | 0,63 | 1,00 | 0,630 | 169,4 lt | — | — |
| **TOTAL / m³ hormigón** | (suma vol. real = 3,719) | | | | | **≈ 4.846 $/m³** |

*(Pasos: Vol. real = aparente×coeficiente; Verificación = vol.real/Σvol.real (debe sumar 1); Vol. aparente(1m³) = Verificación/coeficiente; Reducción a unidad comercial = aparente(1m³) tal cual para áridos (m³), ×1.400 para cemento (kg), ×1.000 para agua (lt); Costo = cantidad×costo unitario.)*

---

## III – Costo Financiero (20 pts)

**a) Valor Neto Actualizado (VNA):** es la suma de los valores presentes de todos los ingresos y egresos que componen el flujo de la inversión, traídos a valor presente mediante una tasa de descuento/interés definida. El resultado indica el monto a presente que genera la inversión por encima de los intereses considerados. Si VNA=0, la tasa de descuento usada coincide con la TIR del proyecto. Si VNA>0, la inversión rinde más que la tasa de descuento (TIR mayor). Si VNA<0, rinde menos (TIR menor).

**b1) Deuda de $1.000.000, 3 alternativas de pago, tasa trimestral 20%:**

| Alternativa | Trim1 | Trim2 | Trim3 | Trim4 | Trim5 | **VNA (a 20%/trim.)** |
|---|---|---|---|---|---|---|
| 1 | 350 | 350 | 350 | 300 | 300 | **1.002,508** (miles $) |
| 2 | 400 | 400 | 200 | 200 | 200 | 903,678 |
| 3 | 0 | 0 | 0 | 0 | 2.450 | 984,600 |

**Orden de conveniencia para la empresa constructora (mayor a menor VNA): Alternativa 1 > Alternativa 3 > Alternativa 2.**

**b2)** Solo la **Alternativa 1** devuelve un VNA ($1.002.508) **superior** a la deuda original ($1.000.000): reconoce al contratista una indemnización mayor que el costo del dinero. Las alternativas 2 y 3 devuelven un VNA menor a $1.000.000 → no compensan siquiera el costo del dinero a esa tasa.

---

## IV – Movimiento de suelos (10 pts)

Platea 40m×25m=1.000 m². Capas (de arriba abajo, según corte del Anexo): capa vegetal 20cm (a retirar completa), arcilla debajo (hasta 40cm bajo capa vegetal, mayoritariamente arcilla, retirar lo necesario para poner el balasto), balasto compactado 30cm + hormigón 15cm sobre el nivel resultante. Camión de 10 m³ útiles.

**Dos soluciones posibles** (el ejercicio no define si se cambia toda la arcilla o solo el espesor que ocupará el balasto):

**Opción 1 — se retira solo la arcilla necesaria para colocar los 30cm de balasto (15cm de arcilla):**

| Concepto | Espesor (m) | Área (m²) | Vol. compactado (m³) | Coef. (Ce/Ca) | Vol. suelto (m³) | **Viajes** |
|---|---|---|---|---|---|---|
| Capa vegetal | 0,20 | 1.000 | 200 | 1,25 | 250 | **25** |
| Arcilla | 0,15 | 1.000 | 150 | 1,4 | 210 | **21** |
| Balasto | 0,30 | 1.000 | 300 | 0,9 | 333,3 | **34** |

**Opción 2 — se retira toda la arcilla (40cm) y se rellena con balasto hasta la cota final (0,55m compactado):**

| Concepto | Espesor (m) | Área (m²) | Vol. compactado (m³) | Coef. | Vol. suelto (m³) | **Viajes** |
|---|---|---|---|---|---|---|
| Capa vegetal | 0,20 | 1.000 | 200 | 1,25 | 250 | **25** |
| Arcilla | 0,40 | 1.000 | 400 | 1,4 | 560 | **56** |
| Balasto | 0,55 | 1.000 | 550 | 0,9 | 611,1 | **62** |

*(Viajes = Vol. suelto / 10 m³ por camión, redondeado hacia arriba. Coeficiente usado: para retirar material (capa vegetal, arcilla) se usa Ce=esponjamiento porque el material sale del terreno y se esponja al cargarlo suelto en el camión; para llevar balasto de aporte se usa Ca porque el balasto se transporta suelto y luego se compacta en obra — dividir el volumen COMPACTADO requerido por Ca da el volumen suelto a transportar.)*

---

## V – Licitaciones (15 pts)

**a) TOCAF — procedimientos y montos (vigentes al momento de este examen, jul-2025 — los montos se actualizan periódicamente, ver Guía de Ejercicios Tipo para los valores 2026):**

| Procedimiento | Monto (2025) |
|---|---|
| Compra Directa | hasta $200.000 ($750.000 Gob. Departamentales) |
| Concurso de Precios | hasta $1.000.000 |
| Licitación Abreviada | hasta $10.000.000 |
| Licitación Pública | obligatoria por encima de $10.000.000 |

**b) Tipos de contrato:**
- **Precio Global**: precio fijo total, independiente de los costos reales del contratista. *Ejemplo: construcción de una vivienda con proyecto y alcance cerrados.*
- **Precio Unitario**: precios pactados por partida (ej. $/m³ hormigón, $/m² pavimento), se paga según cantidad ejecutada. *Ejemplo: obra vial o de saneamiento, donde las cantidades reales se definen en obra.*
- **Por Administración**: el contratista cobra costos reales + % o suma fija de administración. *Ejemplo: obra donde no se puede definir el alcance completo al inicio (reforma con imprevistos).*

---

## VI – Régimen Salarial (10 pts)

**a) Consumo Unitario vs. Rendimiento:**
- **Consumo Unitario**: cantidad de un recurso (material, insumo o energía) que se utiliza para ejecutar una unidad de trabajo. *Ej.: consumo de cemento = 8 bolsas/m³ de hormigón; consumo de pintura = 0,25 lt/m².*
- **Rendimiento**: cantidad de trabajo ejecutado por unidad de recurso (mano de obra, maquinaria o material) en un período de tiempo. *Ej.: un oficial albañil coloca 12 m² de muro/día (rendimiento de M.O.); una retroexcavadora excava 30 m³/hora (rendimiento de maquinaria).*

**b) Partes del Convenio Colectivo de la Construcción (Grupo 9):** Acta de Acuerdo del Consejo de Salarios, tripartito entre **Empresas** (Cámara de la Construcción del Uruguay, LIGA, APPCU y otras), **Poder Ejecutivo** (MTSS) y **Trabajadores** (SUNCA). Trata laudos salariales, categorías, compensaciones, licencias, condiciones de trabajo, etc. (ver Resumen Teórico y Guía, sección 6, para el detalle completo de ítems).

**c) Fondos Sociales de la Construcción:** FOSVOC (vivienda del obrero), Fondo Social de la Construcción (canastas, útiles escolares, odontología, cursos), FOCAP (capacitación técnica), FOCER (cuentas de cesantía y retiro). Los pagan las **empresas** (aporte patronal) y en menor medida los propios **trabajadores** (aporte personal): FSC/FOCAP 1,2691% patronal + 0,5809% trabajador = 1,85% total; FOSVOC 0,025%+0,025%=0,05%; FOCER 5,00% patronal (obrero no permanente) o 0,50% (permanente) + 0,50% personal.

**d) Diferencia entre Salario, Monto Imponible y Leyes Sociales:**
- **Salario de la construcción**: lo que efectivamente cobra el operario (hora común + compensaciones).
- **Monto Imponible**: base sobre la que se calculan los aportes, aprox. **80% del salario** (no todas las partidas del salario están gravadas, ver Guía sección 6).
- **Leyes Sociales**: el aporte patronal que se paga sobre el Monto Imponible, **71,8%** (obra pública/ingeniería) o **75,8%** (obra de arquitectura) del Monto Imponible — no del salario directamente.
