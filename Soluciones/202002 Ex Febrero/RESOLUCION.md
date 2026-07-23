# Examen Costos (2240) — 29/01/2020 ("Febrero 2020")

Fuente: `Exámenes/202002 Ex Febrero/Examen Costos 02-2020.pdf` (letra + Anexo I y II) + `Examen Costos Feb-2020 - Preg A,B,D.pdf` (planilla oficial de A, B y D). **Partes A, B y D verificadas contra la planilla oficial. Partes C, E y F son teóricas, sin solución oficial en el repo (respondidas con el criterio de la Guía).**

## Enunciado resumido

- **A. Metraje Hormigón (20 pts):** volumen, cuantía de acero y tenor de encofrado de una pieza prefabricada de hormigón armado (viga+ménsula, croquis Anexo I), longitud 3,5 m.
- **B. Punto de Equilibrio (15 pts):** (a) precio de venta unitario para que el PE se dé al 80% de la capacidad máxima. (b) % de reducción de costos fijos necesario para llevar el PE al 70% de la capacidad.
- **C. Seguros para las Obras (15 pts):** finalidad general de los seguros de obra, componentes de una póliza, los 4 seguros más usuales y qué cubre cada uno.
- **D. Ajuste de Precios (20 pts):** finalidad y expresión genérica de la fórmula paramétrica; proponer una fórmula concreta para hormigones armados a partir de una tabla de insumos (Anexo II).
- **E. Estudio Comparativo de Ofertas (10 pts):** documentación a entregar por el contratante y criterios de comparación de ofertas.
- **F. Costo de Equipos (10 pts):** explicar Depreciación e Interés Horario como componentes del costo de un equipo.

---

## A. Metraje — pieza prefabricada (viga + ménsula/nervio)

**Geometría (Anexo I):** pieza prefabricada de 3,5 m de longitud, sección compuesta por una "mesa"/ala superior (con una zona en voladizo de 20 cm, notch de 10 cm) y un nervio/pilar vertical inferior de 30 cm de ancho, con capas de armadura escalonadas (Ø8, Ø12, Ø16 en la mesa; Ø8/20 y Ø12/15 en el nervio; estribos Ø6/15). El croquis rotado con múltiples cotas parciales (10-15-10, 20, 175, 100, 30) no permite reconstruir con certeza absoluta el desglose barra a barra a partir del escaneo — se usan los valores de la **planilla oficial**, ya resuelta, validando que Tenor y Cuantía cierren exactos a partir de los totales (mismo criterio que en Marzo-2024/Feb-2022 ante croquis ambiguos, ver Guía sección 1).

**a) Volumen de hormigón:** Sección = 0,76 m² × Longitud = 3,5 m → **Volumen = 2,65 m³.**

**b) Acero — planilla oficial (kg totales, con desperdicio incluido por diámetro: 5% Ø6/Ø8, 10% Ø10/Ø12, 15% Ø16):**

| Familia | Ø | Long. c/u (m) | Cant. | Kg con desp. |
|---|---|---|---|---|
| Transversales inferiores | 8 | 2,25 | 19 | 17,3 |
| Transversales superiores | 12 | 3,85 | 24 | 91,7 |
| Estribos | 6 | 3,36 | 24 | 18,9 |
| Longitudinales | 8 | 3,61 | 21 | 31,4 |
| Longitudinales | 16 | 3,77 | 2 | 13,7 |
| Longitudinales | 12 | 3,69 | 2 | 7,2 |
| Longitudinales | 10 | 3,65 | 6 | 14,9 |
| **Total** | | | | **195,2 kg** |

**Cuantía = 195,2 / 2,65 = 73,6 kg/m³.**

**c) Encofrado:** perímetro a encofrar × longitud = 4,94 × 3,5 = 17,29 m² + tapas verticales laterales (los 2 extremos de la pieza) 1,52 m² = **18,81 m² de encofrado total**.

**Tenor = 18,81 / 2,65 = 7,10 m²/m³** (valor alto, esperable en una pieza prefabricada de sección delgada/compuesta — más superficie de molde relativa al volumen que un elemento macizo simple, mismo razonamiento que en la variante de pilar delgado de Jul-2025, ver Guía sección 1).

---

## B. Punto de Equilibrio

**Concepto:** Punto de Equilibrio (PE) = nivel de producción/venta donde Ingresos Totales = Costos Totales (CF+CV), resultado nulo: `Q_PE = CF/(Pu−Cvu)`, o directo desde la producción objetivo: `Pu = (CF+CV_total)/Q_PE`.

