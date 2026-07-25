# Resumen Teórico — Costos (ingeniería de costos de obra)

## Índice de temas por frecuencia en exámenes (recalculado sobre los 24 exámenes 2019-2026, cobertura completa)

**Metodología:** conteo por búsqueda de palabras clave sobre los 24 `Soluciones/<examen>/RESOLUCION.md`, verificado a mano en los casos ambiguos (ej. "Metraje" de Dic-2022 es en realidad movimiento de suelos, no hormigón — se contó en la categoría correcta). Ordenado de mayor a menor frecuencia: **estudiar primero lo de arriba**.

| Tema | Frecuencia | Sección de la Guía |
|---|---|---|
| Metraje de hormigón armado (losas/vigas/muros/pilares/zapatas) | **23/24** | Guía §1 |
| Costo Financiero — VNA/TIR | **20/24** | Guía §12 |
| Mano de obra / Ley 14.411 / Convenio Colectivo / Leyes Sociales | **20/24** | Guía §5-6 |
| Garantías (con o sin perfil temporal) | **17/24** | Guía §7 |
| Consumos unitarios de hormigón armado | **15/24** | Guía §2 |
| Fórmulas paramétricas | **12/24** | Guía §8 |
| Suministros / Subcontratos / INCOTERMS | **10/24** | Guía §14 |
| Seguros de obra (TRC, RC, Ley 16.074) | **10/24** | Guía §10 |
| Dosificación de hormigón (agregados+cemento+agua) | **8/24** | Guía §3 |
| Costo horario de equipos | **8/24** | Guía §4 |
| Movimiento de suelos (Ce/Cc/Ca, viajes de camión) | **8/24** | Guía §13 |
| Punto de Equilibrio / costos fijos-variables | **8/24** | Guía §11 |
| Clasificación de costos por naturaleza | **7/24** | Guía §15 |
| Costo horario de mano de obra (jornalero/obrero) | **5/24** | Guía §5 |
| Licitaciones (TOCAF, tipos de contrato) | **4/24** | Guía §9 |
| Consumo de mampostería y revoques | **2/24** | Guía §16 |

*(Un examen puede aportar a varios temas a la vez — ej. Metraje + Consumos + Dosificación suelen ir juntos en la Parte I-II. La tabla se recalcula cuando se detecten inconsistencias o se sumen exámenes nuevos al repo.)*

---

## 1. Metrajes de hormigones y albañilería (Clase 3, Clase 4 y Clase 7)

**Concepto:** cuantificar para cada estructura (clasificada por tipo — pilares, vigas, losas... — y por nivel — PB, 1er piso...) el volumen de hormigón (m³), el tenor de encofrado (m²/m³) y la cuantía de acero (kg/m³). Existen varios criterios válidos: lo importante es ser coherente.

**Criterios de volumen** (ver tabla completa en la Guía de Ejercicios Tipo, sección 1): hormigón ciclópeo=volumen neto; zapatas=volumen neto+tronco de pirámide; pilares de fundación=sección×(zapata→viga); pilares=sección×(losa→losa); vigas=sección×longitud entre pilares; losas=espesor×superficie entre vigas; tanques=exterior−interior; escaleras=sección del escalón×longitud.

**Armaduras:** se metra por diámetro, agrupado por nivel y elemento. Empalmes: 50Φ. No se descuentan recubrimientos. Desperdicios crecientes con el diámetro (Φ6-8: 5%; Φ10-12: 10%; Φ16-20: 15%; Φ25+: 15-20%, aprox. — usar siempre la tabla del examen).

**Errores comunes a evitar** (de "Aclaraciones sobre errores comunes de la parte práctica"):
- En losas, el volumen es el contenido **entre vigas** (las vigas no son parte de la losa).
- Cantidad de hierro = redondear.hacia arriba(tramo/paso)+1; *paso*=separación entre armaduras, *tramo*=ancho del espacio donde se colocan (no la longitud). En losas, el tramo no incluye la viga.
- Encofrado de losa: solo cara inferior fuera de vigas (si un lateral no tiene viga, se encofra ese lateral). El hormigón común no suele necesitar encofrar caras superiores (viscosidad alta).
- Vigas/losas suspendidas → encofrado inferior salvo indicación contraria. Zapatas/muros de contención → apoyan en el suelo, no se encofra la cara inferior.
- Tenor = área encofrado/volumen hormigón; Cuantía = kg hierro/volumen hormigón. Conocer rangos esperables por tipo de pieza para detectar errores — un valor fuera de rango no es automáticamente un error, puede haber una justificación (ej. losa apoyada en el suelo → tenor mucho menor).
- Consumos por m³: no hace falta el total de material, con tenor/cuantía se llega directo. Mano de obra (hs/m³) = 1×(hs/m³ pasta) + tenor×(hs/m² encofrado) + cuantía×(hs/kg hierro). Hormigón (m³/m³)=1×(1+%desp). Hierro (kg/m³)=cuantía. Tabla de pino/chapón (unid/m³) = (tenor×(1+%desp))/(área_unitaria×reúsos).

**Fórmula general de acero (Clase 4):** `kg = Cantidad×(Longitud+Empalmes+Ganchos)×Densidad×(1+%Desperdicio)`, con `Cantidad = redondear.hacia arriba(tramo/paso)+1`.

**Valores de referencia de Tenor y Cuantía por tipo de elemento (Clase 4 — útiles para detectar un resultado fuera de rango):**

