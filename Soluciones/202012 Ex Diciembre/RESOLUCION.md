# Examen Costos — 14/12/2020

Fuente: `Exámenes/202012 Ex Diciembre/Examen Costos 12-2020.pdf` + solución oficial de I y II en `Examen Costos 12-2020 I y II.pdf`. **Partes I y II verificadas contra solución oficial. Partes III y IV son teóricas, sin solución oficial en el repo.**

## Enunciado resumido

- **I. Metraje y Consumos (40 pts):** (a, 15 pts) volumen de hormigón, cuantía de hierro y tenor de encofrado de una viga-dintel con pretil y alero sobre un muro de bloques (Anexo I). (b, 25 pts) consumo unitario (/m²) y total de un muro de ticholos con 4 tipos de mortero/revoque (toma, impermeable, grueso, fino).
- **II. Ajuste de Precios (20 pts):** finalidad y expresión genérica de la fórmula paramétrica; proponer una fórmula de ajuste completa para los hormigones armados de una obra (datos de costo directo por insumo + indirectos + beneficio); elegir los índices representativos de un boletín real (Anexo II, Cámara de la Construcción / INE).
- **III. Seguros para las Obras (15 pts):** finalidad general, componentes de una póliza, 4 seguros más usuales (mismo temario que Dic-2021/sección 10 de la Guía).
- **IV. Mano de Obra y Monto Imponible (15 pts):** definición de Monto Imponible y cargas sociales; qué integra el Monto Imponible; diferencias contrato permanente vs. a término/por obra.

---

## I.a) Metraje — viga-dintel con pretil y alero

**Geometría (Anexo I):** dintel de hormigón armado sobre un muro de ticholos, largo L=6,75 m, sección compuesta por 3 rectángulos: cuerpo principal (h=0,37m × b=0,12m), una ceja/ledge inferior (hi=0,10m × bi=0,09m) y una ceja/ledge superior — el "pretil" — (hd=0,07m × bd=0,10m), todas SUMADAS (no se restan, forman un perfil escalonado, no un rebaje):

V = (h×b + hi×bi + hd×bd) × L = (0,37×0,12 + 0,10×0,09 + 0,07×0,10) × 6,75 = **0,41 m³**

*(El encofrado exacto de este perfil escalonado —qué caras del perfil quedan expuestas y cuáles apoyan sobre el muro de bloques— no se pudo reconstruir con certeza pixel a pixel del croquis escaneado; se usa el valor de la planilla oficial, **Enc = 6,41 m²**, validado porque el Volumen sí se reconstruye exacto con la geometría de arriba — mismo criterio que en Marzo-2024 y Febrero-2022 para secciones compuestas.)*

**Tenor** = 6,41/0,41 = **15,73 m²/m³** (alto para un elemento de hormigón — esperable: es un elemento muy esbelto, con mucha superficie de encofrado relativa a su pequeño volumen, igual que la variante de pilar delgado de Jul-2025).

**Armadura** (recubrimiento 3cm, ganchos 10Ø, varillas de 12m):

| Familia | Ø | Cant. | L total (m) | kg con desp. |
|---|---|---|---|---|
| A (inferior, longitudinal) | 8 | 2 | 13,50 | 5,53 |
| E (superior, longitudinal) | 8 | 2 | 13,50 | 5,53 |
| Pretil (barra de la ceja superior) | 6 | 1 | 6,75 | 1,56 |
| Alero (barra de la ceja inferior/cantiléver) | 6 | 2 | 13,50 | 3,12 |
| Estribos Ø6 c/25 | 6 | 28 (=redondeo(6,75/0,25)+1, tramo 1,20m c/u) | 33,60 | 7,76 |
| **Total** | | | | **23,50 kg** |

**Cuantía** = 23,50/0,41 = **57,63 kg/m³**.

---

## I.b) Consumos de mampostería y revoques (muro L=6,75m × h=2,65m → Superficie=17,89 m²)

