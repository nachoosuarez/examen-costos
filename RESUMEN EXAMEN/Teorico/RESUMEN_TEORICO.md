# Resumen Teórico — Costos (ingeniería de costos de obra)

## Índice de temas por frecuencia en exámenes (se actualiza con cada examen resuelto)

| Tema | Exámenes en que apareció (hasta ahora) | Frecuencia |
|---|---|---|
| Metraje de hormigón (losas/vigas/muros/pilares) | Ene-2026, Dic-2025, Jul-2025, Marzo-2025, Feb-2025, Dic-2024 | 6/6 |
| Consumos unitarios + dosificación de hormigón | Ene-2026, Dic-2025, Jul-2025, Marzo-2025, Feb-2025, Dic-2024 | 6/6 |
| Mano de obra / Ley 14.411 / Convenio Colectivo | Ene-2026, Dic-2025, Jul-2025, Feb-2025 | 4/6 |
| Garantías y Seguros | Ene-2026, Dic-2025, Feb-2025, Dic-2024 | 4/6 |
| Punto de equilibrio / costos fijos-variables | Marzo-2025, Dic-2024 | 2/6 |
| Costo de equipos | Ene-2026, Feb-2025 | 2/6 |
| Licitaciones (TOCAF, tipos de contrato) | Ene-2026, Jul-2025 | 2/6 |
| Fórmulas paramétricas | Dic-2025, Marzo-2025, Dic-2024(conceptual) | 3/6 |
| Costo Financiero / VNA | Jul-2025, Marzo-2025(conceptual) | 2/6 |
| Movimiento de suelos | Jul-2025, Dic-2024(conceptual) | 2/6 |
| Suministros / INCOTERMS | Dic-2025, Marzo-2025 | 2/6 |
| Estado Económico y Financiero de la obra (Clase 20) | Feb-2025 | 1/6 |
| Clasificación de costos por naturaleza | Dic-2024 | 1/6 |

*(Se irá completando a medida que se resuelvan más exámenes — objetivo: que esta tabla diga qué estudiar primero.)*

---

## 1. Metrajes de hormigones (Clase 3 y Clase 4)

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

**Garantías contractuales requeridas por el Contratante:** Mantenimiento de Oferta, Fiel Cumplimiento de Contrato, Fondo de Reparo (Buena Ejecución), Sustitución de Fondo de Reparo, Anticipo o Acopio, Ley de Tercerizaciones, otras. (Detalle de monto/plazo/objetivo de cada una en la Guía de Ejercicios Tipo, sección 7). Formas de constitución: garantía bancaria, carta de crédito irrevocable, póliza de seguro de fianza (BSE), bonos del tesoro en U$D, depósito.

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

## Clases ya resumidas
- Clase 1 (Introducción/administrativa del curso — objetivos, metodología, cronograma del Trabajo Práctico; **sin contenido de examen**, solo logística del curso).
- Clase 2 (Características históricas de la industria, obra pública/privada, TOCAF, tipos de contrato).
- Clase 3 y Clase 4 (Metrajes de hormigones — criterios de volumen, encofrado, armaduras, planilla tipo, valores de referencia de Tenor/Cuantía por elemento, ejemplos resueltos incl. Marzo-2020 con discrepancia frente a la planilla oficial — ver sección 1).
- Clase 5 (Presentación/logística del Trabajo Práctico — proyecto "Complejo Turístico Derrégibus"; **sin contenido de examen**).
- Clase 6 (Movimiento de suelos — metraje de excavaciones a mano/a máquina, áreas mínimas de trabajo, coeficientes Ce/Cc/Ca formales en cadena de 3 pasos con tabla de valores por tipo de suelo — ver sección 7).
- Clase 9 (Mano de obra — Ley 14.411, Convenio Colectivo, ítems del jornal, viáticos, aportes, Fondos Sociales).
- Clase 19 (Riesgos, Garantías, Seguros).
- Clase 20 (Programa Económico y Financiero de obra, elaboración y comparación de ofertas).
- Equipos.pdf (Costo horario de equipos, movimiento de suelos con camiones).

## Clases pendientes (quedan para próximas corridas)
Clase 7, Clase 8, Clase 11, Clase 12, Clase 17, Clase 18, Clase 21 (probablemente Estudio Comparativo de Ofertas ampliado o Elaboración de Contratos — verificar contenido real al leerla), Clase 23.