| Elemento | Tenor (m²/m³) | Cuantía (kg/m³) |
|---|---|---|
| Pilares | 10-14 | 100-180 |
| Vigas | 8-12 | 70-150 |
| Losas | 5-10 | 60-80 |

*(Un muro de contención macizo da valores bastante más bajos que estos rangos —ver Guía sección 1, variantes de Feb-2025/Jul-2023— por tener menos superficie de encofrado y menos densidad de armado relativa a su volumen; no es un error, es coherente con la geometría del elemento.)*

**¡Importante! Discrepancia detectada entre el material de Clase 4 (2026) y la planilla oficial de un examen real:** la Clase 4 usa el muro de contención de **Marzo-2020** como ejemplo resuelto en diapositivas, pero llega a un encofrado (117 m², Tenor 4,6) y una cuantía de acero (2.239,2 kg, 88,9 kg/m³) **distintos** a los de la planilla oficial que calificó ese examen real (126 m², Tenor 5,0; 2.177,28 kg, 86,4 kg/m³) — la diferencia está en si la pata del muro se encofra con 1 o 2 caras, y en el desarrollo exacto de la longitud de la barra "horquilla". Ver el detalle completo de ambos cálculos en `Soluciones/202003 Ex Marzo/RESOLUCION.md` y en la Guía de Ejercicios Tipo, sección 1 — ante esta ambigüedad, priorizar el criterio de la Clase 4 (más reciente) salvo que el examen aclare lo contrario.

**Ejemplos que la Clase 4 usa/referencia como casos resueltos:** Marzo 2020 (visto arriba), Julio 2025 (ya resuelto en `Soluciones/`), y **Febrero 2026 / Marzo 2026** — estos 2 últimos NO están todavía en la carpeta `Exámenes/` del repo (son exámenes futuros de este mismo año lectivo, mencionados en la diapositiva como referencia pero sin PDF disponible aún) — revisar si aparecen en corridas futuras.

**Albañilería (Clase 7):** se clasifica por tipo de muro (simple/doble, de ticholo/rejillón, tipo de terminación). **Criterio de descuento de aberturas** en la superficie de un muro: aberturas **menores a 2 m² NO se descuentan**; entre **2 y 4 m² se descuenta el 50%** del área; mayores a 4 m² se descuentan completas (criterio inferido, coherente con no restar áreas cuando la dificultad constructiva no lo justifica). Ver también el ejemplo completo de planilla de metraje de muros con revoques/pinturas del Trabajo Práctico 2020 en la diapositiva 149 de la Clase 7.

**Dosificación de hormigones y morteros (Clase 7 — complementa Guía sección 3):** los coeficientes de aporte son promedios estadísticos, válidos con material de humedad baja/normal; por practicidad se dosifica en **volumen**, no en peso. El agua se dosifica distinto según el material: en **hormigones**, por relación agua(lt)/cemento(kg); en **morteros**, como **% sobre el volumen aparente de los demás componentes** (ej. 15%). Los resultados finales se expresan en unidades comerciales: áridos en m³ aparentes, cemento en kg o bolsas de 25kg, cal en kg. Ver la tabla de referencia de Coeficiente de Aporte y Peso Específico por material (canto rodado, pedregullo, piedra partida/bruta, arena gruesa/fina, cemento, cal, agua) en la Guía de Ejercicios Tipo, sección 3.

---

## 2. Costo de equipos (Equipos.pdf)

**Por qué se presupuesta como si fuera un alquiler:** aunque el equipo sea propio, se le debe asignar una tarifa horaria que cubra comprar, usar, mantener y reponer el equipo.

**Componentes del costo horario (todos referidos a horas de uso):**
- **Amortización/Depreciación** = (VN−VR)/VU, con VU=vida útil en horas (n años × horas/año). Hipótesis: depreciación lineal.
- **Reparaciones** = α (tabulado por equipo, ej. 40% para retroexcavadora CASE 580) × Amortización.
- **Combustible** = consumo (lt/h) × precio ($/lt); depende del equipo (retroexcavadora combinada ≈6 lt/h, CAT215 ≈20 lt/h, motoniveladora ≈14 lt/h, D6≈20, D7≈32 lt/h).
- **Lubricantes** = β (tabulado) × costo de Combustible, o bien directamente por consumo×precio si se dan los insumos (aceite, grasa, filtro) por separado.
- **Tren de Rodado (TR)** = VI_TR / VU_TR (mismo criterio que amortización pero para orugas/neumáticos, que tienen vida útil propia mucho más corta).
- **Maquinista (mano de obra)** = Salario mensual / horas trabajadas por mes del equipo. Se paga el mes completo aunque el equipo no trabaje todas las horas (viajes, lluvia, sin obra) — por eso se prorratea sobre las horas de uso reales, no sobre las teóricas.
- **Seguro** = 2% anual del valor inicial (VN) / horas trabajadas por año.
- **Patente** = equivalente al seguro (solo pagan patente los equipos que se trasladan por vía pública por sus propios medios; los de orugas se transportan en chatas y no pagan).
- **Costo Financiero** = [(VN−VR)/2 × tasa anual activa] / horas trabajadas por año (interés sobre el capital medio inmovilizado en el equipo).
- **Costo Total** = suma de todos los anteriores. A **menor cantidad de horas de uso al mes/año, mayor el costo horario** (los costos fijos se reparten entre menos horas) — de ahí que para usos esporádicos convenga alquilar en vez de comprar el equipo.

