# Guía de Ejercicios Tipo — Costos (examen práctico y teórico)

Guía acumulativa organizada por tipo de ejercicio. Antes de un examen, repasar cada receta y el mini-ejemplo. Se va enriqueciendo con cada examen resuelto (ver `Soluciones/`).

---

## 1. Metraje de hormigón armado (losas, vigas, pilares, zapatas, muros)

**Cuándo aparece:** casi siempre como Parte I, 20 puntos. Te dan un plano/corte (Anexo) con cotas y una planilla de armaduras, piden volumen de hormigón, tenor de encofrado y cuantía/kg de acero por diámetro.

**Reglas de oro (de "Aclaraciones sobre errores comunes"):**
1. **Volumen de hormigón** = sección × longitud entre elementos de apoyo, según el criterio del elemento (ver tabla abajo). En losas, el volumen es el comprendido **entre vigas** — el volumen de las vigas no es parte de la losa.
2. **Encofrado**: en losas, solo la cara **inferior** por fuera de las vigas (si un lateral de losa no tiene viga, ahí sí hay que encofrar el lateral). Vigas y losas están suspendidas → encofrado inferior salvo que la letra diga lo contrario. Zapatas/muros de contención → apoyan en el suelo, la cara inferior NO se encofra.
3. **Cantidad de barras de una armadura** = redondear hacia arriba(tramo/paso) + 1, donde *paso* = separación entre barras y *tramo* = ancho del espacio donde van (no la longitud de la barra). En losas, el tramo de una franja no incluye la viga.
4. **Longitud de barra** = tramo/longitud real de la pieza + ganchos (10Φ donde no esté especificado) + empalmes (50Φ) si la longitud supera los 12 m de varilla comercial.
5. **Tenor** = área de encofrado / volumen de hormigón. **Cuantía** = kg de hierro / volumen de hormigón. Cada elemento tiene un rango esperable (una losa apoyada en el suelo tendrá tenor mucho menor a una losa suspendida, por ejemplo) — si el resultado se aleja del rango, revisar antes de concluir que hay error; puede haber una justificación geométrica.

**Criterios de volumen por tipo de elemento (Clase 3 — Metrajes de Hormigones):**

| Elemento | Criterio de volumen |
|---|---|
| Hormigón ciclópeo | volumen neto |
| Zapatas | volumen neto de la base + tronco de pirámide (si tiene) |
| Pilares de fundación | sección × altura desde la parte superior de la zapata hasta el nivel superior de la viga que apoya en él |
| Pilares | sección × altura entre niveles superiores de losas adyacentes |
| Vigas | sección × longitud entre pilares de apoyo |
| Losas | espesor × sección comprendida entre vigas de apoyo |
| Carreras, dinteles, antepechos | volumen real |
| Tanques de agua | volumen exterior − volumen interior |
| Escaleras | sección del escalón completo × longitud del escalón |
| General | excepcionalmente se descuenta el volumen del hierro (caso muy particular) |
| Relleno triangular (haunch/cartela entre dos elementos) | **½×base×altura×longitud** — no es un prisma rectangular, hay que usar el área del triángulo (visto en Dic-2023, viga con alero) |

**Armaduras — criterios generales:** se metra por diámetro; se agrupa por nivel y tipo de elemento; empalmes 50Φ como norma; no se descuentan recubrimientos; usar siempre la misma planilla tipo (columnas: Horm. m³ | Encof. m² | Hierro kg | kg por cada diámetro con su % desperdicio). Desperdicios típicos por diámetro (pueden variar según el enunciado, siempre usar la tabla que da el examen): Φ6-Φ8 → 5%; Φ10-Φ12 → 10%; Φ16-Φ20 → 15%; Φ25+ → 15-20%.

**Variante "muro de contención con bloque vibrado"** (visto en Dic-2025): el muro se separa en: hormigón de limpieza (bajo la zapata), zapata/pie de muro, bloques vibro-prensados (con % de sección hueca a rellenar con hormigón — ej. 45% de un bloque 19x19x39), viga de coronamiento. La cantidad de bloques = bloques/m² (dato) × área de muro sin vigas. El volumen de hormigón interior a bloques = cantidad de bloques × %hueco × volumen bruto del bloque. El tenor de encofrado solo se calcula sobre zapata+viga (los bloques no se encofran). Ver `Soluciones/202512 Ex Diciembre 2025/`.

**Mini-ejemplo (pilar 0,6×0,6×0,15 con 1Φ16 por pilar, 4 pilares iguales):**
Vol = 0,6×0,6×0,15×4 = 0,216 m³. Encof (lateral, 4 caras) = perímetro×altura×4 = (0,6×4)×0,15×4 = 1,44... (ajustar según criterio de la pieza). Hierro: long=0,6m×4pilares=2,4m sin desperdicio → con 15% desp. → 2,76m × 1,58kg/m = 4,36 kg (orden de magnitud, ver planilla tipo completa en Clase 3 p.119 para el desglose fila a fila).

**Variante "pilar de piso intermedio con espera de empalme"** (visto en Jul-2025): si el pilar está en un piso intermedio de un edificio de varios niveles, la longitud de cada barra debe incluir la **espera para empalmar con el nivel siguiente** (normalmente 50Φ), además del gancho si corresponde en la base. Un pilar de sección muy delgada (ej. 12cm de espesor) da un **tenor de encofrado más alto de lo típico** — no es un error, es esperable porque la relación superficie/volumen crece cuando una dimensión de la sección es chica; hay que decirlo explícitamente si el examen pregunta "¿es esperable el resultado?". Ver desarrollo completo en `Soluciones/202507 Ex Julio/`.

**Variante "losa angosta de corredor/pasillo, encofrado solo inferior"** (visto en Dic-2024): cuando la
losa está contenida por vigas en sus 4 lados (no hay laterales expuestos), el encofrado es simplemente
Encof=L×b (el área en planta) y por lo tanto **Tenor = Encof/Vol = (L×b)/(L×b×e) = 1/e** — una
identidad matemática directa, sin necesidad de calcular nada más: el tenor depende únicamente del
**espesor** de la losa (a menor espesor, mayor tenor). Útil como atajo para verificar el resultado. Para
leer las cotas del vano libre cuando el plano da distancias eje-a-eje entre vigas (no cotas corridas como
en Marzo-2025): vano libre = cota eje-a-eje − ancho de cada viga limítrofe (ej. 170cm−15cm(viga
izq.)−18cm(viga der.)=137cm). Ver desarrollo completo en `Soluciones/202412 Ex Diciembre/`.

**Variante "muro de contención monolítico en L" (base + pantalla vertical de hormigón armado, sin
bloques)** (visto en Feb-2025): a diferencia de la variante con bloques (Dic-2025), acá todo el muro es
hormigón armado macizo. Se separa en Base (zapata: ancho×espesor×longitud, apoya en el suelo →
no se encofra la cara inferior, solo las 2 caras laterales) y Muro/pantalla (espesor×altura×longitud,
elemento libre → se encofran ambas caras). La armadura tiene dos familias con lógica de conteo
distinta: (a) barras **"longitudinales"** que corren a lo largo de toda la longitud del muro dentro de la
sección transversal (espaciadas verticalmente cada "paso"; cantidad=redondeo hacia arriba(altura del
elemento/paso)+1; si la longitud del muro supera los 12 m de la barra comercial, cada barra lleva 2
empalmes de 50Φ por unidad de longitud continua); y (b) barras **"transversales"** que son la
armadura propia del corte (leída directamente del plano de detalle, con su gancho/anclaje incluido),
repetida cada "paso" a lo largo de toda la longitud del muro (cantidad=redondeo hacia
arriba(longitud_muro/paso)+1, sin empalme porque cada barra individual es corta). Tenor y cuantía de
un muro son notablemente más bajos que los de una losa (aquí 3,13 m²/m³ y 60,31 kg/m³, contra
6,67/167,20 de una losa) — es esperable, un elemento macizo tiene menos superficie de encofrado
relativa a su volumen y menos densidad de armado. Ver desarrollo completo en `Soluciones/202502 Ex
Febrero/`.

**Decodificación de la planilla en "cruz" — RESUELTA (visto en Feb-2024 y confirmada en Jul-2022):**
comparando contra la solución oficial de ambos exámenes, en el formato `Φ(dir.2) arriba / Φ(dir.1)—paso1
paso2 / paso3 abajo` los 3 números se leen así: el número de **abajo** es el **paso de la familia
vertical** (la que aparece arriba de todo en la cruz, ej. Φ10); los **dos números del medio, casi siempre
IGUALES entre sí**, son el **mismo paso de la familia horizontal repetido dos veces** (no dos pasos
distintos) — se muestra duplicado porque el paño suele tener armadura simétrica a ambos lados del eje
central de la cruz. Ej. (Jul-2022): `Φ10 / Φ16—15  15 / 23` → Φ16 horizontal paso 0,15 (repetido), Φ10
vertical paso 0,23. Cuando el plano trae también rótulos explícitos tipo "Φ6/30", "Φ8/25" o "F:Φ12/12"
junto a otras armaduras (bordes, capa negativa junto a vigas), esos SIEMPRE son directos y sin
ambigüedad — la cruz solo afecta a la armadura "de fondo"/positiva central del paño. Ver desarrollo
completo en `Soluciones/202402 Ex febrero/` y `Soluciones/202207 Ex Julio/`.