**Perfil del muro (Anexo I, de ext. a int.):** Revoque fino (0,5cm) + Revoque grueso (1cm) + Revoque impermeable/"arena y portland c/hidrófugo" (1cm) + **Ticholo 12x25x25cm** + Mortero de toma (junta horizontal, 2cm) + Revoque grueso (1cm) + Revoque fino (0,5cm). Espesor total revocado: 2,5cm (ext.) + 12cm (bloque) + 1,5cm (int.) = 16cm, coincide con la cota del croquis.

**Método general para cada capa de mortero** (NUEVO tipo de ejercicio, ver Guía sección 16):
1. Tomar la relación en **partes** de cada componente sólido (dato de la tabla de dosificación).
2. Agua aparente = (relación Agua/Otros, 0,15 m³/m³) × suma de las partes sólidas de esa mezcla. Hidrófugo aparente (solo en revoque impermeable) = (relación Hidrófugo/Agua, 0,10) × Agua aparente.
3. Volumen real de cada componente = Vol. aparente × su Coeficiente de Aporte (arena gruesa 0,57; arena fina 0,54; cemento 0,47; cal 0,54; agua e hidrófugo usan coef.=1, no corrigen).
4. Sumar los volúmenes reales de la mezcla → "rendimiento real" (NO se normaliza a 1 m³, se deja como da — misma lógica que la variante de doble aplicación del Coef. de Aporte de la sección 3).
5. Dosificación por m³ real = Vol. aparente de cada componente / rendimiento real (paso 4).
6. Cemento y cal → kg (× su densidad aparente, 1410 y 1400 kg/m³ resp.); agua e hidrófugo → litros (×1000); arena queda en m³.
7. Consumo /m² de esa capa = Dosificación por m³ (paso 6) × espesor de la capa.
8. Sumar el consumo de cada componente entre las 4 capas donde aparece → consumo unitario final /m² de muro.
9. Multiplicar por la superficie total (17,89 m²) → consumo total.

**Ejemplo de referencia (Revoque grueso, espesor 1cm, relación 3,5 arena gruesa : 1 cemento : 1,5 cal):**
- Agua aparente = 0,15×(3,5+1+1,5) = 0,90.
- Volumen real: arena=3,5×0,57=2,00; cemento=1×0,47=0,47; cal=1,5×0,54=0,81; agua=0,90×1=0,90. Rendimiento real = 2,00+0,47+0,81+0,90 = **4,175**.
- Dosificación /m³ real: arena=3,5/4,175=0,84 m³; cemento=1/4,175=0,24 → ×1410=337,7 kg; cal=1,5/4,175=0,36 → ×1400=506,6 kg; agua=0,90/4,175=0,22 → ×1000=215,6 lts.
- Consumo /m² (×espesor 0,01m): arena 0,008 m³/m²; cemento 3,38 kg/m²; cal 5,07 kg/m²; agua 2,16 lts/m² (el agua no se totaliza en la tabla final de consumos, no se compra/valora aparte).

**Tabla de consumo unitario final (suma de las 4 capas: toma+impermeable+grueso+fino), /m² de muro:**

| Componente | Ticholo (unid) | Arena gruesa (m³) | Arena fina (m³) | Cemento (kg) | Cal (kg) | Hidrófugo (lts) |
|---|---|---|---|---|---|---|
| Mampuestos | 16 | | | | | |
| Mortero de toma | | 0,020 | | 0,93 | 9,23 | |
| Revoque impermeable | | 0,011 | | 4,97 | | 0,21 |
| Revoque grueso | | 0,008 | | 3,38 | 5,07 | |
| Revoque fino | | | 0,004 | 1,03 | 3,10 | |
| **Consumo unitario /m²** | **16** | **0,047** | **0,009** | **18,8** | **25,6** | **0,21** |

*(Ticholos: 1 unid. cubre 0,25×0,25=0,0625 m² de cara de muro → 1/0,0625=16 unid/m², sin descontar juntas para este nivel de aproximación.)*