**Leyes sociales sobre la mano de obra del equipo:** Monto Imponible = u% del jornal (≈80%); LLSS = K% (≈70-76%) del Monto Imponible — mismo mecanismo que en mano de obra general (Ley 14.411).

**Movimiento de suelos con equipos:** para dimensionar la cantidad de camiones necesarios para que una máquina nunca quede sin camiones: tiempo de ciclo del camión = ida cargado + descarga + vuelta vacío; viajes/jornada = (horas de jornada×60)/tiempo de ciclo; capacidad de transporte por camión = viajes×capacidad; camiones necesarios = producción de la máquina (m³/jornada) / capacidad de transporte por camión.

---

## 3. Mano de obra (Clase 9 — Ley 14.411 y Convenio Colectivo)

**Regulación:** la Construcción es el Grupo 9 de la clasificación de Actividad Nacional. El sistema de contratación (remuneración, laudos, viáticos, licencia, incentivos, aumentos, aportes sociales) está regulado principalmente por la **Ley 14.411**, complementada por un **Convenio Colectivo tripartito** (Empresas, Trabajadores -SUNCA-, MTSS/Poder Ejecutivo que homologa), renovado cada 3 años, con ajustes ligados a metas de inflación del BCU.

**Formas de retribuir:**
- **Por tiempo trabajado**: mensuales (encargados/capataces) o jornaleros (44hs/semana: lunes-jueves 9hs, viernes 8hs), según Laudo vigente (valor de "hora común" por categoría).
- **Por producción ("destajo")**: valor por unidad de obra ejecutada; poco usado en presupuestación convencional, requiere control exhaustivo.

**Ítems que se pagan al jornalero** (ver detalle y %/fórmulas en la Guía de Ejercicios Tipo, sección 5): hora común; ropa/transporte/herramientas (sobre Cat. V); presentismo semanal (10,42%) y mensual (5%); media hora de descanso; incentivos por producción; horas extra (+100%); feriados (7 no laborables/año); horas de lluvia/barro/crecidas (topeadas por cuatrimestre, con reglas de traspaso entre cuatrimestres); tickets de alimentación ($200 cada 8hs); vestimenta (ropa de invierno 1/abril, verano 1/octubre, campera bianual); suplemento por altura (10% jornal Cat. V c/8hs, >6m; Cat. VII en montaje electromecánico); suplemento por acarreo en plataformas voladas (30%); horas nocturnas (20 a 6hs, +30% esporádico / +50% permanente).

**Viáticos por distancia:** monto=50% del jornal Cat. V (=100% del viático). Composición: 40% alimentación (descontable si la empresa brinda el servicio) + 40% locomoción/vivienda (descontable) + 20% no descontable. Personal no permanente: sin viático hasta 5km del área urbana más próxima; 60% del viático entre 5-25km; 100% a más de 25km.

**Aporte Unificado de la Construcción (Ley 14.411):**
`TOTAL A PAGAR = [Precio Obra + IVA] + [Monto Imponible de M.O.] × Coeficiente de Aporte Unificado según tipo de obra`.
- Monto Imponible ≈ 80% del salario del operario.
- Leyes Sociales ≈ 71,8% del MI (obra pública/ingeniería) o 75,8% (obra de arquitectura) — la diferencia es el CJPPU (2% ingeniería, 4% arquitectura, Ley 17.738).
- Partidas gravadas totalmente: hora común, presentismo semanal/mensual, horas extra, feriados no laborables, nocturnidad, horas en altura. No gravadas: ropa, herramientas, transporte, media hora descanso, pasajes, horas de lluvia, tickets. Parcialmente gravadas (sobre-laudo, viático, incentivo por producción): si b<30% de RT no se grava; si b>30% de RT se grava el 50% del excedente.

**4 Fondos Sociales de la Construcción:**
1. **FOSVOC** — vivienda de obreros (compra/construcción/reforma).
2. **Fondo Social de la Construcción (FSC)** — canastas familiares, útiles escolares, odontología, cursos, capacitación.
3. **FOCAP** — capacitación técnica ocupacional (soldadura, maquinaria, etc.).
4. **FOCER** — cuentas individuales de cesantía y retiro (aportes patronales+personales, disponible en su totalidad para el trabajador).
Aportes patronales de referencia: FSC/FOCAP 1,2691%, FOSVOC 0,025%, FOCER 5,00% (obrero no permanente) o 0,50% (permanente).

---

## 4. Características de la industria de la construcción y licitaciones (Clase 2)

**Características históricas:** régimen laboral especial (convenio tripartito); alta incidencia de mano de obra no calificada; alta rotación (solo ~20% de los obreros son permanentes de una empresa entre obra y obra).

**Obra pública:** contratación por licitaciones abiertas; baja planificación a largo plazo (depende del ciclo político); regida por el **TOCAF** (Texto Ordenado de Contabilidad y Administración Financiera), que fija los montos límite y procedimientos de compra estatal (ver tabla en Guía de Ejercicios Tipo sección 9). Excepciones a Licitación Pública sin importar el monto: compras entre organismos estatales, procedimiento desierto, proveedor único, reparación de maquinaria no trasladable, urgencia. Publicación en ARCE, control del Tribunal de Cuentas. Otras reglas TOCAF: depósito de dinero público en BROU (Art.5), gasto solo para lo presupuestado (Art.16), ejecución dentro del año fiscal (Art.13).