**Variante "losa continua de varios paños, doble capa de armado"** (visto en Marzo-2025): cuando el plano muestra **dos capas de armadura** — una de "fondo" (F, positiva, recorre todo el vano en ambas direcciones) y una "de arriba" (A, negativa, refuerzo corto solo sobre los apoyos) — la capa negativa suele estar **duplicada** (una franja junto a cada uno de los dos apoyos de la losa), lo que se ve en la planilla como el doble de barras de lo que daría `ceil(tramo/paso)+1` para una sola franja. Esto es normal en losas continuas con momento negativo importante y produce una **cuantía de acero más alta que en una losa de un solo paño simplemente apoyada** (aquí 167 kg/m³ contra un rango típico de 80-120 kg/m³) — no es error, hay que justificarlo por la doble capa. Para leer las cotas del vano libre en plantas con dimensiones acumuladas ("cotas corridas"): el vano libre entre ejes de viga = diferencia entre la cota mayor y la cota menor de la línea de cotas paralela a esa dirección (ej. 8,53−0,43=8,10 m). Ver desarrollo completo en `Soluciones/202503 Ex Marzo/`.

**Variante "muro de contención en L con armadura tipo estribo/vertical+pie con estribos transversales"** (visto en Jul-2023): otra forma de nombrar/organizar las mismas 2 familias de barras de un muro monolítico en L (ver variante Feb-2025 arriba), útil para reconocer la nomenclatura cuando el examen usa otros nombres: la armadura vertical de la pantalla (que ancla doblada dentro del pie, funcionando como un "estribo" abierto) es la barra **principal a flexión** de la pantalla (aquí Ø12 c/15, cantidad=redondeo(long.muro/paso)+1=135, sin empalme por ser una pieza corta con gancho ya incluido); la horizontal de repartición de la pantalla (aquí Ø6 c/15) SÍ necesita empalme si su longitud (=long. del muro) supera los 12m de la varilla comercial. El **pie/zapata corrida** lleva su propia armadura: longitudinal superior + inferior (corren los 20m del muro, con empalme) y estribos transversales que las atan (barra corta, sin empalme, cantidad según paso a lo largo del muro). **Ojo con enunciados que llaman "viga" a lo que en realidad es la sección del muro** (visto también en el enunciado de Consumos de este examen) — verificar siempre contra el Anexo qué elemento es el que realmente hay que metrar/consumir, no solo el nombre que usa la letra. Ver desarrollo completo (con verificación fila a fila contra la planilla oficial) en `Soluciones/202307 Ex Julio/`.

**Variante "viga T-invertida asimétrica, 3 perfiles de estribo distintos"** (visto en Feb-2022): cuando la sección de una viga es compuesta por dos rectángulos apilados sin encimarse (ala superior ancha, ej. 0,72×0,80, + alma inferior angosta y descentrada, ej. 0,30×0,70 — el volumen SÍ se reconstruye exacto como suma de las dos áreas × longitud, sin necesidad de descontar solapes), el contorno de encofrado deja de ser un rectángulo simple y por eso el plano trae **3 perfiles de estribo distintos** (de menor a mayor perímetro, ej. 2,12 / 3,20 / 5,70 m), cada uno cerrando una porción distinta del alma+ala — todos con el mismo paso y misma cantidad (ceil(largo/paso)+1), solo cambia el perímetro de cada uno. Cuando el croquis escaneado no permite reconstruir con certeza qué caras exactas se encofran (geometría compuesta ambigua a pixel), usar el valor de tenor/Enc de la planilla oficial tal cual, validando que el volumen si cierre exacto — mismo criterio que en Marzo-2024. Ver desarrollo completo en `Soluciones/202202 Ex Febrero/`.

---

## 2. Consumos unitarios de hormigón armado (mano de obra, materiales, encofrado)

**Cuándo aparece:** Parte II, justo después del metraje (10-15 puntos); pide consumos "por m³ de hormigón" de una lista de insumos (Ayudante, Of. Carpintero, Of. Herrero, Hormigón premezclado, Acero, Chapón fenólico/Tabla de pino).

**Paso a paso:**
1. Del metraje (parte I) obtener **tenor** (m² encofrado / m³ hormigón) y **cuantía** (kg hierro / m³ hormigón) del elemento. **Ojo:** la cuantía se calcula con el hormigón TOTAL del elemento (incluyendo, si corresponde, el hormigón que no lleva encofrado, ej. relleno de bloques); el tenor solo con el hormigón que SÍ lleva encofrado.
2. Mano de obra (hs/m³) por oficio = 1×(hs/m³ de pasta, dato) + tenor×(hs/m² de encofrado, dato) + cuantía×(hs/kg de hierro, dato). Sumar todas las partidas que correspondan a ese oficio (un oficio puede aportar a más de una tarea, ej. Ayudante aporta a pasta+encofrado+hierro).
3. Hormigón premezclado (m³/m³) = 1×(1+% desperdicio).
4. Acero (kg/m³) = cuantía (con su desperdicio ya incluido si el metraje lo trae incluido).
5. Chapón fenólico / Tabla de pino (unid/m³) = (tenor×(1+%desperdicio)) / (área unitaria de la pieza × cantidad de reúsos).

**Errores comunes:** no hace falta calcular el total de material de la obra, con tenor/cuantía ya se llega directo al consumo por m³ — no hay que "deshacer" a totales y volver a dividir. Escribir siempre las cuentas usadas (piden mostrar el desarrollo).

**Mini-ejemplo:** Encofrado 3,08 m²/m³, desperdicio tabla 15%, reúsos 3, tabla de 3,30m×0,15m (área unitaria 0,495 m²) → (3,08×1,15)/3 = 1,18 m²/m³ equivalente → 1,18/0,495 = **2,38 unidades de tabla /m³**.

---

## 3. Dosificación y costo de un m³ de hormigón (agregados + cemento + agua)

**Cuándo aparece:** segunda mitad de la Parte II. Dan relación en volumen (ej. 3,5:2:1 = agregado grueso:agregado fino:cemento), relación agua/cemento (kg agua/kg cemento) y densidad aparente del cemento, más coeficiente de aporte y costo unitario de cada componente.

**Paso a paso:**
1. Volumen aparente de cada componente = su parte en la relación dada (ej. grueso=3,5; fino=2; cemento=1, en las unidades de la relación).
2. Volumen real = volumen aparente × coeficiente de aporte (el coeficiente corrige el hecho de que los granos no llenan el 100% del volumen aparente).
3. Verificar que la suma de fracciones (volumen real de cada uno / suma de todos los reales) da 1 → repartir 1 m³ real de hormigón según esas fracciones.
4. Pasar cada fracción a **unidades comerciales**: agregados en m³, cemento en kg (y luego a bolsas de 25kg dividiendo), agua en litros usando la relación a/c sobre el peso de cemento (peso cemento = volumen cemento × densidad aparente).
5. Costo = cantidad en unidad comercial × costo unitario; sumar todos los componentes (el agua normalmente no se cobra aparte).

**Mini-ejemplo (Dic-2025):** relación 3,5:2:1, a/c=0,50, dens. cemento 1.400 kg/m³. Cemento real 0,47 m³ → 0,47×1.400=658 kg → como el coeficiente de aporte ya reparte los 4,24 m³ aparentes en 1 m³ real, el cemento resultante por m³ de hormigón es 330,58 kg = 13,22 bolsas × 220 $/bolsa = 2.909 $. Agregado grueso 0,83 m³ × 1.250 $/m³ = 1.033 $. Total materiales ≈ **4.344 $/m³**.

**Variante "doble aplicación del Coeficiente de Aporte" (visto en Feb/Marzo-2024):** algunas planillas oficiales hacen el camino completo en 3 pasos en vez de ir directo: (1) **Volumen real** de la mezcla dada = cada término de la relación × su Coef. de Aporte (ej. relación 4,5:3:1 → Grueso 4,5×0,55=2,48 m³, Fino 3×0,57=1,71 m³, Cemento 1×0,47=0,47 m³; más el agua = kg cemento×a/c). Sumar todo = volumen real que rinde la mezcla (ej. 5,495 m³). (2) **Normalizar a 1 m³ real** dividiendo cada componente por esa suma (ej. Grueso 2,48/5,495=0,45; deben sumar 1). (3) **Volver a volumen "aparente"/comercial** dividiendo CADA UNO otra vez por su propio Coef. de Aporte (ej. Grueso 0,45/0,55=0,82 m³ — esta es la cantidad que efectivamente se compra/mide suelta). El agua no pasa por el coeficiente de aporte: se prorratea directo del total de la mezcla sobre el volumen real total. **No es un error usar el coeficiente dos veces** — la primera vez convierte "aparente dado → real", la segunda "real normalizado → aparente a comprar"; son direcciones opuestas de la misma conversión. Ver desarrollo completo en `Soluciones/202403 Ex marzo 2024/`.

---

## 4. Costo horario de equipos

**Cuándo aparece:** Parte III, 15 puntos. Piden costo horario de producción de un equipo (retroexcavadora, motoniveladora, etc.) separando costo y leyes sociales (LLSS), a veces agrupado en "costo operativo / costos fijos / costo de mantenimiento".