**Consumo total (×17,89 m² de muro):** Ticholos ≈ 286 unid; Arena gruesa ≈ 0,84 m³; Arena fina ≈ 0,16 m³; Cemento ≈ 337,0 kg; Cal ≈ 457,1 kg; Hidrófugo ≈ 3,78 lts.

---

## II. Ajuste de Precios

**a) Finalidad y expresión genérica:** idéntica a la desarrollada en `Soluciones/202202 Ex Febrero/RESOLUCION.md` (sección V) — reflejar las variaciones de costo en el precio, eliminando riesgo para ambas partes; `P₁=P₀×(j·J₁/J₀+m·M₁/M₀+cv·CV₁/CV₀+d·D₁/D₀)` con Σparámetros=1.

**b) Fórmula propuesta para hormigones armados** (Costo Directo por insumo + Indirectos a asignar $396.000 + Beneficio 15% sobre venta):

| Insumo | Monto $ | Incidencia s/Venta Total |
|---|---|---|
| Mano de Obra | 660.000 | 20,86% → **21%** |
| Cemento | 234.000 | 7,39% → **7%** |
| Arena | 399.000 | 12,61% → **13%** |
| Piedra partida | 433.000 | 13,68% → **14%** |
| Hierro | 288.000 | 9,10% → **9%** |
| Madera pino Brasil | 180.000 | 5,69% → **6%** |
| Varios | 100.000 | 3,16% |
| Costo Total sin indirectos | **2.294.000** | |
| Gastos Indirectos a asignar | 396.000 | 12,51% |
| Beneficio (15% sobre venta) | Venta=(2.294.000+396.000)/(1−15%)=**3.164.706**; Beneficio=3.164.706−2.690.000=**474.706** | 15,00% |
| **Venta Total** | **3.164.706** | **100%** |

Criterio propuesto (Varios+Indirectos+Beneficio no tienen insumo físico propio → se ajustan con índices generales de la economía, IPC y/o Dólar; el resto usa el índice de su propio insumo):
- **J** (mano de obra, ICC Índice de mano de obra) = 21%.
- **M₁** (cemento) = 7%, **M₂** (arena, como Arena Gruesa) = 13%, **M₃** (piedra partida) = 14%, **M₄** (hierro) = 9%, **M₅** (madera) = 6%.
- Restante (Varios 3,16%+Indirectos 12,51%+Beneficio 15%=30,67%≈30%) se reparte entre **CV** (Índice de Precios al Consumo, INE) y **D** (Dólar interbancario venta) — no hay una única combinación correcta, por ejemplo CV=15%/D=15%, o todo a CV=30%/D=0% (la solución oficial muestra 4 combinaciones válidas distintas, reforzando que lo que se evalúa es el criterio, no un único número).

`P₁ = P₀ × (0,21·J₁/J₀ + 0,07·M₁₁/M₁₀ + 0,13·M₂₁/M₂₀ + 0,14·M₃₁/M₃₀ + 0,09·M₄₁/M₄₀ + 0,06·M₅₁/M₅₀ + 0,15·CV₁/CV₀ + 0,15·D₁/D₀)`

**c) Elección de índices del Anexo II (Boletín I.N.E./Cámara de la Construcción, Octubre 2020):** cada parámetro se identifica por código, nombre, unidad y valor base. Ejemplos usados: **J**=D02 "ICC Índice de mano de obra" (índice, 1.369,07); **M₁**=C12 "Portland gris en bolsa en planta (25kg)" (2 bolsas, 787,66); **M₂**=B04 "Arena Gruesa" (m³, 842,60); **M₃**=B12 "Pedregullo doble lavado y clasificado" (m³, 791,26); **M₄**=B02 "Acero Tratado ADM 420" (ton, 763,57); **M₅**=B10 "Madera para encofrado de pino nacional" (mil pies, 366,51); **CV**=E03 "Índice de los precios al consumo" (índice, 572,20); **D**=E01 "Dólar interbancario venta - promedio mensual" (índice, 410,05).