**Obra privada:** contratación por licitaciones cerradas (información reservada); alta sensibilidad a la economía; dependencia de inversión extranjera (ej. Punta del Este/Argentina).

**Tipos de contrato según el presupuesto solicitado:**
- **Precio Global**: precio fijo total. Ventaja: certeza de costo para el cliente, transfiere riesgo de sobrecosto al contratista. Desventaja: poca flexibilidad, márgenes de seguridad en el precio.
- **Precio Unitario**: precio por partida, se paga según cantidad ejecutada. Ventaja: flexible ante variaciones de cantidad. Desventaja: incertidumbre del costo final, requiere control riguroso de mediciones.
- **Por Administración**: costos reales + % o suma fija de gestión. Ventaja: se puede iniciar sin definir todo el alcance, transparencia. Desventaja: requiere control detallado, poco incentivo a bajar costos si no hay tope.

---

## 5. Riesgos, Garantías y Seguros (Clase 19)

**Riesgo** = todo evento posible que, de ocurrir, es perjudicial; tiene una probabilidad y una valoración/costo asociados. `RIESGO = VALORACIÓN × PROBABILIDAD`. Gestión del riesgo: identificación preliminar → valoración y cuantificación → tratamiento y mitigación → valoración final o residual (Riesgo Máximo + Plan de Acción de Riesgos).

**Garantías contractuales requeridas por el Contratante (7, Clase 19):** Mantenimiento de Oferta, Fiel Cumplimiento de Contrato, Fondo de Reparo (Buena Ejecución), Sustitución de Fondo de Reparo, Anticipo o Acopio, **Ley de Tercerizaciones**, otras. (Detalle de monto/plazo/objetivo de cada una en la Guía de Ejercicios Tipo, sección 7). ⚠️ La Clase 19 SÍ trata la Ley de Tercerizaciones como una garantía contractual más (misma ficha Oportunidad/Monto/Plazo/Costo que las demás: garantía fraccionada por certificado, ~5% c/u, costo ~2% anual) — el motivo de fondo es que la ley le da al contratante **responsabilidad solidaria/subsidiaria** por las obligaciones laborales de los subcontratistas del contratista, y esta garantía es la forma de cubrir ese riesgo. Formas de constitución: garantía bancaria, carta de crédito irrevocable, póliza de seguro de fianza (BSE), bonos del tesoro en U$D, depósito.

**Componentes de un Seguro:** objeto asegurado, valor del objeto, riesgos/eventos cubiertos, monto máximo de indemnización, prima (costo), deducible, plazo de vigencia, deberes del contratante, exclusiones.

**Seguros de obra:**
1. **Accidentes de Trabajo** (Ley 16.074, obligatorio, monopolio BSE): personal obrero Ley 14.411 → incluido en el aporte unificado; técnico → 2% de su salario; administrativo → 0,6%.
2. **Vehículos y maquinaria**: cubre daños propios y a terceros; ~2% del valor del equipo/año; suele venir en el alquiler pero hay que verificarlo.
3. **Todo Riesgo de Construcción (TRC)**: cubre derrumbe, incendio, inundación, accidentes sobre la obra/propiedad adyacente; obras comunes 0,3%-0,5% del monto del contrato (más en obras marítimas/portuarias).
4. **Responsabilidad Civil (RC)**: daños a terceros por la actividad del contratista; ~0,3% anual sobre el contrato (a veces ya incluido, limitado, dentro del TRC).
5. Otros: diseño, cumplimiento de plazos, cumplimiento de demanda.

---

## 6. Programa Económico y Financiero de una Obra (Clase 20)

**Estado Económico** = `Ventas − Costos = Utilidad`. Mide la **rentabilidad** del negocio en su conjunto,
sin importar cuándo ocurren los cobros/pagos. Objetivo: **economicidad/viabilidad económica** (utilidad
positiva) — el punto de equilibrio solo no alcanza, hace falta ver el margen/beneficio real.

**Estado Financiero** = `Ingresos − Egresos = Disponibilidad`. Mide si hay **caja suficiente en todo
momento** durante la obra (estudio del flujo de dinero en el tiempo). Objetivo: **viabilidad
financiera/equilibrio financiero**. De acá surge el **Costo Financiero**: interés sobre el capital que la
empresa debe adelantar mientras espera cobrar (por el desfasaje entre cuándo paga insumos/mano de
obra y cuándo cobra los certificados).

**Cómo se arma el ejemplo tipo (ver mini-ejemplo numérico completo en `Soluciones/202502 Ex
Febrero/`):**
1. Resumen de insumos (Mano de Obra, Equipos, Materiales, Suministros y Subcontratos, Varios) con
   su costo total e incidencia %, más Costo Indirecto y Beneficio (%s/venta) → Venta Total (pasaje de
   costo a venta = 1/(1−%beneficio)).
2. Cronograma físico de avance por rubro y por mes (% de avance de cada rubro en cada mes, suma
   100% por rubro) → Previsión de Costos por mes (costo total del rubro × % de avance de ese mes) y
   Previsión de Ventas Mensuales (venta total del rubro × % de avance) → **Estado Económico Mensual**
   (Utilidad = Venta−Costo de cada mes, y su acumulado, que converge al beneficio total).