**Datos típicos:** VN (valor nuevo), VR (valor residual), n (años de amortización), H (horas de uso al año — si no se aclara "al mes", asumir anual, coherente con que el resto de tasas son anuales), i (tasa de interés anual), s (seguro anual %), p (patente anual %), K (tasa de leyes sociales sobre el monto imponible ≈70-76%), u (monto imponible como % del jornal ≈80%), consumos de combustible/lubricantes/neumáticos por hora y su costo unitario, jornales de ayudante y maquinista.

**Paso a paso (todo llevado a $/hora, cuidado con la conversión U$D→$):**

1. **Vida útil en horas:** VU = n × H.
2. **Amortización** = (VN−VR)/VU → costo fijo.
3. **Seguro** = s×VN/H → costo fijo.
4. **Patente** = p×VN/H → costo fijo (similar al seguro).
5. **Costo financiero** = [(VN−VR)/2 × i] / H → costo fijo (interés sobre el capital medio invertido en el equipo).
6. **Combustible** = consumo (lt/h) × precio ($/lt) → costo operativo/variable.
7. **Lubricantes** (aceite + grasa + filtro) = consumo × precio de cada uno (si el filtro viene como "% s/lub", tratarlo con la misma lógica cantidad×precio, explicitando el supuesto) → costo de mantenimiento.
8. **Tren de rodado / neumáticos** = (1 juego / horas de vida útil del juego) × costo del juego → costo de mantenimiento.
9. **Mano de obra (ayudante + maquinista)** = horas-hombre/hora-máquina × jornal $/hh → costo operativo. Si hay % de reparaciones (alfa) dado directamente sobre la amortización, sumarlo también como costo de mantenimiento: Reparaciones = alfa × Amortización.
10. **Leyes Sociales (LLSS), aparte:** Monto imponible = u × jornal. LLSS = K × Monto imponible. Aplicar a cada categoría de mano de obra y sumar.
11. **Costo total (sin LLSS)** = suma de 2 a 9. **LLSS aparte**. Costo total con LLSS = suma de ambos.

**Errores comunes:** no mezclar U$D y $ sin convertir explícitamente con el tipo de cambio dado; H bajo (equipo poco usado) dispara la amortización/seguro/patente por hora — es un resultado esperado, no un error (ilustra por qué conviene alquilar equipos de uso esporádico en vez de comprarlos).

**Mini-ejemplo (Ene-2026, retroexcavadora combinada):** VN=50.000 U$D, VR=15.000 U$D, n=5, H=180 h/año → VU=900h. Amortización=(50.000-15.000)/900=38,89 U$D/h. Con 1U$D=38,5$ → 1.497,2 $/h. Ver desarrollo completo en `Soluciones/202601 Examen Enero 2026/`.

**Variante "costo directo de una tarea = costo horario de cuadrilla+equipo × rendimiento" (visto en Feb-2025 y Feb/Marzo-2024):** cuando piden el costo directo **unitario de una tarea puntual** (ej. "izado de columna", "excavación") en vez del costo horario del equipo en sí, el camino es: (1) armar el **costo horario de la cuadrilla completa** sumando Mano de Obra (jornales×cant., sin LLSS si el enunciado lo pide así) + Materiales de consumo (combustible, etc.) + Costo de Equipo (Interés+Depreciación+Seguro/Patente horarios, fórmulas de la sección de arriba) + Mantenimiento horario (tasa media×VC/horas); (2) obtener el **rendimiento** de la tarea en horas/unidad (dato directo, o derivado de "X unidades cada Y horas" — ej. 30 columnas en 44 hs/semana → 44/30=1,47 h/columna); (3) **Costo directo unitario = Costo horario total de la cuadrilla × rendimiento (h/unidad)**. Ver desarrollo numérico completo (cuadrilla 3 personas + hidrogrúa, 52,65 U$S/h × 1,47 h/columna = 77,40 U$S/columna) en `Soluciones/202403 Ex marzo 2024/`.

**Variante "fórmula del interés horario sobre capital medio"** (visto en Feb-2025): en vez de dar
directamente "costo financiero = (VN-VR)/2 × i / horas" (forma simplificada de la sección de arriba), a
veces el examen da la fórmula exacta del interés sobre saldo con depreciación lineal:
`IH = [(n+1)·VN + (n-1)·VR] / (2n) · i / (horas trabajadas por año)`. Da el mismo tipo de resultado
(interés sobre el capital medio invertido) pero con una expresión algebraica distinta — usar la fórmula
que dé el enunciado, no memorizar una sola. Mini-ejemplo: VN=100.000, VR=20.000, n=5, i=6%,
2.880 h/año → capital medio=[(6×100.000)+(4×20.000)]/10=68.000 → IH=68.000×0,06/2.880=**1,42
U$S/h**. Ver desarrollo completo (incluye también mantenimiento con tasa creciente por año, promediada
a 5 años) en `Soluciones/202502 Ex Febrero/`.

---

## 5. Costo horario de mano de obra (jornalero)

**Cuándo aparece:** Parte de "Mano de obra", pide el costo horario de un obrero de determinada categoría, dado el laudo vigente (tabla de categorías con $/hora de "hora común").

**Paso a paso:** sumar sobre la hora común de la categoría pedida (y de la Cat. V cuando la partida se calcula "sobre Cat. V"):
1. Hora común (dato de tabla, según categoría).
2. Ropa (5% de Cat. V), transporte (4,374% de Cat. V), herramientas (2% de Cat. V).
3. Presentismo semanal (10,42% de la hora común de la categoría propia) y presentismo mensual (5% ídem) — **si aplica** (asistencia perfecta; en un ejercicio "normal" se asume que sí corresponde salvo que se diga lo contrario).
4. Media hora de descanso: 0,5 × hora común.
5. Feriados no laborables: 7 al año → prorratear (ej. 7/8 si se expresa como fracción de jornada, o directamente como partida anual/horas trabajadas).
6. Tickets de alimentación: $/ticket ÷ horas por ticket (actualmente cada 8 horas).
7. Sumar solo lo que aplica según la hipótesis de la obra: horas extra, nocturnidad, trabajo en altura, plataformas voladas, lluvia/barro/crecidas **NO corresponden** si es una obra interior/sin esas condiciones (leer bien la hipótesis, p.ej. "reforma de un baño, sin horas extra" excluye varias partidas).

**Monto Imponible (para LLSS):** integran siempre el MI: hora común, presentismo semanal y mensual, horas extra, feriados no laborables, nocturnidad, horas en altura. NO integran: ropa, herramientas, transporte, media hora de descanso, pasajes, horas de lluvia, tickets de alimentación. Parcialmente gravadas (sobre-laudo, viático, incentivo por producción): si <30% de la Remuneración Total no se gravan; si superan el 30%, se grava el 50% del excedente.

**Mini-ejemplo:** Cat. VI (Medio Of. Carpintero) hora común $279,92; obra interior sin horas extra → costo horario ≈ hora común + ropa/transporte/herramientas (sobre Cat.V $258,65) + presentismos + media hora + feriados + tickets ≈ **$402,9/hora** (ver detalle en `Soluciones/202512 Ex Diciembre 2025/`).

---

## 6. Leyes sociales y Ley 14.411 (Aporte Unificado de la Construcción)

**Cuándo aparece:** preguntas teóricas de "Mano de obra" (15 pts) — sistema de remuneración, gestión de aportes, Convenio Colectivo, Fondos Sociales.

- El personal con tareas directas en obra tributa el **Aporte Unificado de la Construcción** en vez de Industria y Comercio.
- `TOTAL A PAGAR = [Precio Obra + IVA] + [Monto Imponible de M.O.] × Coeficiente de Aporte Unificado`.
- **Monto Imponible ≈ 80% del salario**. **Leyes Sociales ≈ 71,8% del MI en obra pública/ingeniería o 75,8% en obra de arquitectura** (la diferencia es el CJPPU: 2% obras de ingeniería, 4% obras de arquitectura, Ley 17.738).
- **Convenio Colectivo**: tripartito entre Empresas, Trabajadores (SUNCA) y MTSS/Poder Ejecutivo (homologa); se renueva cada 3 años; fija laudos y su ajuste (ligado a metas de inflación BCU), categorías, licencias, etc.
- **4 Fondos Sociales de la Construcción:** FOSVOC (vivienda del obrero), Fondo Social de la Construcción -FSC- (canastas, útiles escolares, odontología, capacitación), FOCAP (cursos de capacitación técnica), FOCER (cuentas individuales de cesantía y retiro, aportes patronales+personales).

---

## 7. Garantías con perfil variable en el tiempo

**Cuándo aparece:** Parte "Garantías", 15 pts. Piden estimar el costo (prima anual %) de garantías cuyo monto a garantizar varía a lo largo de la obra (ej. Fiel Cumplimiento constante, Buena Ejecución creciente y luego constante, Anticipo decreciente).

