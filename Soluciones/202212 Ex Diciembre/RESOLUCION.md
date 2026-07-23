# Examen Costos — Diciembre 2022 (14/12/2022)

Verificado contra solución oficial (planilla de cálculo incluida en `Examen Costos 12-2022 - Preg. I,III,V.pdf` — cubre I, III y V). Las Partes II y IV (teóricas) no vienen con solución oficial en el repo — se responden con el criterio de la Guía.

**Ojo:** la letra en PDF de este examen tiene un problema de extracción de texto (fuente corrupta) en las páginas 1-2; los datos completos de la Parte I (anchos, espesores de paquete estructural, pendiente) solo aparecen legibles en el archivo de solución oficial — se usaron esos datos para la resolución.

---

## I – Metraje: movimiento de suelos (30 pts)

**Enunciado:** volumen de desmonte o terraplén general de un tramo de calle de 25,00m entre progresivas A y B (Anexo 1: sección transversal con cordón-cuneta, base, sub-base y tratamiento bituminoso doble).

**Datos:** ancho de media sección=4,50m (ancho total=9,00m); pendiente de la sección=4%; espesores: tratamiento bituminoso 0,03m + base 0,15m + sub-base 0,15m = **0,33m de paquete estructural**; capa vegetal a descartar=0,15m; Coeficiente de aporte=1,11; Coef. esponjamiento=1,25; Coef. compactación=0,72.

**Paso 1 — cota de subrasante en 3 puntos de cada sección (eje "p2" + bordes "p1"/"p3" a ±4,50m, afectados por la pendiente del 4%: ±4,50×0,04=±0,18m), restando el paquete estructural (0,33m):**

| Progresiva | Punto | Cota pavimento terminado | Cota subrasante (−0,33m) | Cota terreno limpio (terreno natural −0,15m capa vegetal) | Diferencia (terreno limpio − subrasante) |
|---|---|---|---|---|---|
| A | p1 | 1,98−0,18=1,80 | 1,47 | 1,85−0,15=1,70 | **+0,23** (desmonte) |
| A | p2 (eje) | 1,98 | 1,65 | 1,70 | **+0,05** (desmonte) |
| A | p3 | 1,80 | 1,47 | 1,70 | **+0,23** (desmonte) |
| B | p1 | 2,43−0,18=2,25 | 1,92 | 1,90−0,15=1,75 | **−0,17** (terraplén) |
| B | p2 (eje) | 2,43 | 2,10 | 1,75 | **−0,35** (terraplén) |
| B | p3 | 2,25 | 1,92 | 1,75 | **−0,17** (terraplén) |

*(diferencia positiva = terreno por encima de la subrasante requerida → sobra material → desmonte; diferencia negativa = subrasante por encima del terreno → falta material → terraplén)*

**Paso 2 — área de cada sección** (2 trapecios de 4,50m de ancho cada uno, entre p1-p2 y p2-p3):
- Área A = 4,50×(0,23+0,05)/2 + 4,50×(0,05+0,23)/2 = 0,63+0,63 = **+1,26 m²** (desmonte)
- Área B = 4,50×(−0,17−0,35)/2 + 4,50×(−0,35−0,17)/2 = −1,17−1,17 = **−2,34 m²** (terraplén)

**Paso 3 — la sección pasa de desmonte a terraplén en algún punto entre A y B** (área cambia de signo): interpolando linealmente sobre los 25,00m según la magnitud de cada área,
- Xₐ (desde A hasta el punto de cruce) = 25,00×1,26/(1,26+2,34) = **8,75 m**
- X_b (desde B hasta el punto de cruce) = 25,00−8,75 = **16,25 m**

**Paso 4 — volumen de cada tramo parcial** (pirámide/cuña: área en el extremo × longitud parcial /2, porque el área decrece linealmente hasta 0 en el punto de cruce):
- **Volumen desmonte parcial = 1,26×8,75/2 = 5,51 m³**
- **Volumen terraplén parcial = 2,34×16,25/2 = 19,01 m³**