3. **Flujo de Fondos Mensual**: cada insumo se cobra/paga con su propio desfasaje (ej. Mano de Obra
   50% en el mes, 50% al mes siguiente; Equipos y Materiales a 30 días; Suministros a 60 días;
   Ingresos de venta a 60 días) → Flujo de Fondos sin Costo Financiero y su acumulado (puede dar
   negativo en los primeros meses → necesidad de financiación).
4. **Costo Financiero** = interés mensual (`i_mensual=(1+I_anual)^(1/12)-1`) aplicado sobre el saldo
   acumulado negativo de cada mes → se resta del flujo de fondos, dando el Beneficio real (algo menor
   al 15% "de catálogo", en el ejemplo del curso 15,00%→14,46%). También se puede calcular
   actualizando todo el flujo a valor presente: `Margen = VNA(Cobros−Pagos)/VNA(Cobros)`.
5. **Un anticipo del cliente al inicio de la obra reduce fuertemente la necesidad de financiación** (en el
   ejemplo del curso, con 20% de anticipo el costo financiero baja de 0,54% a 0,03% de la venta) —
   acerca la obra a la "autofinanciación".

**Elaboración y comparación de ofertas** (Clase 20, segunda mitad — teórico corto, puede aparecer
como pregunta suelta):
- Proceso: Oportunidades → Selección → Viabilidad Económica/Contractual/Técnica → Oferta → Contrato.
- **Precalificación** (obra pública/grandes obras): etapa previa donde se evalúa capacidad técnica,
  económica-financiera y legal de las empresas interesadas, para admitir solo a las habilitadas a ofertar.
- Contenido de una oferta: carta de presentación, memoria, cumplimiento del pliego, propuesta
  económica, resumen ejecutivo, documentación complementaria.
- **Criterios de comparación de ofertas** (deben fijarse ANTES de abrir las ofertas y no modificarse
  después): precio, plazo de ejecución, flujo financiero (VNA de los pagos), proyecto (si está a cargo
  del oferente), personal y equipos, calidad de materiales, rendimientos, antecedentes/capacidad de
  la empresa. Mejor no considerar un criterio que considerarlo mal; en licitación pública, las
  aclaraciones solicitadas a un oferente no pueden usarse para que modifique/ajuste su oferta.

---

## 7. Movimiento de suelos (Clase 6)

**Metraje de excavaciones "a mano" (pico y pala):** para pozos y zanjas puntuales (ej. terreno natural por encima del nivel de fundación de cabezales/vigas — se procura evitar por encarecer la obra). Volumen = volumen del elemento a fundar, ajustado por la estabilidad de la excavación y el área mínima de trabajo necesaria (ver tabla de áreas mínimas por profundidad en la Guía sección 13).

**Excavaciones generales "a máquina":** (1) identificar la cota del terreno natural (curvas de nivel/progresivas, **después de retirar la capa vegetal**); (2) identificar la cota de excavación de proyecto (cota de piso terminado/pavimento menos los espesores de capas intermedias — contrapiso, base, etc.); (3) subdividir el terreno en zonas de igual "cota objetivo" (la cota inferior de la base a colocar); (4) dentro de cada zona, ver dónde el terreno limpio queda por encima (desmonte) o por debajo (terraplén) de la cota objetivo, marcando puntos clave y calculando el volumen por secciones transversales (ver método completo con interpolación en Guía sección 13, variante Dic-2022).

**Los 3 coeficientes formales, en cadena Vb→Vs→Vc** (Vb=volumen en banco/sitio, sin remover; Vs=volumen suelto, sobre camión o acopiado; Vc=volumen compactado, en el terraplén final): **Esponjamiento Ce=Vs/Vb** (siempre >1). **Compactación Cc=Vc/Vs** (siempre <1). **Aporte Ca=Vb/Vc=1/(Ce×Cc)** (cuántos m³ en banco hacen falta por cada m³ compactado final). Ver la tabla de valores de referencia por tipo de suelo (Arena/Tierra Común/Arcilla/Piedra) y la advertencia sobre convenciones alternativas usadas en distintos exámenes en la Guía de Ejercicios Tipo, sección 13 — **importante:** varios exámenes reales usan una convención de 2 pasos (banco→compactado directo) con nombres que no siempre coinciden con esta cadena formal de 3 pasos; verificar siempre contra un resultado conocido o presentar el razonamiento explícito si la pregunta es teórica.

---

## 8. Clasificación de costos: Fijos/Variables, Directos/Indirectos, por Naturaleza (Clase 8)

**Costo Fijo:** independiente de que se ejecuten o no tareas, y del volumen de ejecución (ej. capataz, ingeniero, alquiler de oficina, UTE). **Costo Variable:** aumenta/disminuye en el mismo sentido que el volumen de tareas ejecutadas; si no se trabaja, no existe. **Relación práctica con Directo/Indirecto** (clasificación distinta, no siempre coincidente): mayoritariamente los Costos Directos son Variables y los Indirectos son Fijos, pero no es una regla absoluta — Directo/Indirecto depende de si el gasto se puede **imputar a una tarea** específica (y de qué tareas se listaron), mientras que Fijo/Variable depende de si **reacciona al volumen** de obra ejecutado. Ver tabla cruzada de ejemplos (mano de obra, equipos, materiales, varios) en la Guía sección 15.