**Paso a paso:**
1. Calcular la base sobre la que se aplica cada garantía: Precio con IVA y LLSS incluidos (Fiel Cumplimiento, Buena Ejecución) o Precio sin IVA/LLSS (Anticipo, si así lo indica el enunciado). Para el Monto Imponible de M.O., **puede venir dado directamente** en el enunciado (ej. "Costo total de la mano de obra imponible: $30.000.000", visto en Feb-2024 — en ese caso NO hay que aplicar el 80% ficto, se usa el valor tal cual) o, si no está dado, estimarlo como % del costo (dato u orden de magnitud ~30%, o 80% de la M.O. sujeta a ley) y aplicar el coeficiente de leyes sociales (~71,8% obra pública, ~75,8% obra de arquitectura).
2. Para cada garantía, identificar la **forma en el tiempo** (constante, rampa creciente, rampa decreciente) entre los hitos: Inicio (I), Recepción Provisoria (RP), Recepción Definitiva (RD).
   - Fiel Cumplimiento: monto fijo (% del precio) desde la firma hasta RP.
   - Buena Ejecución: crece linealmente de 0 a su monto máximo entre I y RP (se retiene % de cada certificado, certificación uniforme ⇒ rampa lineal), luego se mantiene constante entre RP y RD (plazo de garantía adicional).
   - Anticipo: monto máximo al inicio, decrece linealmente a 0 durante el plazo de ejecución (se devuelve en cada certificado).
3. Costo de la garantía = **monto medio a garantizar en cada tramo** × tasa anual de la póliza × (meses del tramo/12).
4. Sumar todos los tramos de todas las garantías → costo total de garantías.
5. Comparar el costo total contra el costo/precio de la obra (%) — valores del orden de 0,5%-1,5% se consideran razonables (coherente con las primas de 0,4%-3% vistas en la Clase de Garantías y Seguros).

**Mini-ejemplo:** ver desarrollo numérico completo (Fiel Cumplimiento $1.163.885,88 + Buena Ejecución $989.303,00 + Anticipo $617.647,06 = $2.770.835,94, el 0,99% del costo de obra) en `Soluciones/202512 Ex Diciembre 2025/`.

**Segundo ejemplo completo (Dic-2024, mismas 3 garantías con bases distintas por tipo)**: Fiel
Cumplimiento y Buena Ejecución se calculan sobre el **Precio con IVA y LLSS incluidos**; el Anticipo, si el
enunciado lo indica así, se calcula sobre el **Precio sin IVA ni LLSS**. Fiel Cumplimiento $793.447 (perfil
constante) + Buena Ejecución $674.430 (rampa 0→5% durante ejecución + constante al 5% durante el
plazo de garantía) + Anticipo $588.235 (rampa 20%→0) = **$2.056.112, el 0,65% del precio de venta**.
Ver desarrollo completo (incluye cómo armar el precio con IVA y LLSS paso a paso) en `Soluciones/202412 Ex Diciembre/`.

**Ejemplo de Monto Imponible "a estimar" (Jul-2022):** cuando el enunciado da el costo de mano de obra
sujeta a ley 14.411 (ej. $10.000.000) pero pide "estimar coeficiente para el Monto Imponible" (no lo da
directo como en Feb-2024), usar el ~80% mencionado en el paso 1 de arriba: Monto Imponible=80%×
10.000.000=$8.000.000, y sobre ESE valor aplicar el % de leyes sociales (75,8% obra privada de
arquitectura en este caso). Ver desarrollo completo en `Soluciones/202207 Ex Julio/`.

**Garantías — tabla rápida (qué, cuándo, cuánto, forma):**

| Garantía | Momento | Monto usual | Plazo típico | Forma de constitución |
|---|---|---|---|---|
| Mantenimiento de Oferta | al presentar la oferta | ~1% de la oferta | 3-6 meses | aval, póliza, depósito |
| Fiel Cumplimiento de Contrato | previo a firmar el contrato | ~5-10% del contrato | firma → Recepción Provisoria | aval bancario/póliza de fianza |
| Fondo de Reparo / Buena Ejecución | fraccionada, por certificado | ~5% de c/certificado | hasta Recepción Definitiva | retención directa |
| Sustitución de Fondo de Reparo | previo al inicio de obra | equivalente a lo retenido | hasta Recepción Definitiva | evita costo financiero de la retención |
| Anticipo/Acopio | previo a recibir el anticipo | 100% del anticipo | se devuelve gradualmente | aval/póliza (~3%/año) |

---

## 8. Fórmula paramétrica (ajuste de precios)

**Cuándo aparece:** Parte "Fórmulas Paramétricas", 15 pts.

**Paso a paso:**
1. Objetivo: reflejar las variaciones de costo en el precio de venta, eliminando riesgo tanto para contratista como contratante.
2. Listados de referencia habituales: MTOP-Dirección Nacional de Vialidad, MTOP-Dirección Nacional de Arquitectura, Cámara de la Construcción del Uruguay.
3. Para el rubro dado: calcular cantidad × precio de cada insumo (hormigón, acero, madera/encofrado, mano de obra) → precio total del rubro.
4. % de incidencia de cada insumo = precio parcial / precio total. Redondear a valores que sumen 100% (ajuste fino de cada %, normalmente conviene redondear el de mayor peso para cuadrar la suma).
5. Armar la fórmula: `Precio_n = Precio_0 × Σ (%insumo × índice_n/índice_0)`, eligiendo el índice de referencia más parecido a cada insumo (si no hay un ítem exacto para el hormigón, se puede usar el de cemento, o una combinación cemento+áridos — explicitando el razonamiento).
6. No incluir insumos que no estén especificados en el enunciado (ej. si no dan combustible, no armar un término para combustible).
7. **Gastos Indirectos + Beneficio** (cuando el enunciado deja el criterio "a proponer por el estudiante"): al no tener un insumo físico asociado, se ajustan con un **índice general de la economía** — típicamente el **Índice de Precios al Consumo (IPC)** y/o el **dólar interbancario**, nunca con el índice de un insumo puntual de obra. No hay una única combinación correcta: lo que se evalúa es que el criterio sea razonable y quede explícito.

**Mini-ejemplo:** viga 20x50x1000cm, armadura 80kg/m³ (60$/kg), hormigón 6000$/m³, encofrado 12m²/m³ (300$/m²), M.O. 30hs/m³ (550$/h) → Precio total 30.900$/m³ con incidencias Hormigón 20%, Acero 16%, Madera 11%, M.O. 53% → `Precio_n=Precio_0×(0,53·MOn/MO0+0,20·Cementon/Cemento0+0,16·Acero_n/Acero0+0,11·Madera_n/Madera0)`.

**Segundo ejemplo — armar la fórmula desde un presupuesto completo con Indirectos y Beneficio a repartir
(visto en Dic-2022):** dan Costo Directo desglosado por insumo (Mano de Obra + 5 materiales + "Varios"),
más Gastos Indirectos (15% del directo) y Beneficio (20% s/directo+indirecto), con la consigna de que
"Varios" y el Beneficio ajustan por Costo de Vida (CV) y los Indirectos se reparten 50% CV/50% Dólar.
Método: 1) calcular Venta Total = Directo+Indirecto+Beneficio; 2) expresar cada partida como % de esa
Venta Total (no del costo directo — el % relevante para la fórmula es sobre el precio final); 3) agrupar los
materiales afines en un solo índice **M** (ponderando internamente por su propio peso relativo dentro del
grupo, útil si el organismo pide el índice de materiales desagregado); 4) sumar Varios+Beneficio+mitad
Indirectos al índice **CV**, y la otra mitad de Indirectos al índice **D** (dólar); 5) Mano de Obra queda como
índice **J** solo. Con Directo=$1.000.000 (MO 25%, 5 materiales 10-20% c/u, Varios 5%), Indirecto=$150.000,
Beneficio=$230.000, Venta=$1.380.000 → **Pₙ=P₀×[0,18·Jₙ/J₀ + 0,51·Mₙ/M₀ + 0,26·CVₙ/CV₀ + 0,05·Dₙ/D₀]**.
Ver desarrollo completo en `Soluciones/202212 Ex Diciembre/`.

---

## 9. Licitaciones — TOCAF y tipos de contrato

**Cuándo aparece:** Parte "Licitaciones", 15 pts, en exámenes que no traen "Fórmulas Paramétricas".

**TOCAF (obra pública) — montos de referencia (Sección 2, Art. 33°):**

| Procedimiento | Monto |
|---|---|
| Compra Directa | hasta $630.000 ($987.000 Gob. Deptales.) |
| Concurso de Precios | hasta $1.000.000 |
| Licitación Abreviada | hasta $10.000.000 |
| Licitación Pública | obligatoria por encima de $10.000.000 |

⚠️ **Los montos de Compra Directa y Gobiernos Departamentales se reajustan periódicamente** (en Jul-2025 eran $200.000/$750.000; en el material 2026 figuran $630.000/$987.000) — Concurso de Precios ($1.000.000) y Licitación Abreviada/Pública ($10.000.000) se mantuvieron estables entre esas dos referencias. **Usar siempre los valores que da el enunciado del examen o el material del año en curso**, no memorizar un solo valor fijo.

Excepciones a Licitación Pública (sin importar monto): compras entre organismos estatales, procedimiento desierto, proveedor único, reparación de maquinaria no trasladable, urgencia/emergencia. Contrataciones publicadas en ARCE; control del Tribunal de Cuentas.

**Tipos de contrato:**
- **Precio Global**: precio fijo total, riesgo de sobrecosto en el contratista. Ideal cuando el alcance está bien definido (ej. vivienda con proyecto cerrado).
- **Precio Unitario**: precio por unidad de partida, se paga según cantidad ejecutada. Ideal cuando las cantidades no se pueden fijar de antemano (ej. obras viales, saneamiento).
- **Por Administración**: se pagan costos reales + % de gestión. Ideal cuando no se conoce el alcance real al inicio (ej. reparación tras un siniestro).