**Paso 5 — como el desmonte disponible (5,51 m³) es MENOR que el terraplén necesario (19,01 m³)**, todo el desmonte se reutiliza como terraplén y el resto debe traerse de préstamo (2ª observación del enunciado):
- Volumen de terraplén con material de desmonte = Vol. desmonte / **Coeficiente de aporte** = 5,51/1,11 = **4,97 m³** *(en este examen, "Coeficiente de Aporte" se usa como el factor que convierte volumen de banco/desmonte extraído en volumen de terraplén compactado logrado con ese material — Ca=V.banco aportado/V.compactado logrado; ojo que esta definición es distinta de la usada en Dic-2023 (Ca=Vcompactado/Vsuelto) — **siempre revisar con qué otros datos es consistente el coeficiente antes de aplicarlo**, no asumir la misma fórmula en todos los exámenes.*
- **Volumen de terraplén con material de préstamo = 19,01 − 4,97 = 14,05 m³** ← este es el volumen final "de préstamo" que hay que comprar/transportar.

*(El Coeficiente de esponjamiento (1,25) no se usa en esta pregunta — sería necesario si pidieran el volumen suelto a transportar en camión, no pedido acá.)*

**Resultados finales:** Volumen de desmonte = **5,51 m³** (se reutiliza íntegro como terraplén). Volumen de terraplén total = **19,01 m³**, de los cuales 4,97 m³ salen del propio desmonte y **14,05 m³ deben traerse de préstamo**.

---

## II – Estado Económico y Financiero (10 pts) *(teórico, sin solución oficial en el repo)*

**a) Cronograma Económico vs. Financiero:**
- **Cronograma Económico** (devengado): refleja ingresos (venta) y egresos (costo) en el momento en que se **generan/certifican**, independientemente de cuándo se cobran o pagan. Mide la **rentabilidad** de la obra a lo largo del tiempo.
- **Cronograma Financiero** (caja): refleja los mismos ingresos y egresos pero en el momento en que efectivamente se **cobran/pagan**, según las condiciones reales de pago pactadas (anticipos, plazos, desfases). Mide la **necesidad de caja/financiamiento** de la obra.

**b) Importancia y control:** el Cronograma Económico es la base para controlar la **rentabilidad real** de la obra frente a lo presupuestado (comparando beneficio devengado vs. previsto, detectando desvíos de costo o de productividad). El Cronograma Financiero es la base para controlar la **liquidez**: permite anticipar necesidades de línea de crédito, evitar caer en impagos, y dimensionar el costo financiero de la obra — ambos cronogramas suelen diferir sustancialmente en el tiempo aunque compartan el mismo total final (ver Guía sección 12, variante Marzo-2023).

---

## III – Costos Fijos, Variables (20 pts)

**a) Definición de Punto de Equilibrio:** ver Guía sección 11 — nivel de producción/venta donde Ingresos totales = Costos totales (fijos+variables), beneficio nulo.

**b) Caso: extensión del plazo de 12 a 18 meses (6 meses más) por pedido del comitente, con reconocimiento de sobrecostos a evaluar.**

**Datos (base 100 = costo total original):** Costo fijo original=30% del costo total (30,00); Costo variable=70% del costo total (70,00, **no varía en monto total** aunque cambie el ritmo, porque depende de las cantidades de tarea y los rendimientos quedan inalterados — no del tiempo transcurrido); Beneficio original=20% **sobre el costo** (no sobre la venta) → Venta original=100×1,20=**120,00**; plazo original=12 meses.

**Costo fijo nuevo:** el costo fijo mensual promedio ORIGINAL = 30/12=2,50/mes. El contratista acepta reducir ese costo fijo mensual solo un 10% (queda en 27% del costo mensual promedio ORIGINAL = 2,25/mes), pero ahora se paga durante 18 meses en vez de 12:
**Costo fijo nuevo = 2,25×18 = 40,50** (equivalente a: 30×(18/12)×0,90 = 45,00×0,90 = 40,50 — mismo resultado por las dos vías, ya que la multiplicación es conmutativa).