**a) Precio de venta para que el PE se dé al 80% de la capacidad máxima:**

| | Valor |
|---|---|
| Costo variable unitario | 250 USD/unidad |
| Costo fijo mensual | 40.000 USD/mes → **480.000 USD/año** |
| Producción máxima | 100.000 u/año |
| Producción de equilibrio (80%) | **80.000 u/año** |
| Costo variable anual (80.000×250) | 20.000.000 USD/año |
| **Costo total** | **20.480.000 USD/año** |
| **Precio de venta de equilibrio = 20.480.000/80.000** | **256,00 USD/u** |

**b) Reducción de costos fijos para que el PE pase al 70% de la capacidad máxima**, manteniendo el mismo precio de venta (256 USD/u) y el mismo costo variable unitario (250 USD/u):

Como `Pu` y `Cvu` quedan fijos, el margen de contribución por unidad (`Pu−Cvu=6`) también queda fijo — el costo fijo necesario para que el equilibrio "calce" exactamente a una nueva cantidad Q' es directamente **proporcional a Q'**: `CF' = CF × (Q'/Q) = CF × (70/80)`.

| | Valor |
|---|---|
| Producción de equilibrio (70%) | 70.000 u/año |
| Costo variable anual (70.000×250) | 17.500.000 USD/año |
| Costo total (a Pu=256: 256×70.000) | 17.920.000 USD/año |
| Costo fijo anual necesario (17.920.000−17.500.000) | 420.000 USD/año → 35.000 USD/mes |

**Reducción = 1 − 70/80 = 1 − 0,875 = 12,5%.** Los costos fijos deben reducirse un **12,5%** respecto de los 40.000 USD/mes previstos (verificación directa: 70/80=0,875, reducción=1−0,875=12,5%, sin necesidad de repetir todo el cálculo del costo total — atajo válido siempre que Pu y Cvu no cambien).

---

## C. Seguros para las Obras (sin solución oficial — teórico, criterio de la Guía)

**a) Finalidad general:** transferir a un tercero (asegurador) el riesgo de siniestros que puedan afectar la obra, al personal o a terceros durante la ejecución, protegiendo el patrimonio del contratista y del comitente ante eventos que de otro modo comprometerían la viabilidad económica del contrato (daños materiales, responsabilidad civil, accidentes laborales).

**b) Componentes principales de una póliza:** (1) objeto/bien asegurado y suma asegurada; (2) riesgos cubiertos y exclusiones; (3) vigencia (fecha de inicio y fin, coincidente con el plazo de obra + eventual extensión); (4) prima (costo, habitualmente % anual de la suma asegurada); (5) franquicia/deducible a cargo del asegurado; (6) condiciones particulares y generales (obligaciones de ambas partes, procedimiento de denuncia de siniestro).

**c) Los 4 seguros más usuales en obra:**
1. **Todo Riesgo Construcción / Incendio:** cubre daños materiales a la obra en ejecución (incendio, robo, fenómenos climáticos, derrumbe).
2. **Responsabilidad Civil (RC):** cubre daños a terceros (personas o bienes ajenos a la obra) originados por la ejecución de los trabajos.
3. **Accidentes de Trabajo (BSE en Uruguay):** obligatorio por ley, cubre al personal afectado a la obra ante accidentes laborales y enfermedades profesionales.
4. **Equipos y Maquinaria:** cubre daños o pérdida de los equipos propios o de terceros afectados a la obra.

---

## D. Ajuste de Precios — Fórmula Paramétrica

**Finalidad:** reconocer, mediante una fórmula matemática, la variación de los costos de los insumos de una obra a lo largo del tiempo de ejecución, para que el precio del contrato se mantenga actualizado sin necesidad de renegociar cada certificado. **Expresión genérica:** `Coef. de ajuste = Σ (aᵢ × Pᵢ/Pᵢ₀)`, donde cada `aᵢ` es la incidencia (%) del insumo *i* en el costo total (Σaᵢ=1 ó 100%) y `Pᵢ/Pᵢ₀` es la relación entre el valor del índice representativo de ese insumo en el mes de aplicación y su valor base (mes "sub 0", el del boletín vigente al momento de la oferta).