---

## 10. Garantías y Seguros (teórico general, sin perfil temporal)

Ver Clase 19 ("Riesgos"): 8 componentes de un seguro (objeto, valor, riesgos, monto, prima, deducible, plazo, deberes/exclusiones). 5 seguros de obra: Accidentes de Trabajo (Ley 16.074, monopolio BSE; incluido en aporte unificado para obreros Ley 14.411), Vehículos y maquinaria (~2%/año del valor del equipo), Todo Riesgo de Construcción -TRC- (0,3%-0,5% obras comunes), Responsabilidad Civil -RC- (~0,3% anual sobre el contrato, a veces ya incluido en el TRC), Otros (diseño, plazos, demanda).

---

## 11. Punto de Equilibrio y costos fijos/variables

**Cuándo aparece:** Parte "Punto de Equilibrio", 15 pts. Suele traer una pregunta conceptual (definir el
punto de equilibrio) y un caso de evaluar un cambio de escenario (campaña de publicidad, cambio de
precio, cambio de mezcla de productos) preguntando si conviene o no.

**Concepto:** el Punto de Equilibrio es el nivel de producción/venta donde **Ingresos Totales = Costos
Totales** (CF+CV), es decir, resultado nulo. `Q_equilibrio = CF / (Pu − Cvu)`.

**Paso a paso para casos de "¿conviene el cambio?" (no piden el punto de equilibrio numérico, piden
comparar dos escenarios):**
1. Partir de la situación base. Si dice que la empresa "no gana ni pierde", ya está en su punto de
   equilibrio → `Ventas1 = Costos1 = CF1 + CV1` (útil como identidad para simplificar todo en función
   de CF1 y CV1, sin necesitar sus valores absolutos).
2. Expresar el escenario nuevo (Ventas2, Costos2) como variaciones porcentuales sobre CF1/CV1: ojo
   que un cambio de **cantidad** afecta tanto a Ventas como al Costo Variable (son proporcionales a
   la cantidad); un cambio de **precio unitario** solo afecta a Ventas; un gasto extra fijo (ej. campaña
   de publicidad) solo afecta al Costo Fijo.
3. Plantear la desigualdad `Ventas2 > Costos2`, sustituir y simplificar — normalmente los términos en
   CV1 y CF1 se factorizan y, como ambos son siempre positivos, el signo de sus coeficientes finales
   determina si conviene siempre, nunca, o depende de la proporción CF1/CV1 de la empresa.