**Punto de Equilibrio:** volumen de producción a partir del cual los ingresos (venta) superan el costo total (fijo+variable) — por debajo, pérdida; por encima, beneficio (ver desarrollo completo en Guía sección 11).

**Variante "ampliación/reducción del alcance de una obra" (apalancamiento operativo, 3ª forma):** cuando cambia la CANTIDAD de obra contratada (no el plazo ni un turno adicional), el Costo Variable escala proporcionalmente al cambio, el Costo Fijo NO cambia, y la Venta también escala proporcionalmente (mismos precios unitarios) — el margen mejora al ampliar y empeora al reducir, pudiendo llegar a pérdida. Ver el ejemplo numérico completo (ampliar 50%→margen 25,0%; reducir 50%→margen −8,3%, pérdida) en la Guía sección 11.

**Clasificación de Costos por Naturaleza, 8 grupos formales:** Mano de Obra, Equipos, Materiales, Suministros (+subcontratos), Varios (gastos generales de obra, garantías/seguros, fletes, proyectos), Gastos Generales (de oficina central), Imprevistos (análisis/valoración de riesgos, no siempre considerados en obras chicas), Costos Financieros. Ver el detalle completo con qué insumos integran cada grupo en la Guía sección 15.

---

## 9. Materiales, Suministros y Subcontratos — Costos por Naturaleza en detalle (Clase 12)

**Concepto:** profundiza los grupos "Materiales" y "Suministros/Subcontratos" de la clasificación por Naturaleza (ver sección 8) — qué información hay que relevar de cada insumo antes de poder presupuestarlo correctamente. Aplica a los 3: **identificar, cuantificar y valorar**.

**Materiales** (materias primas que se transforman en obra vía mano de obra/equipos — valor agregado):
- **Identificados**: especificaciones técnicas claras (normas/memorias del cliente), incumplimientos explicitados y valorados si los hay, proveedor(es) potencial(es), ensayos a exigir al proveedor, lugar de entrega (flete/carga/descarga incluidos o no), necesidad de contrato.
- **Cuantificados**: unidad de medida clara (ej. cemento por kg o bolsa; arena por m³ o bolsa), criterio de desperdicio, cantidad total y plazo de entrega.
- **Valorados**: condición de entrega (INCOTERM), forma/plazo de pago, plazo de validez de la oferta, garantía si corresponde, ajuste de precios (paramétrica); conviene discriminar del precio los costos asociados (flete, introducción, ensayos) y registrar el proveedor de referencia.

**INCOTERMS completos y consideraciones prácticas de precios (fuentes válidas, plazo estándar de 30 días):** ver tabla completa y detalle en la Guía de Ejercicios Tipo, sección 14.

**Suministros** (bienes con bajo valor agregado en obra) y **Subcontratos** (tareas de una especialidad a cargo de un tercero): mismos 3 pasos que Materiales pero con evaluación técnico-económica más rigurosa. El **contratista nunca se libera de responsabilidad** frente al cliente por lo que haga el subcontratista (control estricto, en especial en seguridad laboral — **Ley de Tercerizaciones**: responsabilidad solidaria laboral del contratista frente al trabajador subcontratado). Si el rubro subcontratado cae dentro de la **Ley 14.411**, la cotización del subcontratista debe incluir su propio Monto Imponible, para sumarlo al Monto Imponible total del presupuesto del contratista principal. Motivos usuales para subcontratar: falta de experiencia/especialidad propia, competitividad, limitación de recursos, reducción de riesgo.

---

## 10. Consumos unitarios, rendimientos y Costos Indirectos de obra (Clase 17)

**Consumo Unitario vs. Rendimiento:** el **Consumo Unitario** es la cantidad de un recurso que se usa para ejecutar una unidad de tarea (ej. 14 bolsas de cemento/m³ de hormigón — base de la Planilla de Consumos, ver sección 1 y Guía secciones 2-3). El **Rendimiento** es la cantidad de trabajo que ejecuta una unidad de recurso en un tiempo dado (ej. un oficial coloca 12 m²/día de muro; una retroexcavadora excava 45 m³/hora) — sirve para planificar tiempos/costos y comparar alternativas de ejecución.

**Consumo Estándar:** consumo de un insumo bajo condiciones de referencia fijas; el consumo real de una obra concreta se obtiene ajustando el estándar por los **desvíos** respecto de esas condiciones, con coeficientes multiplicadores:

| Factor de desvío | Condición Estándar (coef.=1) | Efecto de un desvío | Rango típico |
|---|---|---|---|
| Climático (ic) | Clima moderado sin lluvia, 5°C-38°C, viento <30km/h, altitud <1.500m | Siempre EMPEORA (temperaturas extremas, viento, altura) | >1 (1,1 / 1,2 / 1,3) |
| Horario (ih) | Horario diurno, horas extra acotadas | Siempre EMPEORA (trabajo nocturno a la intemperie, exceso de horas seguidas) | >1 |
| Emplazamiento (ie) | Suelo nivelado y seco, sin obstáculos, <150m desde el ingreso, sin restricciones de seguridad | Siempre EMPEORA (traslados largos, restricciones de seguridad) | >1 (1,2 / 1,3) |
| Personal — capacitación/incentivo (ip) | Personal capacitado, jornal por hora o a destajo, sin conflictividad | Puede MEJORAR o EMPEORAR (incentivos/premios, conflictividad, falta de capacitación) | 0,8 a 1,3 |
| Repetitividad/secuencialidad (ip) | Volumen de tarea continuo, sin "producción en serie" que distorsione | Puede MEJORAR o EMPEORAR (tareas muy discretas/aisladas, o repetición a gran escala) | 0,8 a 1,3 |

