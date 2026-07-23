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

**Armaduras — criterios generales:** se metra por diámetro; se agrupa por nivel y tipo de elemento; empalmes 50Φ como norma; no se descuentan recubrimientos; usar siempre la misma planilla tipo (columnas: Horm. m³ | Encof. m² | Hierro kg | kg por cada diámetro con su % desperdicio). Desperdicios típicos por diámetro (pueden variar según el enunciado, siempre usar la tabla que da el examen): Φ6-Φ8 → 5%; Φ10-Φ12 → 10%; Φ16-Φ20 → 15%; Φ25+ → 15-20%.

**Variante "muro de contención con bloque vibrado"** (visto en Dic-2025): el muro se separa en: hormigón de limpieza (bajo la zapata), zapata/pie de muro, bloques vibro-prensados (con % de sección hueca a rellenar con hormigón — ej. 45% de un bloque 19x19x39), viga de coronamiento. La cantidad de bloques = bloques/m² (dato) × área de muro sin vigas. El volumen de hormigón interior a bloques = cantidad de bloques × %hueco × volumen bruto del bloque. El tenor de encofrado solo se calcula sobre zapata+viga (los bloques no se encofran). Ver `Soluciones/202512 Ex Diciembre 2025/`.

**Mini-ejemplo (pilar 0,6×0,6×0,15 con 1Φ16 por pilar, 4 pilares iguales):**
Vol = 0,6×0,6×0,15×4 = 0,216 m³. Encof (lateral, 4 caras) = perímetro×altura×4 = (0,6×4)×0,15×4 = 1,44... (ajustar según criterio de la pieza). Hierro: long=0,6m×4pilares=2,4m sin desperdicio → con 15% desp. → 2,76m × 1,58kg/m = 4,36 kg (orden de magnitud, ver planilla tipo completa en Clase 3 p.119 para el desglose fila a fila).

**Variante "pilar de piso intermedio con espera de empalme"** (visto en Jul-2025): si el pilar está en un piso intermedio de un edificio de varios niveles, la longitud de cada barra debe incluir la **espera para empalmar con el nivel siguiente** (normalmente 50Φ), además del gancho si corresponde en la base. Un pilar de sección muy delgada (ej. 12cm de espesor) da un **tenor de encofrado más alto de lo típico** — no es un error, es esperable porque la relación superficie/volumen crece cuando una dimensión de la sección es chica; hay que decirlo explícitamente si el examen pregunta "¿es esperable el resultado?". Ver desarrollo completo en `Soluciones/202507 Ex Julio/`.

**Variante "losa continua de varios paños, doble capa de armado"** (visto en Marzo-2025): cuando el plano muestra **dos capas de armadura** — una de "fondo" (F, positiva, recorre todo el vano en ambas direcciones) y una "de arriba" (A, negativa, refuerzo corto solo sobre los apoyos) — la capa negativa suele estar **duplicada** (una franja junto a cada uno de los dos apoyos de la losa), lo que se ve en la planilla como el doble de barras de lo que daría `ceil(tramo/paso)+1` para una sola franja. Esto es normal en losas continuas con momento negativo importante y produce una **cuantía de acero más alta que en una losa de un solo paño simplemente apoyada** (aquí 167 kg/m³ contra un rango típico de 80-120 kg/m³) — no es error, hay que justificarlo por la doble capa. Para leer las cotas del vano libre en plantas con dimensiones acumuladas ("cotas corridas"): el vano libre entre ejes de viga = diferencia entre la cota mayor y la cota menor de la línea de cotas paralela a esa dirección (ej. 8,53−0,43=8,10 m). Ver desarrollo completo en `Soluciones/202503 Ex Marzo/`.

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
1. Calcular la base sobre la que se aplica cada garantía: Precio con IVA y LLSS incluidos (Fiel Cumplimiento, Buena Ejecución) o Precio sin IVA/LLSS (Anticipo, si así lo indica el enunciado). Para el Monto Imponible de M.O., si no está dado, estimarlo como % del costo (dato u orden de magnitud ~30%) y aplicar el coeficiente de leyes sociales (~75,8% obra de arquitectura).
2. Para cada garantía, identificar la **forma en el tiempo** (constante, rampa creciente, rampa decreciente) entre los hitos: Inicio (I), Recepción Provisoria (RP), Recepción Definitiva (RD).
   - Fiel Cumplimiento: monto fijo (% del precio) desde la firma hasta RP.
   - Buena Ejecución: crece linealmente de 0 a su monto máximo entre I y RP (se retiene % de cada certificado, certificación uniforme ⇒ rampa lineal), luego se mantiene constante entre RP y RD (plazo de garantía adicional).
   - Anticipo: monto máximo al inicio, decrece linealmente a 0 durante el plazo de ejecución (se devuelve en cada certificado).
3. Costo de la garantía = **monto medio a garantizar en cada tramo** × tasa anual de la póliza × (meses del tramo/12).
4. Sumar todos los tramos de todas las garantías → costo total de garantías.
5. Comparar el costo total contra el costo/precio de la obra (%) — valores del orden de 0,5%-1,5% se consideran razonables (coherente con las primas de 0,4%-3% vistas en la Clase de Garantías y Seguros).

**Mini-ejemplo:** ver desarrollo numérico completo (Fiel Cumplimiento $1.163.885,88 + Buena Ejecución $989.303,00 + Anticipo $617.647,06 = $2.770.835,94, el 0,99% del costo de obra) en `Soluciones/202512 Ex Diciembre 2025/`.

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