4. Concluir con palabras, no solo con el álgebra: explicar la intuición (ej. "el aumento combinado de
   cantidad y precio supera al aumento de costos, así que conviene sin importar la estructura de
   costos de la empresa").

**Errores comunes:** confundir qué aumenta con la cantidad (CV y Ventas) y qué no (CF, salvo que el
enunciado diga explícitamente que el costo fijo también sube, como una campaña de publicidad).

**Mini-ejemplo (Marzo-2025):** ventas +20% en cantidad y +5% en precio (`VT2=1,26·VT1`), CV +20%,
CF +10% (costo de la campaña) → `VT2−CT2 = 0,06·CV1+0,16·CF1 > 0` siempre (CV1,CF1>0) → **conviene
en todos los casos**. Ver desarrollo completo en `Soluciones/202503 Ex Marzo/`.

**Variante "hallar el precio para que el equilibrio se dé a un % dado de la capacidad"** (visto en
Dic-2024): en vez de pedir el punto de equilibrio en unidades, dan CF, Cvu y una capacidad máxima, y
piden el **precio unitario** tal que el equilibrio se alcance justo al X% de esa capacidad. Paso a paso:
(1) `Q_equilibrio = X% × Capacidad_máxima`; (2) en el equilibrio `Pu × Q_equilibrio = CF + Cvu ×
Q_equilibrio` → despejar `Pu = (CF + Cvu×Q_equilibrio) / Q_equilibrio`. Con ese mismo Pu ya fijado, se
puede calcular el **beneficio máximo** vendiendo el 100% de la capacidad: `Beneficio = Pu×Cap −
Cvu×Cap − CF`, y el margen sobre venta = Beneficio/Venta.

**Variante "apalancamiento operativo al agregar un turno"** (visto en Dic-2024): al duplicar la
capacidad de producción agregando un turno, el CF sube solo por el incremento propio de ese turno
(ej. +$50.000/mes), NO se duplica. Con el mismo precio unitario, el beneficio total puede crecer mucho
más que proporcionalmente al volumen (en el ejemplo, el beneficio casi se triplica al duplicar la
producción) porque cada unidad extra por encima del punto de equilibrio aporta su margen de
contribución (`Pu−Cvu`) casi íntegro al resultado, mientras el costo fijo adicional es chico en
comparación — a esto se le llama **apalancamiento operativo**. Ver desarrollo numérico completo
(precio equilibrio $32,40/u; beneficio 1 turno $3,6M=3,70% s/venta; beneficio 2 turnos $10,2M=5,25%
s/venta) en `Soluciones/202412 Ex Diciembre/`.

**Variante "extensión de plazo por pedido del comitente — impacto en costo fijo y beneficio"** (visto en
Dic-2022): el comitente pide extender el plazo de ejecución (ej. de 12 a 18 meses) por motivos propios,
sin cambiar el alcance/monto de obra. El **costo variable total NO cambia** (las cantidades de tarea y los
rendimientos son los mismos, solo cambia el ritmo). El **costo fijo SÍ cambia**, porque se sigue pagando
mes a mes durante más tiempo — el enunciado suele dar un % de reducción posible del costo fijo
mensual (por eficiencias al bajar el ritmo). Paso a paso: (1) costo fijo mensual nuevo = %reducido ×
(costo fijo mensual PROMEDIO ORIGINAL, = CF original/plazo original — no el costo fijo mensual ya
reducido, para no aplicar el % dos veces); (2) costo fijo total nuevo = costo fijo mensual nuevo × plazo
nuevo; (3) costo total nuevo = costo fijo nuevo + costo variable (sin cambios); (4) si el Beneficio del
contrato original es % **sobre el costo** (no sobre la venta, leer bien el enunciado — acá Venta=Costo×
(1+%beneficio), no Costo/(1−%beneficio)), calcular la Venta original una sola vez y no volver a tocarla
si el comitente "no reconoce" el sobrecosto. (5) **Sin reconocimiento**: Beneficio nuevo = Venta original −
Costo nuevo → variación % = (Beneficio nuevo−Beneficio original)/Beneficio original. (6) **Con
reconocimiento** (el comitente acepta mantener el margen % original, pero sobre el costo nuevo): Venta
con reconocimiento = Costo nuevo×(1+%beneficio) → reconocimiento en $ = Venta con reconocimiento
− Venta original; reconocimiento % = eso / Venta original.

**Mini-ejemplo:** Costo total=100 (CF=30, CV=70), Beneficio=20% s/costo → Venta=120, plazo=12 meses.
Comitente extiende a 18 meses; CF mensual nuevo=27% del CF mensual promedio original (30/12×0,90)
→ CF nuevo total=27%×(30/12)×18=40,50. Costo nuevo=110,50. **Sin reconocimiento:** Beneficio
nuevo=120−110,50=9,50 → **cae 52,5%** respecto al original. **Con reconocimiento:** Venta
nueva=110,50×1,20=132,60 → hay que reconocer **+10,5%** sobre la venta original. Ver desarrollo
completo en `Soluciones/202212 Ex Diciembre/`.

**Variante espejo — "reducción de plazo por pedido del comitente" (visto en "Marzo"-2022, real
15/02/2022):** el caso inverso al de arriba: el comitente pide **acortar** el plazo, y el contratista tiene
holgura para no aumentar el costo variable ni cambiar el costo fijo mensual — el costo fijo **total** baja
simplemente porque se paga durante menos meses. Fórmula: **Costo fijo nuevo = Costo fijo original ×
(plazo nuevo/plazo original)** (proporción directa, sin ningún % de ajuste adicional salvo que el
enunciado lo pida). Si la venta no se revisa (queda igual), el beneficio **aumenta** porque el costo total
baja mientras el precio de venta se mantiene — exactamente lo opuesto al caso de extensión de plazo.
Mini-ejemplo: Costo=100 (CF=20,CV=80), Beneficio=15% s/costo→Venta=115, plazo 20→17 meses (sin
revisión de presupuesto). CF nuevo=20×(17/20)=17,00. Costo nuevo=97,00. Beneficio nuevo=115−97=
18,00 → **aumenta +20,0%**. Ver desarrollo completo en `Soluciones/202203 Ex Marzo/`.

---

## 12. Costo Financiero — Valor Neto Actualizado (VNA)

**Cuándo aparece:** Parte "Costo Financiero", 15-20 pts. Suele incluir una pregunta teórica (definir VNA) y un caso de comparar alternativas de pago/cobro en el tiempo.

- **VNA**: suma de los valores presentes de todos los ingresos y egresos de un flujo, descontados a una tasa de interés/descuento dada. `VNA = Σ Flujo_t / (1+i)^t`.
- Si VNA=0 a la tasa usada, esa tasa ES la TIR del proyecto. Si VNA>0, la inversión rinde más que la tasa de descuento (TIR mayor a la tasa). Si VNA<0, rinde menos (TIR menor).
- **Comparar alternativas de cobro/pago**: traer cada flujo a valor presente con la tasa dada (ej. 20% trimestral) y comparar. La de mayor VNA es la más conveniente para quien cobra (ej. la empresa constructora que recibe pagos).
- **¿La indemnización compensa el costo del dinero?** Comparar el VNA de la alternativa contra el monto original de la deuda/obligación: si VNA resultante > monto original, la alternativa compensa (y supera) el costo financiero de esperar el cobro; si es menor, no lo compensa.

**Mini-ejemplo:** deuda $1.000.000, tasa trimestral 20%, alternativa que paga 350+350+350+300+300 (miles $) al final de cada uno de 5 trimestres → VNA = 1.002,5 (miles $) > 1.000 → SÍ compensa el costo del dinero.

**Aproximar la TIR por interpolación lineal (visto en "Marzo"-2022):** cuando piden estimar la TIR de un
flujo sin calculadora financiera, calcular el VNA a **dos tasas distintas** tales que una dé VNA **positivo**
y la otra **negativo** (la TIR está garantizado que cae entre esas dos tasas, porque el VNA es decreciente
con la tasa de descuento). Interpolar linealmente: `TIR ≈ tasa_baja + [VNA(tasa_baja)/(VNA(tasa_baja)
−VNA(tasa_alta))]×(tasa_alta−tasa_baja)`. **Ojo: esto es solo una APROXIMACIÓN**, no el valor exacto —
el VNA no es lineal en la tasa (es convexo), así que el resultado interpolado se acerca a la TIR real pero
no coincide exactamente (en el ejemplo, interpolando entre 5% (VNA=+246,57) y 12% (VNA=−217,80) da
8,72% aproximado, contra 8,34% de TIR real exacta). Aclarar siempre que es una aproximación si el
enunciado no pide expresamente el método de interpolación. Ver desarrollo completo en `Soluciones/202203
Ex Marzo/`.

**Variante "flujo de caja con anticipo + elección de línea de crédito" (visto en Dic-2023):** en vez de comparar alternativas de cobro, dan un **cronograma de ingresos y egresos mes a mes** y piden armar el flujo financiero y elegir entre líneas de crédito disponibles. Paso a paso:
1. Si hay **anticipo** del cliente (ej. 10% del precio, recibido al inicio y devuelto como quita en cada certificado posterior): armar la fila de ingresos netos = ingresos sin anticipo − quita de cada mes (10% de ese ingreso), sumando el anticipo recibido en el mes 0. El total del anticipo a lo largo de toda la obra da 0 (se devuelve completo).
2. **Flujo mensual = ingresos netos + egresos** (egresos ya negativos); **Flujo acumulado** = flujo acumulado del mes anterior + flujo mensual del mes actual. El mínimo (más negativo) del acumulado es el **déficit máximo a financiar**.
3. Para elegir la línea de crédito: **el interés de usar la línea también se acumula y aumenta el déficit** — no alcanza con comparar el déficit "sin intereses" contra el límite de la línea. Recalcular el flujo acumulado **incluyendo el costo financiero mes a mes** (interés = tasa mensual × |déficit acumulado del mes anterior|, restado como un egreso más) y comparar ESE nuevo mínimo contra el límite de cada línea. Una línea puede parecer suficiente sin intereses y no serlo una vez que se sincera el costo de usarla.
4. El **monto máximo a utilizar de la línea** = el mínimo (peor) valor del flujo acumulado con intereses incluidos. El **total de intereses previstos** = suma de la fila de costo financiero de la línea elegida.

**Mini-ejemplo:** déficit máximo sin intereses $3.930 (miles), por debajo del límite de una línea de $4.000 al 4%/mes → en principio alcanzaría, pero al sumar los intereses mes a mes el déficit acumulado llega a $4.147, **superando el límite de esa línea** → hay que usar una segunda línea de mayor monto (aunque tenga tasa más alta, ej. 5%/mes) → con esa segunda línea, déficit máximo con intereses $4.202 (mes 4), intereses totales $480. Ver desarrollo completo en `Soluciones/202312 Ex diciembre/`.

**Segundo ejemplo — comparar 3 alternativas y ninguna compensa (Feb-2024):** deuda $1.000.000 (miles $),
tasa trimestral 25%, 3 alternativas de pago a 5 trimestres. Se calcula el VNA de cada una (Alt.1=813,
Alt.2=904, Alt.3=655, todas en miles $) y se ordenan de mayor a menor VNA para saber cuál conviene más
a quien cobra (Alt.2 > Alt.1 > Alt.3) — **ojo que la alternativa con mayor monto nominal total no es
necesariamente la de mayor VNA** (Alt.3 suma $2.000 pero todo al final del 5º trimestre, así que su VNA
resulta el más bajo de las tres). Como las 3 VNA quedan por debajo de los $1.000 originales, **ninguna**
alcanza a indemnizar el costo del dinero. Ver desarrollo completo en `Soluciones/202402 Ex febrero/`.

**Tercer ejemplo — caso mixto, solo una alternativa compensa (Jul-2023, el mini-ejemplo de arriba es
justamente esta alternativa 2):** deuda $1.000.000 (miles $), tasa trimestral 20%, 3 alternativas de pago a
5 trimestres (Alt.1: 400+300+300+200+200; Alt.2: 350+350+350+300+300; Alt.3: 0+0+0+0+2.000). VNA:
Alt.1=892, Alt.2=1.003, Alt.3=804. Orden de conveniencia Alt.2>Alt.1>Alt.3. Como solo el VNA de la
**Alt.2 supera los $1.000** originales, es la **única** que compensa el costo del dinero — las otras dos
pagan la deuda "desvalorizada". Ver desarrollo completo en `Soluciones/202307 Ex Julio/`.

**Variante "Cronograma Económico vs. Financiero + línea de crédito, dos alternativas de remuneración"
(visto en "Marzo"-2023, real 16/02/2023):** en vez de comparar alternativas de cobro de una deuda ya
generada, acá se arma **desde cero** el flujo financiero de toda una obra a partir del presupuesto y las
formas de pago. Paso a paso:
1. **Precio de venta**: si el beneficio es % **sobre la venta** (no sobre el costo), P = Costo/(1−%beneficio)
   (no Costo×(1+%beneficio) — error común, ver "Aclaraciones sobre errores comunes").
2. **Cronograma económico** (devengado): venta y costo repartidos uniformemente en los meses de
   ejecución → beneficio mensual = venta mensual − costo mensual, acumulado hasta llegar al %
   beneficio total sobre venta.
3. **Cronograma financiero** (caja): NO usa las mismas fechas que el económico — hay que correr cada
   partida según su forma de pago:
   - Un **anticipo** (ej. 20% de la venta) se cobra todo de una vez en el mes indicado, no repartido.
   - El resto de la venta (ej. 80%, "sin anticipo") se cobra **con el desfase indicado** (ej. 90 días = 3
     meses) respecto del mes en que se devengó/certificó cada tramo — no respecto del final de la obra.
   - Costos con pago **"a 30 días"**: desfasados 1 mes completo respecto del mes en que se incurrieron.
   - Costos con pago **"convenio colectivo"** (mano de obra): suele modelarse con **medio mes de
     desfase** (jornales quincenales) — la mitad del gasto de cada mes cae en ese mismo mes y la otra
     mitad en el siguiente, generando una rampa de entrada y salida (ej. 150k-300k-300k-300k-300k-150k
     para 5 meses de 300k cada uno).
4. **Flujo acumulado** = igual que siempre, saldo mensual acumulado; **línea de crédito mínima
   necesaria = valor absoluto del mínimo (peor) del flujo acumulado**.
5. **Costo financiero, comparar dos alternativas de remuneración de la línea:**
   - **"Remunerando excedentes":** el interés se aplica **con signo** al flujo acumulado de cada mes —
     los meses con saldo **positivo** también generan un ingreso por interés (5%×saldo positivo), no
     solo los negativos generan costo. El flujo acumulado "con interés" de cada mes = flujo acumulado
     plano de ese mes + la suma acumulada de todos los intereses hasta ese mes.
   - **"Remunerando solo necesidades":** el interés **solo se cobra** sobre los meses con saldo negativo
     (0 en los meses positivos, no hay ingreso por intereses ahí).
   - La alternativa "remunerando excedentes" da **siempre un costo financiero total menor (o igual)**
     que "solo necesidades", porque los intereses ganados en los meses de superávit compensan parte
     del costo de los meses de déficit — hay que elegirla si el enunciado permite comparar y elegir.

**Mini-ejemplo:** Costo $5.000.000, beneficio 20% s/venta → Venta=$6.250.000. Línea de crédito mínima
$900.000 (peor mes de caja). Costo financiero con "remunerando excedentes" = −$112.500 (18,20% de
beneficio final) vs. "remunerando solo necesidades" = −$172.500 (17,24%) → **conviene la primera**.
Ver desarrollo completo en `Soluciones/202303 Ex Marzo/`.

**Sub-variante "ajustar un pago para que el VNA sea EXACTAMENTE igual a la deuda" (visto en Feb-2023):**
en vez de solo comparar/ordenar alternativas ya dadas, piden encontrar qué monto X habría que pagar en
un trimestre/período determinado para que el VNA de esa alternativa iguale (ni más ni menos) el monto
nominal de la deuda original. Si el resto de los pagos de esa alternativa es $0 y todo se concentra en un
único período *t*: despejar de `Deuda = X/(1+i)ᵗ` → **X = Deuda×(1+i)ᵗ** (es directamente la deuda
llevada a valor futuro con la tasa de interés, en el período *t*). Si la alternativa tiene otros pagos además
del que se ajusta, primero restar el VNA de esos otros pagos a la deuda y recién ahí despejar X del
período que falta. Mini-ejemplo: deuda $3.000.000 (miles), tasa trimestral 10%, alternativa que paga todo
en el trim5 → X = 3.000×(1,1)⁵ = **$4.832 (miles)**. Ver desarrollo completo en `Soluciones/202302 Ex
Febrero/`.

---

## 13. Movimiento de suelos (viajes de camión)

**Cuándo aparece:** Parte "Movimiento de Suelos", 10 pts. Dan un corte de terreno con capas (capa vegetal a desechar, capas de suelo natural a excavar, capas de aporte a rellenar/compactar) y piden cantidad de viajes de camión (capacidad dada) para cada material.

**Definiciones formales de los 3 coeficientes** (los tres relativos al mismo volumen de referencia, el
**volumen en banco** = material en su estado natural, sin remover): **Esponjamiento (Ce)** =
Vol.suelto/Vol.banco (>1, el material removido ocupa más volumen). **Compactación (Cc)** =
Vol.compactado/Vol.banco (<1, compactado con rodillo/pisón queda más denso que en su estado
natural). **Aporte (Ca)** = Vol.compactado/Vol.suelto (el que se usa para pasar de "cuánto compactado
necesito" a "cuánto suelto transportar", ver paso a paso abajo). **Relación entre los tres: `Ca = Cc/Ce`**
(ya que Cc = Vol.compactado/Vol.banco = (Vol.compactado/Vol.suelto)×(Vol.suelto/Vol.banco) = Ca×Ce).

**Paso a paso:**
1. Para cada capa: Volumen "en banco"/compactado = espesor × área.
2. **Material que se retira** (capa vegetal, suelo natural excavado): pasar a volumen SUELTO usando el coeficiente de **esponjamiento (Ce)**: Vol. suelto = Vol. en banco × Ce (el material esponja al ser removido, por eso ocupa más en el camión).
3. **Material de aporte que se trae y compacta** (ej. balasto para sub-base): el volumen pedido en el enunciado suele ser el volumen ya **compactado** requerido; para saber cuánto material SUELTO hay que transportar, usar el coeficiente de **aporte (Ca)**: Vol. suelto a transportar = Vol. compactado requerido / Ca.
4. Viajes = Vol. suelto / capacidad del camión, **redondeado hacia arriba**.
5. Si el enunciado es ambiguo sobre cuánto suelo natural se retira (ej. "el material de aporte reemplaza a la arcilla" sin precisar si toda la arcilla o solo el espesor que ocupará el aporte), presentar **las dos opciones razonables** y aclarar el supuesto de cada una — no hay una única respuesta "correcta" si el dato es ambiguo.

**Mini-ejemplo:** platea 40×25m=1.000 m²; balasto compactado necesario 30 cm → Vol. compactado=300 m³; Ca=0,9 → Vol. suelto=300/0,9=333,3 m³; camión de 10m³ → 34 viajes (redondeado hacia arriba).

**⚠️ El nombre de la columna del coeficiente varía según el examen** (visto en Jul-2024): a veces la tabla de datos trae 3 columnas separadas (Esponjamiento, Compactación, Aporte) y el coeficiente que efectivamente reproduce `Vol.suelto = Vol.compactado/coeficiente` es el de la columna **"Compactación"**, no el de "Aporte" — mientras que en Jul-2025 ese mismo rol lo cumplía el coeficiente llamado "Ca" (Aporte). **No confiar en la etiqueta**: si el enunciado da un volumen de control (o hay que verificar contra una solución), probar cuál de los coeficientes dados (siempre <1) reproduce el resultado; si no hay forma de verificar, usar el coeficiente conceptualmente correcto según su definición algebraica (Vol.compactado/Vol.suelto), explicitando la elección.

**Variante "terraplén + desmonte del mismo material, con reutilización" (visto en Jul-2024):** cuando el terreno tiene pendiente y hay que nivelarlo antes de colocar las capas de la estructura, en una parte del terreno hay que **rellenar (terraplén)** y en otra hay que **excavar (desmonte)**, ambos del mismo material (ej. arcilla). Si el material desmontado se puede reutilizar como relleno del terraplén, el volumen neto a transportar (import) = (Vol. suelto necesario para el terraplén) − (Vol. suelto que aporta el desmonte), **no** la suma de ambos por separado — sumarlos por separado sobrestima los viajes. Ver desarrollo completo en `Soluciones/202407 Ex julio/`.

**Variante "movimiento general de una calle por secciones transversales con peralte" (visto en Dic-2022):**
cuando piden el volumen de desmonte/terraplén "general" de un tramo de calle (no de una capa
puntual), y el Anexo trae la sección transversal completa (ancho, peralte/pendiente de calzada,
espesores del paquete estructural), el método es por **secciones transversales en cada progresiva**:
1. En cada progresiva (A, B, ...), calcular la **cota de subrasante** en 3 puntos del ancho (borde
   izquierdo, eje, borde derecho): cota de pavimento terminado en cada punto (afectada por el peralte:
   ±ancho_media_sección×pendiente en los bordes) **menos el espesor total del paquete estructural**
   (suma de tratamiento bituminoso+base+sub-base+lo que corresponda).
2. Calcular la **cota de terreno limpio** = cota de terreno natural (dato) **− espesor de capa vegetal a
   descartar** (constante en todo el ancho si el terreno se toma plano en esa progresiva).
3. Diferencia en cada punto = terreno limpio − subrasante: **positiva → sobra terreno → desmonte**;
   **negativa → falta terreno → terraplén**.
4. Área de la sección = suma de 2 trapecios (borde-eje y eje-borde), cada uno = ancho_media_sección
   × (diferencia_borde+diferencia_eje)/2. El signo del área indica si esa progresiva es toda desmonte,
   toda terraplén, o (si dentro de la misma progresiva unos puntos dan + y otros −) una mezcla — acá,
   al ser progresivas completas con un signo cada una, el área total ya sale con signo único por
   progresiva.
5. Si una progresiva da área de desmonte (+) y la otra de terraplén (−) (como A y B en el ejemplo), en
   algún punto **entre A y B** la condición cambia de signo — encontrar ese punto por interpolación
   lineal de las áreas: `X_A = Longitud × |Área_A| / (|Área_A|+|Área_B|)` (y `X_B = Longitud − X_A`).
6. Volumen de cada tramo parcial (una cuña, área decreciendo linealmente de su valor máximo a 0) =
   `Área × X /2` (fórmula de una pirámide/cuña, NO área×longitud entero — ese error duplicaría el
   volumen).
7. Comparar desmonte parcial vs. terraplén parcial (regla dada en el enunciado, igual que en el mini-
   ejemplo de arriba): si el desmonte alcanza y sobra, el terraplén se hace íntegro con material propio y
   el excedente de desmonte se retira; si el desmonte no alcanza, se usa todo como terraplén y el resto
   se completa con material de préstamo — convertir desmonte(banco)→terraplén(compactado) con el
   coeficiente correspondiente (ver alerta de abajo sobre qué coeficiente usar).

**Mini-ejemplo:** tramo 25m, ancho media sección 4,50m, peralte 4%, paquete estructural 0,33m, capa
vegetal 0,15m. Progresiva A: área desmonte=+1,26 m². Progresiva B: área terraplén=−2,34 m². Punto de
cruce: Xₐ=25×1,26/3,60=8,75m, X_b=16,25m. Volumen desmonte parcial=1,26×8,75/2=**5,51 m³**.
Volumen terraplén parcial=2,34×16,25/2=**19,01 m³**. Como el desmonte no alcanza, todo se usa como
terraplén (5,51/1,11=4,97 m³ de terraplén logrado) y el resto (19,01−4,97=**14,05 m³**) es material de
préstamo. Ver desarrollo completo en `Soluciones/202212 Ex Diciembre/`.

**⚠️ Otra vez la alerta del nombre del coeficiente** (ver arriba, Jul-2024/Jul-2025): en este examen
(Dic-2022) el llamado "Coeficiente de Aporte" (1,11) se usó como `Vol.banco aportado = Vol.compactado
÷ Coef.Aporte` — la definición algebraica **inversa** a la que en otros exámenes se llama igual ("Ca=Vol.
compactado/Vol.suelto"). **Antes de aplicar cualquier coeficiente, verificar con qué otro dato dado es
consistente** (¿da un volumen mayor o menor al de referencia? ¿el coeficiente es >1 o <1, y eso es
compatible con la dirección de la conversión que se necesita?) en vez de asumir la misma fórmula usada
en un examen anterior.

**Variante "sustitución de suelo bajo una platea circular, con costeo de cada tarea + leyes sociales"
(visto en Jul-2022):** en vez de solo pedir el volumen, piden armar una **planilla de costeo completa**:
para cada tarea (excavación, compra de material de préstamo, excavación del préstamo en cantera,
tendido, compactación, transporte, recepción en depósito) hay que determinar el **volumen correcto
según en qué estado se mide esa tarea** (banco / suelto-esponjado / compactado — el enunciado lo
aclara tarea por tarea, ej. "medido en piso, antes de ser excavado" = banco; "medido luego de
compactado" = compactado), multiplicar por el costo unitario, y si la tarea tiene mano de obra (dato de
Monto Imponible por unidad), sumar Leyes Sociales=%×Monto Imponible (obra pública o privada, según
corresponda). Fórmula explícita para el volumen de material de préstamo necesario (dato que trae la
propia solución oficial): **V.préstamo(banco) = V.compactado requerido / (Ce×Cc)**, con Ce=esponjamiento
propio del material de préstamo y Cc=compactación propia del material de préstamo — otra fórmula más,
distinta de las dos anteriores, reforzando que **no hay una fórmula universal**, siempre construirla a
partir de las definiciones de Ce/Cc/Ca dadas en cada examen. Volumen a transportar en camión (m³×km)
= volumen SUELTO (esponjado) del material, multiplicado por la distancia — si solo se retira/transporta
una fracción del material excavado (ej. "50% queda para relleno en obra, 50% va a depósito"), aplicar
ese % **después** de esponjar, no antes. Ver desarrollo completo en `Soluciones/202207 Ex Julio/`.

---

## 14. Suministros

**Cuándo aparece:** preguntas teóricas cortas, 10 pts.

- **Identificados**: especificaciones técnicas claras (normas/memorias), incumplimientos explicitados y valorados, proveedores potenciales, ensayos exigibles, lugar de entrega (flete/carga/descarga), necesidad de contrato.
- **Cuantificados**: unidad de medida clara, criterio de desperdicio, cantidad total y plazo de entrega.
- **Valorados**: precio unitario acorde a la unidad definida, con cotización vigente.
- **INCOTERMS**: términos de compraventa internacional que fijan obligaciones/riesgos entre exportador e importador (EXW, FOB, CIF, CFR, FCA, DAP, DDP, etc.).

---

## 15. Clasificación de costos por Naturaleza

**Cuándo aparece:** preguntas teóricas cortas ("Varios"), 5-10 pts (visto en Dic-2024).

Según el criterio usado consistentemente en el material del curso (tabla "Resumen de Insumos" de la
Clase 20, y las tablas de costo directo de los exámenes de Marzo-2025/Dic-2025), los costos de una obra
se agrupan por naturaleza en:

**Costos Directos** (imputables a cada tarea/rubro ejecutado): 1) **Mano de Obra**; 2) **Materiales**
(insumos que quedan incorporados a la obra); 3) **Equipos** (costo horario de la maquinaria propia o
alquilada); 4) **Suministros y Subcontratos** (provisiones/instalaciones a cargo de terceros); 5)
**Varios** (insumos menores no clasificables individualmente).