Antes de aplicar un coeficiente >1 sin más, conviene evaluar si se puede mejorar la condición real (acercarla al estándar) o ajustar el procedimiento constructivo.

**Costos Indirectos de Obra ("Costos Generales de Obra"):** no se pueden asignar a una tarea puntual pero hacen falta para el conjunto de la obra (analogía del curso: "un restaurante no puede servir sin luz, mozos ni un lugar limpio, aunque esos gastos no estén en cada plato"). Principalmente mano de obra de supervisión (Jefe de Obra, capataz, administrativos), equipos de traslado y "varios" (obrador, energía, baños químicos, herramientas compartidas, teléfono/internet). Mayormente intangibles y **Costos Fijos**. **Incidencia típica: 15%-25% del costo total** en obras civiles (menor cuanto mayor el peso de suministros/subcontratos, que traen su propio indirecto incorporado). **Concepto de "Afectación":** cuando un recurso indirecto no está 100% dedicado a la obra (ej. un Jefe de Obra a cargo de 2 obras), se le imputa solo el % de afectación correspondiente (ej. 50%) sobre su costo mensual total.

---

## 11. Ajuste de precios — fórmula paramétrica oficial (Clase 18)

*(Formaliza y complementa la Guía de Ejercicios Tipo, sección 8, con la fórmula y fuentes oficiales.)*

`P₁ = P₀ × (j×J₁/J₀ + m×M₁/M₀ + cv×CV₁/CV₀ + d×D₁/D₀)`, con `j+m+cv+d=1`. Subíndice "0"=mes anterior a la oferta; "1"=mes anterior al del ajuste (siempre con 1 mes de desfasaje).

| Índice | Qué mide | Fuente oficial |
|---|---|---|
| J | Mano de obra — Índice de traslado a precios, Grupo N°37 (Industria de la Construcción) | MTSS |
| M | Canasta de materiales | Boletín mensual Cámara de la Construcción (CCU) o MTOP |
| CV | Costo de vida / gastos generales | IPC — INE |
| D | Variación cambiaria | Dólar interbancario vendedor, último día hábil del mes — BCU |

**Canasta de Materiales (submodelo dentro de M, si se desagrega):** `M₁/M₀ = m₁×M₁₁/M₁₀ + m₂×M₂₁/M₂₀ + ... + mₙ×Mₙ₁/Mₙ₀`, con Σmᵢ=1 — misma lógica de ponderación que la fórmula general, aplicada a los materiales representativos del grupo/obra.

**Variante de alta inflación (infrecuente en el país):** cuando el plazo entre certificación/facturación/pago es largo con muy alta inflación, se agrega un factor de costo financiero: `P₁ = P₀×(j×J₁/J₀+...+d×D₁/D₀)×[(1+i₁)ᵗ/(1+i₀)ᵗ]`, con i₁/i₀=tasas de interés promedio de plaza (moneda nacional no reajustable) de los 3 meses previos al ajuste/oferta, y t=plazo de pago en años (año comercial=360 días).

---

## 12. Estudio Comparativo de Ofertas (Clase 21 — complementa Clase 20)

**Objetivo:** elegir la mejor oferta según los intereses del propietario, con procedimiento profesional (criterios alineados a los objetivos, etapas claras con o sin precalificación, criterios precisos, comparación coherente, profesionales con experiencia).

**Documentación a entregar a los oferentes (antes de presentar ofertas):** carta de invitación (fecha/hora de entrega, plazo de consultas), plazo/importe de garantía de mantenimiento de oferta, pliego de condiciones comerciales y técnicas, alcance de los trabajos, formulario de propuesta con Rubros **Globales** y **Unitarios** (con cantidad fija o a definir por el oferente), definición de cada tarea, moneda(s) de cotización y fórmula de ajuste de precios, plazos requeridos, forma de pago, proyecto de contrato (penalidades, garantías), criterios de comparación, y causales de rechazo.

**Qué debe incluir la oferta:** carta compromiso + garantía de mantenimiento de oferta, listado de apartamientos técnicos/comerciales respecto del pliego, apertura de precios (planilla de precios y cantidades), cronograma de ejecución, cronograma económico-financiero, especificación técnica y proveedores de suministros/materiales principales.

**Procedimiento de comparación (4 pasos):** 1) filtrar ofertas que cumplen requisitos mínimos imprescindibles (antecedentes, apartamientos, plazos); 2) armar cuadro comparativo según los criterios preestablecidos; 3) solicitar aclaraciones a los oferentes (**en licitación pública nunca pueden usarse para que el oferente modifique/ajuste su oferta**); 4) informe de adjudicación con las ofertas ordenadas de más a menos conveniente.

**Buenas prácticas al elegir criterios:** lo más cuantificables/objetivos posible, ponderación coherente con su importancia, no modificarlos después de presentadas las ofertas, mejor no considerar un criterio que considerarlo mal, usar un sistema de evaluación ya probado si existe.