**Costo total nuevo = 40,50 (fijo) + 70,00 (variable, sin cambios) = 110,50**

**a) Variación del beneficio SIN reconocimiento** (la venta se mantiene en 120,00, el comitente no reconoce nada):
Beneficio nuevo = 120,00−110,50 = **9,50** (contra 20,00 original) → **variación = (9,50−20,00)/20,00 = −52,5%** (el beneficio se reduce más de la mitad). *(Como dato adicional: el beneficio/costo también cae de 20% a 9,50/110,50=8,6%, una reducción del 57,0% en esa relación porcentual.)*

**b) Monto a reconocer para mantener el margen del 20% sobre el costo (nuevo):**
Venta con reconocimiento = Costo nuevo×1,20 = 110,50×1,20 = **132,60**
Reconocimiento en valor absoluto = 132,60−120,00 = **12,60**
**Reconocimiento sobre la venta original = 12,60/120,00 = 10,50%** (el comitente debería reconocer un incremento del 10,5% sobre el precio contratado para que el contratista mantenga su margen del 20% sobre costo).

---

## IV – Mano de Obra y Monto Imponible (15 pts) *(teórico, sin solución oficial en el repo)*

**a) Monto Imponible y cargas sociales (Ley 14.411):** el **Monto Imponible** es la base de cálculo sobre la cual se aplican los aportes del Aporte Unificado de la Construcción — compuesto por el jornal básico más los beneficios sociales de naturaleza salarial (incentivo, descanso, feriados pagos, entre otros). Las **cargas sociales** son el conjunto de aportes patronales y obreros (jubilación, salud, seguro de accidentes, fondo de desempleo, etc.) que en este régimen se centralizan como % sobre el Monto Imponible, en vez de liquidarse tarea por tarea (ver Guía sección 6).

**b) Relación porcentual aproximada:** de forma orientativa, el Monto Imponible ronda el 70-80% del costo de mano de obra total (jornal + beneficios sociales imponibles, sin las partidas no imponibles), y las cargas sociales sobre ese Monto Imponible rondan el 70-80% adicional (según sea obra pública o privada — ver coeficientes usados en Garantías de exámenes anteriores: 71,8% obra pública, 75,8% obra privada).

**c) Partidas — integran el Monto Imponible o no:**

| Partida | ¿Integra el Monto Imponible? |
|---|---|
| 1) Jornal básico | **Sí** |
| 2) Incentivo | **Sí** (remuneración variable, naturaleza salarial) |
| 3) Descanso | **Sí** (pago del descanso semanal, naturaleza salarial) |
| 4) Feriados | **Sí** (feriados pagos, naturaleza salarial) |
| 5) Vestimenta | **No** (partida no remunerativa, provisión en especie/reintegro de gasto) |
| 6) Transporte | **No** (viático/reintegro de gasto, no remunerativo) |
| 7) Herramientas | **No** (herramienta de trabajo, no es remuneración) |

---

## V – Ajuste de Precios (fórmula paramétrica) (15 pts)

**a) Finalidad de las fórmulas paramétricas:** ver Guía sección 8 — actualizar el precio contractual a lo largo de la obra reflejando la variación de los costos reales de los insumos (mano de obra, materiales, combustibles, etc.) entre la fecha de la oferta y cada certificación, para que ni el contratista quede perjudicado por inflación de costos ni el comitente pague de más si algún insumo se abarata.

**Expresión genérica completa:** `Pₙ = P₀ × [a₀ + a₁×(J ₙ/J₀) + a₂×(M ₙ/M₀) + a₃×(CVₙ/CV₀) + a₄×(Dₙ/D₀) + ...]`, donde P₀=precio/certificado base, Pₙ=precio/certificado ajustado, cada índice (J=mano de obra, M=materiales, CV=costo de vida, D=dólar, etc.) representa la variación de un insumo o grupo de insumos entre el momento 0 y el momento n, y cada aᵢ es el peso (%) de ese insumo en el precio total — con la condición **Σaᵢ=1** (incluyendo un término fijo a₀ si se estima una porción no ajustable).

