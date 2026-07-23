# Resumen Teórico — Costos (ingeniería de costos de obra)

## Índice de temas por frecuencia en exámenes (se actualiza con cada examen resuelto)

| Tema | Exámenes en que apareció (hasta ahora) | Frecuencia |
|---|---|---|
| Metraje de hormigón (losas/vigas/muros/pilares) | Ene-2026, Dic-2025, Jul-2025 | 3/3 |
| Consumos unitarios + dosificación de hormigón | Ene-2026, Dic-2025, Jul-2025 | 3/3 |
| Mano de obra / Ley 14.411 / Convenio Colectivo | Ene-2026, Dic-2025, Jul-2025 | 3/3 |
| Licitaciones (TOCAF, tipos de contrato) | Ene-2026, Jul-2025 | 2/3 |
| Costo de equipos | Ene-2026 | 1/3 |
| Garantías y Seguros | Ene-2026, Dic-2025 | 2/3 |
| Fórmulas paramétricas | Dic-2025 | 1/3 |
| Costo Financiero / VNA | Jul-2025 | 1/3 |
| Movimiento de suelos | Jul-2025 | 1/3 |
| Suministros / INCOTERMS | Dic-2025 | 1/3 |

*(Se irá completando a medida que se resuelvan más exámenes — objetivo: que esta tabla diga qué estudiar primero.)*

---

## 1. Metrajes de hormigones (Clase 3)

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

## Clases ya resumidas
- Clase 2 (Características históricas de la industria, obra pública/privada, TOCAF, tipos de contrato).
- Clase 3 (Metrajes de hormigones — criterios de volumen, encofrado, armaduras, planilla tipo).
- Clase 9 (Mano de obra — Ley 14.411, Convenio Colectivo, ítems del jornal, viáticos, aportes, Fondos Sociales).
- Clase 19 (Riesgos, Garantías, Seguros).
- Equipos.pdf (Costo horario de equipos, movimiento de suelos con camiones).

## Clases pendientes (quedan para próximas corridas)
Clase 1, Clase 4, Clase 5, Clase 6, Clase 7, Clase 8, Clase 11, Clase 12, Clase 17, Clase 18, Clase 20 (Programa Económico y Financiero de obra), Clase 21 (Estudio Comparativo de Ofertas), Clase 23.