**Costos Indirectos**: gastos no asignables a una tarea específica pero necesarios para la obra en su
conjunto (dirección de obra, administración, obrador, seguros/garantías, gastos generales de empresa
prorrateados). Costo Directo + Costo Indirecto + Beneficio (margen) = Precio de Venta.

---

## Exámenes ya incorporados a esta guía
- Diciembre-2023: Metraje de viga con alero y relleno triangular (haunch), consumos (HH/m³ más alto visto hasta ahora), costo financiero con flujo de caja + anticipo + elección entre 2 líneas de crédito (el interés de la línea puede hacerla superar su propio límite), fórmula paramétrica/Ce-Cc-Ca/costos por naturaleza (teórico), identificación/cuantificación/valoración de materiales, régimen salarial.
- Febrero-2024 (fecha real 30/01/2024): Metraje de losa suspendida en 4 lados (Tenor=1/e, 4º caso de "cruz" con decodificación parcial de 2 de 3 números), consumos con HH/m³ total, costo financiero/VNA (comparar 3 alternativas de pago, ninguna compensa el costo del dinero), garantías (Fiel Cumplimiento+Buena Ejecución+Anticipo, Mano de Obra Imponible dada directamente), punto de equilibrio (precio a %capacidad + beneficio máximo con margen %), régimen salarial/Convenio Colectivo.
- Marzo-2024 (fecha real 20/02/2024): Metraje de viga de sección compuesta (base+muro+soporte+marco), consumos unitarios, dosificación de hormigón (variante doble aplicación del Coef. de Aporte), costo directo de cuadrilla+equipo aplicado a una tarea (izado de columna con hidrogrúa, rendimiento h/unidad), seguros de obra (teórico), fórmula paramétrica con 4 repartos alternativos válidos para gastos sin insumo físico.
- Jul-2024: Metraje de losa con bordes de escalón (tercer caso de planilla en "cruz", resuelto usando la planilla de armado ya provista en la solución oficial), movimiento de suelos con terraplén+desmonte del mismo material reutilizado (coeficiente "Compactación" ≠ "Aporte" entre exámenes), garantías (Fiel Cumplimiento + Buena Ejecución con base IVA+LLSS), tipos de subcontrato, etapas de gestión de riesgos, TIR/VNA.
- Ene-2026: Costo de equipos (retroexcavadora), teoría de mano de obra/licitaciones/garantías.
- Dic-2025: Metraje muro de contención con bloques, consumos+dosificación de hormigón, fórmula paramétrica, costo horario de obrero, garantías con perfil temporal, suministros/INCOTERMS.
- Jul-2025: Metraje de pilar con espera de empalme, dosificación de hormigón (método detallado para sacar la relación volumétrica agua/cemento), costo financiero/VNA, movimiento de suelos (viajes de camión), TOCAF/tipos de contrato, consumo unitario vs. rendimiento, Convenio Colectivo/Fondos Sociales.
- Marzo-2025: Metraje de losa continua con doble capa de armado (fondo + refuerzo negativo duplicado sobre apoyos), dosificación de hormigón, fórmula paramétrica (criterio para Gastos Indirectos+Beneficio), punto de equilibrio (caso "conviene el cambio"), VNA/TIR (obra vs. inversión), suministros.
- Feb-2025: Metraje de muro de contención monolítico en L (base+pantalla, armado longitudinal+transversal), dosificación de hormigón, costo de equipo (retroexcavadora, fórmula de interés sobre capital medio) + costo directo de excavación, seguros de obra, régimen salarial/Convenio Colectivo/mercado de la construcción, Estado Económico vs. Financiero de una obra.
- Dic-2024: Metraje de losa angosta de corredor (encofrado solo inferior, tenor=1/espesor), consumos unitarios, garantías (3 tipos con bases IVA/LLSS distintas), punto de equilibrio (precio para equilibrio a %capacidad + apalancamiento operativo al agregar turno), fórmula paramétrica sin costo financiero, coeficientes de movimiento de tierra (Ce/Cc/Ca), clasificación de costos por naturaleza.
- Jul-2023: Metraje de muro de contención en L (armadura tipo estribo+pie con estribos transversales), consumos con enunciado inconsistente ("viga"→muro), costo financiero/VNA con 3 alternativas (caso mixto donde solo una compensa), garantías, punto de equilibrio.
- "Marzo-2023" (real 16/02/2023): Metraje de viga chica muy densa, cronograma económico vs. financiero armado desde cero (anticipo+90días+convenio colectivo+30días), línea de crédito, 2 alternativas de remuneración de saldos.
- Febrero-2023 (real 26/01/2023): Metraje de 4 vigas de fundación (doble familia de armado en las 2 mayores), VNA 3 alternativas + ajuste de pago para VNA exacto, garantías (solo fiel cumplimiento+buena ejecución).
- Diciembre-2022: Movimiento de suelos por secciones transversales con peralte, extensión de plazo 12→18 meses (beneficio del contratista aumenta), fórmula paramétrica con ejemplo completo de reparto.
- Julio-2022: Metraje de losa "cruz" DECODIFICADA (clave usada luego en Feb-2024), dosificación completa, movimiento de suelos con costeo de 8 tareas (platea circular), garantías (Monto Imponible a estimar, 80%).
- "Marzo-2022" (real 15/02/2022): Metraje de losa+viga separados, costo de componentes de hormigón (variante de dosificación en $), reducción de plazo (caso espejo de Dic-2022, el beneficio del contratista aumenta), VNA/TIR con interpolación lineal entre dos tasas.
- Febrero-2022 (real 26/01/2022): Metraje de viga T-invertida asimétrica con 3 perfiles de estribo distintos, garantías (Fiel Cumplimiento+Buena Ejecución, Monto Imponible a estimar 80%/75,8% LLSS — mismo patrón que Jul-2022), teórico de VNA/TIR (por qué obra usa margen y no TIR), suministros, fórmula paramétrica.

**Pendiente para próximas corridas:** metraje de losas con planilla de armado en "cruz" (notación Φ/paso sin legend clara — visto en Ene-2026, Dic-2024, Jul-2024 y Feb-2024; en Feb-2024 se logró decodificar el paso de 2 de las 3 familias comparando contra la solución oficial, sigue faltando cerrar el 3er número; cuando el examen trae la planilla de cálculo ya resuelta, no bloquea la resolución), más variantes de metraje (tanques, escaleras, zapatas aisladas) a medida que aparezcan en exámenes más viejos.
