# Examen Costos — Julio 2022 (27/07/2022)

Verificado contra solución oficial (planilla de cálculo incluida en `Examen Costos 07-2022 - Preg. A,B,C,D.pdf` — cubre A, B, C y D). La Parte E (teórica) no viene con solución oficial en el repo — se responde con el criterio de la Guía.

---

## A – Metraje Hormigón, losa L102 (20 pts)

**Enunciado:** volumen de hormigón, tenor de encofrado y cuantía de acero de la losa L102 del Anexo 1 (planta con notación de armado "en cruz" en el centro del paño, como en Ene-2026/Dic-2024/Jul-2024/Feb-2024).

**Vano libre** (regla de oro: se considera losa hasta borde interno de vigas, no se encofran laterales — contenida por vigas en sus 4 lados): leyendo cotas corridas del plano, vertical=8,53−0,43=**8,10m**; horizontal=11,71−6,17=**5,54m**. Espesor e=0,15m.

**Volumen y encofrado** (losa contenida en sus 4 lados → solo encofrado inferior, Tenor=1/e, atajo de la Guía sección 1):
- V = 8,10×5,54×0,15 = **6,73 m³**
- Encof = 8,10×5,54 = **44,87 m²** (área en planta)
- **Tenor = 44,87/6,73 = 6,67 m²/m³** (= 1/0,15, verifica la identidad del atajo)

**Armadura** — dos familias, cada una con barra horizontal y vertical:

| Familia | Dirección | Ø (mm) | Paso | Cant. | L unit. (m) | L tot (m) | kg (c/desp) |
|---|---|---|---|---|---|---|---|
| **A** (fondo, positiva) | horizontal | 16 | 0,15 | 55 | 5,86 | 322,30 | **585,62** |
| **A** (fondo, positiva) | vertical | 10 | 0,23 | 25 | 8,85 | 221,25 | **150,89** |
| **F** (arriba, negativa) | horizontal | 12 | 0,12 | 138 | 2,25 | 310,50 | **303,98** |
| **F** (arriba, negativa) | vertical | 12 | 0,23 | 50 | 1,55 | 77,50 | **75,87** |
| **TOTAL** | | | | | | | **1116,36** |

**🔓 Decodificación adicional de la planilla en "cruz"** (ver Guía sección 1 — venía con un número sin explicar desde Feb-2024): en este plano, la notación central `Ø10 / Ø16 — 15  15 / 23` se lee así, comparado con la planilla oficial: el número de **abajo** (23) es el **paso de la familia vertical** (Ø10/23, rotulado también aparte como "A: Ø10/23"); los **dos números del medio, iguales entre sí** (15 y 15), son el **mismo paso de la familia horizontal repetido** (Ø16/15, rotulado aparte como "A: Ø16/15") — se muestra dos veces porque el paño tiene armadura simétrica a ambos lados del eje central de la cruz, no son dos pasos distintos. La familia "F" (negativa, junto a las vigas) siempre viene rotulada de forma explícita y directa (Ø12/12, Ø12/23), sin ambigüedad — consistente con lo ya visto en exámenes anteriores.

**Resultados finales:**
- Total Vol. hormigón: **6,73 m³**
- Total encofrado: **44,87 m²**
- Total acero (con desperdicio): **1116,36 kg**
- **Tenor de encofrado = 6,67 m²/m³**
- **Cuantía de acero = 1116,36/6,73 = 165,85 kg/m³**

---

## B – Dosificación y Consumos (20 pts)

**Rendimientos:** Of.Carpintero 5,00 + Ayudante 3,00 hs/m³ pasta; Of.Carpintero/Ayudante 0,90 hs/m² encofrado c/u; Of.Herrero/Ayudante 0,04 hs/kg hierro c/u. Chapón fenólico 2,44×1,22m (área=2,98 m²≈3,0 usado en planilla), desperdicio 10%, 5 reúsos.

**Dosificación del hormigón** (método de Coeficiente de Aporte — ver Guía sección 3): relación en volumen aparente Piedra:Arena Gruesa:Arena Fina:Cemento = 3:1:1:1 (6 partes totales); Coef. de Aporte de cada componente = volumen REAL que aporta cada unidad de volumen aparente.