---

## 12. Costo Financiero — Valor Neto Actualizado (VNA)

**Cuándo aparece:** Parte "Costo Financiero", 15-20 pts. Suele incluir una pregunta teórica (definir VNA) y un caso de comparar alternativas de pago/cobro en el tiempo.

- **VNA**: suma de los valores presentes de todos los ingresos y egresos de un flujo, descontados a una tasa de interés/descuento dada. `VNA = Σ Flujo_t / (1+i)^t`.
- Si VNA=0 a la tasa usada, esa tasa ES la TIR del proyecto. Si VNA>0, la inversión rinde más que la tasa de descuento (TIR mayor a la tasa). Si VNA<0, rinde menos (TIR menor).
- **Comparar alternativas de cobro/pago**: traer cada flujo a valor presente con la tasa dada (ej. 20% trimestral) y comparar. La de mayor VNA es la más conveniente para quien cobra (ej. la empresa constructora que recibe pagos).
- **¿La indemnización compensa el costo del dinero?** Comparar el VNA de la alternativa contra el monto original de la deuda/obligación: si VNA resultante > monto original, la alternativa compensa (y supera) el costo financiero de esperar el cobro; si es menor, no lo compensa.

**Mini-ejemplo:** deuda $1.000.000, tasa trimestral 20%, alternativa que paga 350+350+350+300+300 (miles $) al final de cada uno de 5 trimestres → VNA = 1.002,5 (miles $) > 1.000 → SÍ compensa el costo del dinero.

---

## 13. Movimiento de suelos (viajes de camión)

**Cuándo aparece:** Parte "Movimiento de Suelos", 10 pts. Dan un corte de terreno con capas (capa vegetal a desechar, capas de suelo natural a excavar, capas de aporte a rellenar/compactar) y piden cantidad de viajes de camión (capacidad dada) para cada material.

**Paso a paso:**
1. Para cada capa: Volumen "en banco"/compactado = espesor × área.
2. **Material que se retira** (capa vegetal, suelo natural excavado): pasar a volumen SUELTO usando el coeficiente de **esponjamiento (Ce)**: Vol. suelto = Vol. en banco × Ce (el material esponja al ser removido, por eso ocupa más en el camión).
3. **Material de aporte que se trae y compacta** (ej. balasto para sub-base): el volumen pedido en el enunciado suele ser el volumen ya **compactado** requerido; para saber cuánto material SUELTO hay que transportar, usar el coeficiente de **aporte (Ca)**: Vol. suelto a transportar = Vol. compactado requerido / Ca.
4. Viajes = Vol. suelto / capacidad del camión, **redondeado hacia arriba**.
5. Si el enunciado es ambiguo sobre cuánto suelo natural se retira (ej. "el material de aporte reemplaza a la arcilla" sin precisar si toda la arcilla o solo el espesor que ocupará el aporte), presentar **las dos opciones razonables** y aclarar el supuesto de cada una — no hay una única respuesta "correcta" si el dato es ambiguo.

**Mini-ejemplo:** platea 40×25m=1.000 m²; balasto compactado necesario 30 cm → Vol. compactado=300 m³; Ca=0,9 → Vol. suelto=300/0,9=333,3 m³; camión de 10m³ → 34 viajes (redondeado hacia arriba).

---

## 14. Suministros

**Cuándo aparece:** preguntas teóricas cortas, 10 pts.

- **Identificados**: especificaciones técnicas claras (normas/memorias), incumplimientos explicitados y valorados, proveedores potenciales, ensayos exigibles, lugar de entrega (flete/carga/descarga), necesidad de contrato.
- **Cuantificados**: unidad de medida clara, criterio de desperdicio, cantidad total y plazo de entrega.
- **Valorados**: precio unitario acorde a la unidad definida, con cotización vigente.
- **INCOTERMS**: términos de compraventa internacional que fijan obligaciones/riesgos entre exportador e importador (EXW, FOB, CIF, CFR, FCA, DAP, DDP, etc.).

---

## Exámenes ya incorporados a esta guía
- Ene-2026: Costo de equipos (retroexcavadora), teoría de mano de obra/licitaciones/garantías.
- Dic-2025: Metraje muro de contención con bloques, consumos+dosificación de hormigón, fórmula paramétrica, costo horario de obrero, garantías con perfil temporal, suministros/INCOTERMS.
- Jul-2025: Metraje de pilar con espera de empalme, dosificación de hormigón (método detallado para sacar la relación volumétrica agua/cemento), costo financiero/VNA, movimiento de suelos (viajes de camión), TOCAF/tipos de contrato, consumo unitario vs. rendimiento, Convenio Colectivo/Fondos Sociales.
- Marzo-2025: Metraje de losa continua con doble capa de armado (fondo + refuerzo negativo duplicado sobre apoyos), dosificación de hormigón, fórmula paramétrica (criterio para Gastos Indirectos+Beneficio), punto de equilibrio (caso "conviene el cambio"), VNA/TIR (obra vs. inversión), suministros.

**Pendiente para próximas corridas:** metraje de losas con planilla de armado en "cruz" (notación Φ/paso sin legend clara — ver examen Ene-2026 parte I), más variantes de metraje (tanques, escaleras, zapatas aisladas) a medida que aparezcan en exámenes más viejos.