**b) Fórmula propuesta para los hormigones armados de esta obra**, a partir del presupuesto dado:

| Insumo | Monto ($) | % sobre Costo Directo | % sobre Venta Total | Grupo/Índice |
|---|---|---|---|---|
| Mano de obra | 250.000 | 25% | 18,1% | **J** |
| Cemento | 100.000 | 10% | 7,2% | M1 (14,3% del total materiales) |
| Arena | 150.000 | 15% | 10,9% | M2 (21,4%) |
| Piedra partida | 200.000 | 20% | 14,5% | M3 (28,6%) |
| Hierro | 150.000 | 15% | 10,9% | M4 (21,4%) |
| Madera pino Brasil | 100.000 | 10% | 7,2% | M5 (14,3%) |
| Varios | 50.000 | 5% | 3,6% | CV |
| **Costo Directo Total** | **1.000.000** | 100% | 72,5% | |
| Gastos Indirectos (15% del directo, 50%CV+50%D) | 150.000 | | 10,9% | 75.000 CV + 75.000 D |
| Beneficio (20% s/directo+indirecto, ajuste CV) | 230.000 | | 16,7% | CV |
| **Venta Total** | **1.380.000** | | **100,0%** | |

**Agrupando en los 4 índices del mercado** (Jornal, Materiales, Costo de Vida, Dólar):
- **J (mano de obra)** = 250.000/1.380.000 = 18,1% → **18%**
- **M (materiales: cemento+arena+piedra+hierro+madera)** = 700.000/1.380.000 = 50,7% → **51%** — internamente compuesto por M1=15%, M2=20%, M3=30%, M4=20%, M5=15% del subtotal materiales (útil si el índice de "materiales" del organismo se pide desagregado por tipo).
- **CV (costo de vida: Varios + mitad de indirectos + todo el beneficio)** = (50.000+75.000+230.000)/1.380.000 = 25,7% → **26%**
- **D (dólar: mitad de indirectos)** = 75.000/1.380.000 = 5,4% → **5%**

**Fórmula paramétrica final (coeficientes redondeados, suman 100%):**

**Pₙ = P₀ × [0,18×(Jₙ/J₀) + 0,51×(Mₙ/M₀) + 0,26×(CVₙ/CV₀) + 0,05×(Dₙ/D₀)]**

*(Nota metodológica: el Beneficio y los "Varios" se ajustan típicamente por el índice de Costo de Vida (rubro genérico/inflación), y los Gastos Indirectos suelen partirse entre dos índices distintos si mezclan partidas de naturaleza diferente — acá mitad en pesos/Costo de Vida y mitad en insumos dolarizados. Ver Guía sección 8 para más ejemplos.)*

---

## Resumen ejecutivo del examen

| Parte | Resultado clave |
|---|---|
| I – Metraje (movimiento de suelos) | Desmonte=5,51 m³ (se reutiliza íntegro); Terraplén total=19,01 m³ (4,97 m³ de desmonte propio + **14,05 m³ de préstamo**) |
| II – Cronograma Económico vs. Financiero | Económico=devengado/rentabilidad; Financiero=caja/liquidez |
| III – Costos Fijos/Variables | Extensión de plazo 12→18 meses sin reconocimiento: beneficio cae **−52,5%**. Con reconocimiento (mantener 20% s/costo): reconocer **+10,5%** sobre la venta original |
| IV – Mano de Obra y Monto Imponible | Monto Imponible=jornal+beneficios sociales remunerativos (no vestimenta/transporte/herramientas) |
| V – Ajuste de Precios | Fórmula: Pₙ=P₀×[0,18×J+0,51×M+0,26×CV+0,05×D] (coeficientes ejemplo con Beneficio+Varios en CV, medio Indirecto en D) |