| Componente | Rel. vol. aparente | Coef. Aporte | Vol. real (rel.×Ca) | Vol. aparente para 1m³ | Reducción comercial |
|---|---|---|---|---|---|
| Piedra Partida | 3 | 0,55 | 1,65 | 0,796 | **0,80 m³** |
| Arena Gruesa | 1 | 0,57 | 0,57 | 0,265 | **0,27 m³** |
| Arena Fina | 1 | 0,52 | 0,52 | 0,265 | **0,27 m³** |
| Cemento | 1 | 0,47 | 0,47 | 0,265 | **371,35 kg** (×1400 kg/m³) |
| Agua (a/c=0,4) | — | — | 0,56 | 0,149 | **148,54 lt** |
| **Suma vol. real** | | | **3,77** | | |

*Método: Vol.real total=Σ(rel.aparente×Ca)=3,77 (este es el volumen que realmente ocupan los granos de cada componente sin huecos, para obtener 1 m³ de hormigón compactado). Vol. aparente de cada componente para 1m³ de hormigón = (rel.aparente/3,77)×1 — luego cada uno se expresa en su unidad comercial: Cemento en kg (×1.400 densidad aparente), Agua en litros (=0,4×kg cemento=0,4×371,35=148,54).*

**Consumos unitarios (/m³ de losa):**

| Insumo | Fórmula | Cons. Unitario |
|---|---|---|
| Ayudante (hs) | 3,00 + 6,67×0,90 + 165,85×0,04 | **15,63** |
| Piedra partida (m³) | dosificación | **0,796** |
| Arena gruesa (m³) | dosificación | **0,265** |
| Arena fina (m³) | dosificación | **0,265** |
| Cemento (kg) | dosificación | **371,35** |
| Chapón fenólico (unid) | (6,67×1,10)/(2,98×5) | **0,49** |
| Hierro (kg) | = Cuantía | **165,85** |

*(Of. Carpintero=5,00+6,67×0,90=11,00 hs/m³ y Of. Herrero=165,85×0,04=6,63 hs/m³ no fueron pedidos en el enunciado de este examen pero se calculan con la misma fórmula que Ayudante, cambiando el rendimiento del oficio correspondiente.)*

---

## C – Movimiento de Suelos (20 pts)

**Enunciado:** platea circular previa sustitución de suelo: excavar en un diámetro mayor (según la solución oficial, **260m** — el enunciado literal dice "130 metros", pero el Área oficial de 53.093 m² solo se reproduce con un círculo de 260m de diámetro; se sigue la planilla oficial) hasta 0,60m de profundidad, y rellenar/compactar con material adecuado hasta nivel −0,15m (0,45m de espesor de relleno). 50% del material retirado va a depósito, 50% se acopia en obra.

**Volúmenes:**
- Terreno a excavar: S=53.093 m² (círculo de D=260m), h=0,60m → **V=31.856 m³** (en banco)
- Terreno a sustituir y compactar: mismo S, h=0,45m (desde −0,60 hasta −0,15) → **V=23.892 m³** (compactado)

**Material de préstamo necesario** (fórmula dada en la solución oficial: **V.préstamo = V.compactado / (Ce×Cc)**, con Ce=esponjamiento del material de préstamo=1,35 y Cc=compactación del material de préstamo=0,9): 23.892/(1,35×0,9) = 23.892/1,215 = **19.664 m³** (en piso de cantera, banco).

**Costeo de cada tarea** (Monto Imponible=coef. dado directo por línea; LLss=75,8%×M.Imp., obra privada):

| Tarea | Unidad | Volumen | Costo unit. | Costo total | M.Imp. | LLss |
|---|---|---|---|---|---|---|
| 1. Excavación en banco | m³ | 31.856 | $120,00 | $3.822.690 | $382.269 | $289.760 |
| 2. Material de préstamo en cantera | m³ | 19.664 | $240,00 | $4.719.370 | — | — |
| 3. Excav. material de préstamo | m³ | 19.664 | $120,00 | $2.359.685 | $235.969 | $178.864 |
| 4. Tendido (compactado) | m³ | 23.892 | $40,00 | $955.672 | $143.351 | $108.660 |
| 5. Compactación (compactado) | m³ | 23.892 | $128,00 | $3.058.152 | $238.918 | $181.100 |
| 6. Transporte mat. a retirar (50% a depósito, esponjado ×1,3, dist. 35km) | m³×km | 20.706 | $8,80 | $6.377.521 | — | — |
| 7. Transporte mat. préstamo (esponjado ×1,35, dist. 25km) | m³×km | 26.546 | $8,80 | $5.840.221 | — | — |
| 8. Recepción en depósito (mismo volumen que línea 6) | m³ | 20.706 | $36,00 | $745.425 | — | — |
| **TOTAL** | | | | **$27.878.736** | **$1.000.507** | **$758.384** |