**Criterios usuales** (amplía Clase 20): precio, plazo de ejecución, flujo financiero (VNA de los pagos), proyecto (si está a cargo del oferente), personal y equipos disponibles, calidad de materiales/suministros, memoria descriptiva, **rendimientos** (ej. en equipos: central térmica), capacidad y antecedentes de la empresa (preferentemente ya evaluados en precalificación).

---

## 13. Valor Neto Actualizado — concepto formal (Clase 23)

*(Formaliza la definición de VNA ya usada en la Guía de Ejercicios Tipo, sección 12 — ver ahí el desarrollo práctico con ejemplos numéricos.)*

**Por qué hace falta:** el dinero de hoy vale más que el mismo monto en el futuro (puede invertirse y generar interés; hay riesgo e inflación de por medio). Para comparar costos y beneficios que ocurren en momentos distintos —decidir entre invertir dinero o ejecutar un proyecto— hace falta **actualizar** (traer a valor presente) cada monto futuro en vez de sumarlos nominalmente.

**Definición:** criterio de evaluación económica que determina el valor presente de todos los flujos de caja futuros de una inversión, descontados a una tasa que refleja el **costo de oportunidad del capital**, menos la inversión inicial. Mide el incremento de valor que el proyecto genera para el inversor. `VNA = Σ Flujo_t / (1+i)^t`.

**Regla de decisión formal:** **VNA>0** → el proyecto genera valor por encima del costo de oportunidad → conviene. **VNA=0** → recupera exactamente el costo de oportunidad → indiferente. **VNA<0** → destruye valor → no conviene. Es la base de todos los ejercicios de comparación de alternativas y evaluación de inversiones de la Guía sección 12 (incluidos los casos de TIR=0%/indefinida).

---

## Clases ya resumidas
- Clase 1 (Introducción/administrativa del curso — objetivos, metodología, cronograma del Trabajo Práctico; **sin contenido de examen**, solo logística del curso).
- Clase 2 (Características históricas de la industria, obra pública/privada, TOCAF, tipos de contrato).
- Clase 3, Clase 4 y Clase 7 (Metrajes de hormigones y albañilería — criterios de volumen, encofrado, armaduras, planilla tipo, valores de referencia de Tenor/Cuantía por elemento, dosificación de hormigones/morteros con tabla de Coef. de Aporte y Peso Específico, descuento de aberturas en muros, ejemplos resueltos incl. Marzo-2020 con discrepancia frente a la planilla oficial — ver sección 1).
- Clase 5 (Presentación/logística del Trabajo Práctico — proyecto "Complejo Turístico Derrégibus"; **sin contenido de examen**).
- Clase 6 (Movimiento de suelos — metraje de excavaciones a mano/a máquina, áreas mínimas de trabajo, coeficientes Ce/Cc/Ca formales en cadena de 3 pasos con tabla de valores por tipo de suelo — ver sección 7).
- Clase 8 (Clasificación de costos — Fijos/Variables, Directos/Indirectos y su relación, apalancamiento operativo por ampliación/reducción de alcance, 8 grupos de Costos por Naturaleza — ver sección 8).
- Clase 9 (Mano de obra — Ley 14.411, Convenio Colectivo, ítems del jornal, viáticos, aportes, Fondos Sociales).
- Clase 19 (Riesgos, Garantías, Seguros).
- Clase 20 (Programa Económico y Financiero de obra, elaboración y comparación de ofertas).
- Equipos.pdf (Costo horario de equipos, movimiento de suelos con camiones).
- Clase 11 (Presentación del modelo de planillas Excel para la Entrega Intermedia del Trabajo Práctico — Listado de Insumos, Planilla de Consumos, Planilla Auxiliar de Hormigones (SUMAPRODUCTO), Planilla de Mano de Obra, Planilla de Dosificación; **administrativa/metodológica, confirma pero no agrega contenido de examen nuevo** más allá de lo ya cubierto en secciones 1-3 y en la Guía).
- Clase 12 (Materiales, Suministros y Subcontratos — identificación/cuantificación/valoración, INCOTERMS, Ley de Tercerizaciones — ver sección 9).
- Clase 17 (Consumo Unitario vs. Rendimiento, Consumos Estándar y coeficientes de desvío ic/ih/ie/ip, Costos Indirectos de obra con concepto de Afectación — ver sección 10; repite además la Planilla de Consumos y Planilla Auxiliar de hormigones ya vistas en Clase 11, sin contenido nuevo en esa parte).
- Clase 18 (Ajuste de precios — fórmula paramétrica oficial con fuentes J/M/CV/D, canasta de materiales, variante de alta inflación — ver sección 11).
- Clase 21 (Estudio Comparativo de Ofertas — documentación previa, contenido de la oferta, procedimiento de comparación en 4 pasos — ver sección 12; complementa Clase 20).
- Clase 23 (Inversiones — concepto formal de VNA y regla de decisión — ver sección 13; parcial, son solo 10 diapositivas introductorias, probablemente continúa en una clase posterior no incluida en el repo).

## Clases pendientes (quedan para próximas corridas)
Ninguna — **las 17 clases del repo (`CLASES TEORICAS/`) están todas resumidas** (Clase 1 a 9, 11, 12, 17, 18, 19, 20, 21, 23, más Equipos.pdf; Clase 1 y 5 son administrativas sin contenido de examen). Si en corridas futuras aparecen clases nuevas en la carpeta (ej. Clase 10, 13-16, 22, 24+), agregarlas aquí.