**Ejemplo con los datos del examen (hormigón armado):** de la tabla de insumos (Mano de Obra $300.000, Cemento $130.000, Arena $190.000, Piedra partida $210.000, Hierro $150.000, Madera $100.000, Varios $50.000, Indirectos $180.000 a asignar proporcionalmente, Beneficio 15% sobre costo total) se calcula la incidencia % de cada insumo sobre la Venta Total y se **redondea** a coeficientes "limpios" que sumen 100% (ej. Mano de Obra 20%, Cemento 9%, Arena 13%, Piedra 14%, Hierro 10%, Madera 7%, y el resto —27%— se reparte entre el parámetro Costo de Vida (CV, representa "Varios"+indirectos+beneficio, rubros sin insumo físico específico) y el parámetro Dólar (D, si hay insumos importados)). Del Anexo II se elige el índice representativo de cada rubro (ej. J=Jornal Medio Oficial CAT V, M1=Cemento Portland, M2=Arena Gruesa, M3=Agregados Pétreos, M4=Hierro 12mm, M5=Madera de Encofrado, CV=Costo de Vida Base Dic-2010, D=Dólar).

**No hay una única forma correcta de repartir el 27% restante entre CV y D** — la planilla oficial muestra **4 repartos igualmente válidos** (13,5%/13,5%, 27%/0%, 15%/15%, 30%/0% para CV/D respectivamente), mismo criterio ya visto en Marzo-2024 (Guía sección 8): lo importante es justificar la elección (si hay insumos con componente importado relevante, dar más peso a D; si no, concentrar todo en CV) y que los coeficientes sumen 100%.

---

## E. Estudio Comparativo de Ofertas (sin solución oficial — teórico, criterio de la Guía)

**a) Documentación a entregar por el contratante a los oferentes:** pliego de condiciones (generales y particulares), planos y memoria descriptiva del proyecto, especificaciones técnicas, cómputo métrico/lista de rubros a cotizar (para que todas las ofertas coticen exactamente lo mismo y sean comparables), plazo de obra previsto, forma de pago, garantías exigidas, y toda información de sitio relevante (estudio de suelos, relevamientos existentes) que condicione el costo.

**b) Criterios de comparación a considerar por el contratante:** no comparar solo el precio final — evaluar también plazo de ejecución ofertado, antecedentes y solvencia técnica/financiera del oferente, cronograma de pagos propuesto, calidad de los materiales/soluciones técnicas ofrecidas cuando el pliego lo permite, coherencia interna de la oferta (precios unitarios razonables, sin desvíos anómalos que sugieran error o riesgo de incumplimiento), y cumplimiento formal de toda la documentación solicitada (para asegurar que las ofertas sean efectivamente comparables entre sí).

## F. Costo de Equipos (sin solución oficial — teórico, criterio de la Guía)

**a) Depreciación:** representa la pérdida de valor del equipo por su uso a lo largo de su vida útil; es la forma de recuperar, a través del costo horario cobrado en cada obra, la inversión inicial neta de su valor residual. Se determina como `(VN−VR)/(n×H)`, donde VN=valor a nuevo, VR=valor residual al final de su vida útil, n=vida útil en años, H=horas de uso productivo por año — el resultado es el costo horario ($/h) de depreciación (ver Guía sección 4).

**b) Interés Horario:** representa el costo de oportunidad del capital inmovilizado en el equipo (lo que ese dinero podría haber rendido invertido de otra forma, o el costo financiero si se financió su compra). Se determina aplicando una tasa de interés anual (i) sobre el **capital medio** invertido durante la vida útil del equipo (no sobre el valor a nuevo completo, porque el capital inmovilizado disminuye a medida que el equipo se deprecia): `Interés horario = [(n+1)×VN + (n−1)×VR] / (2n) × i/H` (ver Guía sección 4, fórmula de interés sobre capital medio).

---

## Resumen de resultados

| Parte | Resultado |
|---|---|
| A.a Volumen hormigón | **2,65 m³** |
| A.b Acero | **195,2 kg** — Cuantía **73,6 kg/m³** |
| A.c Encofrado | **18,81 m²** — Tenor **7,10 m²/m³** |
| B.a Precio de venta de equilibrio (80% capacidad) | **256,00 USD/u** |
| B.b Reducción de costos fijos necesaria (para PE al 70%) | **12,5%** |
| D Coeficiente de ajuste — insumos | MO 20%, Cemento 9%, Arena 13%, Piedra 14%, Hierro 10%, Madera 7%, CV+D **27%** (repartible) |