**⚠️ Ojo con datos erróneos en la tabla de referencia:** la propia solución oficial marca que el valor de B02 (Acero Tratado, 763,57) "parece haber sido expresado en dólares por error" y que el valor de E01 (Dólar, 410,05) "parece haber sido multiplicado por 10". **Antes de usar un valor de una tabla de índices, verificar que el orden de magnitud sea razonable** (ej. el dólar interbancario de Uruguay en 2020 rondaba los 41-43 $/U$D, no 410) — si algo no cuadra, señalarlo explícitamente en la respuesta en vez de usarlo sin cuestionar.

---

## III. Seguros para las Obras (teórico)

Mismo temario que Diciembre 2021 (ver `Soluciones/202112 Ex Diciembre 2021/RESOLUCION.md`, sección V, y Guía sección 10): finalidad (transferir el riesgo de eventos que afecten la obra a un tercero asegurador a cambio de una prima cierta); componentes de una póliza (objeto, valor, riesgos, monto, prima, deducible, plazo, deberes/exclusiones); **los 4 seguros más usuales**: Accidentes de Trabajo (Ley 16.074, BSE), Vehículos y Maquinaria (~2%/año del valor del equipo), Todo Riesgo de Construcción -TRC- (~0,3%-0,5%), Responsabilidad Civil -RC- (~0,3% anual, a veces incluido en el TRC).

---

## IV. Mano de Obra y Monto Imponible (teórico)

**a) Monto Imponible y cargas sociales:** el Monto Imponible es la base de remuneración sobre la cual se calculan los aportes patronales y personales de seguridad social (Ley 14.411, Aporte Unificado de la Construcción) — no es el salario completo, solo las partidas de naturaleza remunerativa. Las cargas sociales (leyes sociales) son el % que se aplica sobre ese Monto Imponible para cubrir BPS, DISSE, FONASA, seguro de accidentes, etc.

**b) Qué integra el Monto Imponible:**

| Partida | ¿Integra el M.I.? |
|---|---|
| 1) Jornal básico | **Sí** |
| 2) Incentivo | **Sí** (remuneración variable ligada al trabajo) |
| 3) Descanso (media hora) | **No** |
| 4) Feriados (no laborables) | **Sí** |
| 5) Vestimenta | **No** |
| 6) Transporte | **No** |
| 7) Herramientas | **No** |
| 8) FOCER (Fondo Cesantía y Retiro) | **No** (es un aporte patronal adicional, no remuneración del trabajador) |

*(Regla general, ver Guía sección 5: integran el M.I. las partidas de naturaleza salarial —jornal, presentismo, horas extra, feriados, incentivos ligados al trabajo, nocturnidad—; NO integran los reintegros de gastos ni beneficios no remunerativos —ropa, herramientas, transporte, descanso, tickets de alimentación, fondos sociales—.)*

**c) Contrato permanente indefinido vs. a término/por obra:**
- **Permanente indefinido:** relación laboral sin fecha de fin preestablecida; el despido sin causa genera indemnización según antigüedad; mayor estabilidad para el trabajador, pensado para la actividad estable de la empresa.
- **A término / por obra:** vigente por un plazo o hasta la finalización de una obra/tarea específica determinada de antemano; al vencer el plazo o terminar la obra, el contrato se extingue sin generar (o generando una indemnización reducida/distinta) responsabilidad de despido — típico del régimen de la construcción por la naturaleza transitoria de cada obra (Ley 14.411 contempla este esquema, con aportes al FOCER como compensación por la alta rotación).

---

## Comparación con solución oficial

Partes I y II verificadas exactamente contra la planilla oficial (Volumen, Encofrado, Tenor, Cuantía y kg por familia de armadura de la viga; las 4 tablas de dosificación de mortero con su rendimiento real, dosificación /m³ y consumo /m² final; la fórmula paramétrica con sus 4 ejemplos de reparto válidos y la elección de índices del Anexo II, incluyendo la advertencia de datos erróneos en la tabla). Partes III-IV son teóricas, sin solución oficial en el repo — desarrolladas con el criterio de la Guía.