*Volumen de la línea 6 = 50%×(31.856×1,3 esponjamiento) = 50%×41.413 = 20.706 m³. Volumen de la línea 7 = 19.664×1,35 (esponjamiento del préstamo) = 26.546 m³.*

**Resultados finales: Costo total = $27.878.736; Monto Imponible total = $1.000.507; Leyes Sociales totales = $758.384.**

---

## D – Garantías (15 pts)

**Datos:** Costo total=$50.000.000; Beneficio=15% sobre venta (P); IVA=22%; Mano de obra ley 14.411=$10.000.000; obra **privada de arquitectura** → Monto Imponible estimado=**80%** de la mano de obra (dato a estimar, distinto de exámenes donde ya daban directo el "costo de mano de obra imponible") → Leyes Sociales=75,8% (privada). Plazo de ejecución=20 meses; plazo de garantía=12 meses. Costo del seguro: 2% anual del monto a garantizar.

**Precio de venta:** P=Costo/(1−0,15)=50.000.000/0,85=**$58.823.529**. IVA=22%×P=$12.941.176 → Venta c/IVA=**$71.764.706**. Monto Imponible=80%×10.000.000=$8.000.000. Leyes Sociales=75,8%×8.000.000=$6.064.000 → **Venta total IVA+LLss = $77.828.706**.

| Garantía | Monto a garantizar | Período | Monto medio | Costo (2% anual × monto medio × período/12) |
|---|---|---|---|---|
| **a) Fiel cumplimiento** | 10%×77.828.706=$7.782.871 (fijo) | 20 meses | $7.782.871 | **$259.429** |
| **b) Buena ejecución** — I→RP | final: $3.891.435 (5%, crece linealmente) | 20 meses | $1.945.718 | $64.857 |
| **b) Buena ejecución** — RP→RD | $3.891.435 (fijo) | 12 meses | $3.891.435 | $77.829 |
| **b) Buena ejecución — TOTAL** | | | | **$142.686** |

**Costo Total de garantías = 259.429 + 142.686 = $402.115**

---

## E – Seguros para las Obras (15 pts) *(teórico, sin solución oficial en el repo)*

Ver Guía sección 10 (mismo criterio usado en `Soluciones/202303 Ex Marzo/`, parte IV):

**a) Finalidad general:** trasladar a un tercero (asegurador) el riesgo de eventos que pueden generar pérdidas patrimoniales significativas durante la ejecución de la obra, a cambio de una prima cierta y conocida.

**b) Componentes principales de una póliza:** objeto/bien asegurado, riesgos cubiertos (y exclusiones), suma asegurada, prima, franquicia/deducible, vigencia/plazo, beneficiario, condiciones particulares y generales.

**c) Los cuatro seguros más usuales:**
1. **Todo Riesgo de Construcción (TRC):** cubre daños materiales a la obra en ejecución (incendio, robo, fenómenos climáticos, errores de ejecución) — 0,3%-0,5% del valor de obra.
2. **Responsabilidad Civil (RC):** cubre daños a terceros (personas o bienes ajenos a la obra) originados por los trabajos — ~0,3% anual sobre el contrato.
3. **Accidentes de Trabajo:** cubre al personal obrero (monopolio BSE, Ley 16.074) — incluido dentro del Aporte Unificado (Ley 14.411).
4. **Vehículos y maquinaria:** cubre daño/rotura de los equipos propios usados en obra — ~2%/año del valor del equipo.

---

## Resumen ejecutivo del examen

| Parte | Resultado clave |
|---|---|
| A – Metraje | Vol=6,73 m³; Encof=44,87 m²; Tenor=6,67 m²/m³; Acero=1116,36 kg; Cuantía=165,85 kg/m³. Decodificación adicional de la "cruz": dos números iguales = mismo paso horizontal repetido; número inferior = paso vertical |
| B – Dosificación y Consumos | Ayudante 15,63 hs/m³; Cemento 371,35 kg/m³; Chapón fenólico 0,49 unid/m³ |
| C – Movimiento de Suelos | Excavación 31.856 m³; relleno compactado 23.892 m³ (préstamo 19.664 m³ en banco); costo total $27.878.736 |
| D – Garantías | Fiel cumplimiento $259.429 + Buena ejecución $142.686 = **$402.115** |
| E – Seguros | Finalidad, componentes de póliza, 4 seguros usuales (TRC, RC, Accidentes, Vehículos/maquinaria) |
