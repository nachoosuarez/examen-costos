# Estado del trabajo — Costos (actualizado: corrida del 23/07/2026 — 17ª pasada)

## Resumen ejecutivo (leer esto primero)
1. Van 19 exámenes con resolución escrita: **Enero 2026** (parcial), **Diciembre 2025**, **Julio 2025**, **Marzo 2025**, **Febrero 2025**, **Diciembre 2024**, **Julio 2024**, **"Marzo 2024"** (real 20/02/2024), **Febrero 2024** (real 30/01/2024), **Diciembre 2023**, **Julio 2023**, **"Marzo 2023"** (real 16/02/2023), **Febrero 2023** (real 26/01/2023), **Diciembre 2022**, **Julio 2022**, **"Marzo 2022"** (real 15/02/2022), **Febrero 2022** (real 26/01/2022), **Diciembre 2021** y **Diciembre 2020** — los últimos 18 completos (partes con solución oficial verificadas exactas, teóricas con criterio de la Guía). Faltan 5 exámenes más viejos (2019-2020).
2. Lo más urgente para estudiar ya mismo: **`RESUMEN EXAMEN/Ejercicios_tipo/GUIA_EJERCICIOS_TIPO.md`** — 16 tipos de ejercicio con receta paso a paso (metraje —con variantes losa simple/doble capa/muro con bloques/muro monolítico/losa angosta/losa con bordes de escalón/viga de sección compuesta/relleno triangular/vigas de fundación con doble familia de armado, **y la planilla en "cruz" ya DECODIFICADA**—, consumos, dosificación de hormigón —con variante de doble aplicación del Coef. de Aporte y variante "costo de componentes" con volumen de agua escalado—, costo de equipos —con variantes de interés sobre capital medio y costo directo de una tarea (cuadrilla+equipo×rendimiento)—, costo de mano de obra, Ley 14.411, garantías con perfil temporal —con variantes Monto Imponible dado directo y Monto Imponible a estimar (80%)—, fórmula paramétrica —con ejemplo completo de reparto de Indirectos+Beneficio en CV/Dólar—, licitaciones/TOCAF, punto de equilibrio —con variantes de apalancamiento operativo, extensión de plazo, y reducción de plazo (espejo)—, costo financiero/VNA —con variantes comparar alternativas (2 y 3 alternativas, caso mixto donde solo una compensa), ajustar un pago para VNA exacto, flujo de caja+línea de crédito, cronograma económico vs. financiero armado desde cero con 2 alternativas de remuneración de saldos, y **aproximar la TIR por interpolación lineal**—, movimiento de suelos —con definiciones formales Ce/Cc/Ca, variante terraplén+desmonte reutilizado, variante de secciones transversales de calle con peralte, y variante de costeo completo de sustitución de suelo bajo platea circular—, seguros, suministros, clasificación de costos por naturaleza).
3. **¡Actualización importante!** La notación de armado de losa en "cruz" (que había bloqueado la Parte I de **Enero 2026**, sin solución oficial en el repo) quedó **decodificada** al comparar Feb-2024 y Jul-2022 contra sus soluciones oficiales: el número de abajo es el paso de la familia vertical, y los dos números del medio (casi siempre iguales) son el mismo paso de la familia horizontal repetido. Sigue pendiente re-visitar Enero 2026 con esta clave para intentar resolver su Parte I y II. Ver Guía sección 1.
4. **Diciembre 2025, Julio 2025, Marzo 2025, Febrero 2025, Diciembre 2024, Julio 2024, "Marzo 2024", Febrero 2024, Diciembre 2023, Julio 2023, "Marzo 2023", Febrero 2023, Diciembre 2022, Julio 2022, "Marzo 2022", Febrero 2022, Diciembre 2021 y Diciembre 2020** están resueltos (las partes con solución oficial en el repo, verificadas exactamente; las teóricas puntuales sin solución oficial se respondieron con el criterio de la Guía).
5. **Diciembre 2020** (solución oficial parcial, I-II) trajo un tipo de ejercicio **NUEVO para la Guía**: consumo de mampostería y revoques (ticholos + 4 tipos de mortero — toma/impermeable/grueso/fino —, cada uno con su propia dosificación en partes y espesor), con el mismo método de Coeficiente de Aporte que la dosificación de hormigón pero aplicado capa por capa. También trajo una advertencia útil sobre fórmula paramétrica: **verificar siempre el orden de magnitud de los índices de una tabla de referencia real** antes de usarlos (la propia solución oficial marca 2 valores erróneos en la tabla del Anexo). Ver Guía secciones 8 y 16.
6. El resumen teórico cubre **5 clases completas** (Clase 2, 3, 9, 19, 20) + Equipos.pdf; quedan 12 clases sin resumir todavía (ver lista abajo).
7. Prioridad para la próxima corrida: seguir con **Julio 2020** hacia atrás (2020→2019, quedan 5 exámenes: Jul-2020, Marzo-2020, Feb-2020, Dic-2019, Jul-2019; Feb-2020 tiene parcial de preguntas A,B,D y Dic-2019 tiene solución oficial completa "Respuestas"); si hay tiempo, sumar clases teóricas pendientes (sugerido: Clase 21 y Clase 23, más cercanas en el temario a lo ya visto — Clase 20 resultó ser "Programa Económico-Financiero + Elaboración/Comparación de Ofertas", puede que Clase 21 solape parcialmente, revisar contenido real al leerla).

## Exámenes — estado (del más nuevo al más viejo)

| Examen | Estado | Notas |
|---|---|---|
| 202601 Enero 2026 | 🟡 Parcial | III (equipos), IV, V, VI resueltos. I (metraje losas) y II (consumos) pendientes — ver limitación de plano en `Soluciones/202601 Examen Enero 2026/RESOLUCION.md`. Sin solución oficial en el repo. |
| 202512 Dic 2025 | ✅ Completo | Verificado contra solución oficial. Muro de contención con bloques, fórmula paramétrica, costo horario obrero, garantías, suministros. |
| 202507 Jul 2025 | ✅ Completo | Verificado contra solución oficial. Metraje de pilar, dosificación, VNA, movimiento de suelos, TOCAF, régimen salarial. |
| 202503 Marzo 2025 | ✅ Completo | Verificado contra planilla oficial de solución (I-IV, incluida en el propio PDF de la letra). Metraje losa doble capa, dosificación, fórmula paramétrica, punto de equilibrio, VNA/TIR, suministros. |
| 202502 Feb 2025 | ✅ Completo | Verificado contra planilla oficial de solución (I-III). Metraje muro monolítico en L, dosificación, costo de equipo (retroexcavadora), seguros, régimen salarial, Estado Económico-Financiero. |
| 202412 Dic 2024 | ✅ Completo | Verificado contra planilla oficial de solución (I,II,IV,V). Metraje losa angosta (tenor=1/e), consumos, garantías (3 tipos), punto de equilibrio (apalancamiento operativo), fórmula paramétrica, Ce/Cc/Ca, clasificación de costos por naturaleza. |
| 202407 Jul 2024 | ✅ Completo | Verificado contra solución oficial (planilla en el PDF de la letra). Metraje losa con bordes de escalón (3er caso de "cruz", no bloqueó por tener planilla resuelta), movimiento de suelos (terraplén+desmonte reutilizado), garantías, subcontratos, riesgos, TIR/VNA. |
| 202403 "Marzo 2024" (real 20/02/2024) | ✅ Completo | Verificado contra solución oficial (I,II,III,V). Metraje de viga compuesta, dosificación (Coef. Aporte doble), costo directo de cuadrilla+equipo (izado de columna), fórmula paramétrica (4 repartos válidos). Parte IV (Seguros) teórica, sin solución oficial. |
| 202402 Feb 2024 (real 30/01/2024) | ✅ Completo | Verificado contra solución oficial (I,II,III,IV,V). Metraje losa 4 lados (Tenor=1/e, 4º caso "cruz" parcialmente decodificado), VNA comparando 3 alternativas, garantías (Monto Imponible dado directo), punto de equilibrio. Parte VI (Régimen Salarial) teórica, sin solución oficial. |
| 202312 Dic 2023 | ✅ Completo | Verificado contra solución oficial (I,II,III). Metraje viga con alero+triángulo, HH/m³ más alto visto, flujo de caja con anticipo + elección de línea de crédito (tipo nuevo). Partes IV,V,VI teóricas, sin solución oficial. |
| 202307 Jul 2023 | ✅ Completo | Verificado contra solución oficial (I-V). Muro de contención en L, consumos con enunciado inconsistente ("viga"→muro), VNA 3 alternativas (caso mixto), garantías, punto de equilibrio. Parte VI teórica, sin solución oficial. |
| 202303 "Marzo 2023" (real 16/02/2023) | ✅ Completo | Verificado contra solución oficial (I-III). Viga chica muy densa, cronograma económico vs. financiero desde cero (anticipo+90días+convenio colectivo+30días), línea de crédito, 2 alternativas de remuneración (tipo nuevo). Partes IV,V,VI teóricas, sin solución oficial. |
| 202302 Feb 2023 (real 26/01/2023) | ✅ Completo | Verificado contra solución oficial (I-III). 4 vigas de fundación (doble familia de armado en las 2 mayores), VNA 3 alternativas + ajuste de pago para VNA exacto (tipo nuevo), garantías (solo fiel cumplimiento+buena ejecución). Partes IV,V teóricas, sin solución oficial. |
| 202212 Dic 2022 | ✅ Completo | Verificado contra solución oficial (I,III,V). Movimiento de suelos por secciones transversales con peralte (tipo nuevo), extensión de plazo 12→18 meses (tipo nuevo), fórmula paramétrica con ejemplo completo. Partes II,IV teóricas, sin solución oficial. |
| 202207 Jul 2022 | ✅ Completo | Verificado contra solución oficial (A-D). Metraje losa "cruz" **DECODIFICADA**, dosificación completa, movimiento de suelos con costeo de 8 tareas (platea circular, tipo nuevo), garantías (Monto Imponible a estimar). Parte E teórica, sin solución oficial. |
| 202203 "Marzo 2022" (real 15/02/2022) | ✅ Completo | Verificado contra solución oficial (A-D). Metraje losa+viga separados, costo de componentes de hormigón, reducción de plazo (tipo espejo de Dic-2022), VNA/TIR con interpolación lineal (tipo nuevo). Parte E teórica, sin solución oficial. |
| 202202 Feb 2022 (real 26/01/2022) | ✅ Completo | Verificado contra solución oficial (I-V). Metraje viga T-invertida asimétrica (3 perfiles de estribo), garantías (Monto Imponible a estimar 80%, mismo patrón que Jul-2022), VNA/TIR (teórico, por qué obra usa margen y no TIR), suministros, fórmula paramétrica. |
| 202112 Dic 2021 | ✅ Completo | Verificado contra solución oficial (I-II). Metraje pilar circular+zapata con ensanche de sección, excavación con talud/tronco de pirámide (3 coeficientes, 3 preguntas), costo horario de retroexcavadora. Partes III,IV,V teóricas, sin solución oficial. |
| 202012 Dic 2020 | ✅ Completo | Verificado contra solución oficial (I-II). Metraje viga-dintel con pretil/alero, consumo de mampostería y revoques (tipo NUEVO en la guía), fórmula paramétrica con índices de boletín real (+ alerta de datos erróneos). Partes III,IV teóricas, sin solución oficial. |
| 202007 Jul 2020 | ⬜ Pendiente | **Siguiente a resolver.** |
| 202003 Marzo 2020 | ⬜ Pendiente | |
| 202002 Feb 2020 | ⬜ Pendiente | Tiene parcial de preguntas (A,B,D). |
| 201912 Dic 2019 | ⬜ Pendiente | Tiene solución oficial ("Respuestas"). |
| 201907 Jul 2019 | ⬜ Pendiente | Tiene parcial de preguntas (A,B,C,D,E). |

## Clases teóricas — resumidas vs. pendientes

**Resumidas:** Clase 2, Clase 3, Clase 9, Clase 19, Clase 20, Equipos.pdf.

**Pendientes:** Clase 1, Clase 4, Clase 5, Clase 6, Clase 7, Clase 8, Clase 11, Clase 12, Clase 17, Clase 18, Clase 21, Clase 23.

## Tipos de ejercicio ya cubiertos en la guía
1. Metraje de hormigón armado (losas simples/con doble capa/angostas, vigas, pilares, zapatas, muros con bloques, muros monolíticos en L).
2. Consumos unitarios de hormigón armado.
3. Dosificación y costo de un m³ de hormigón.
4. Costo horario de equipos (incluye variante de interés sobre capital medio).
5. Costo horario de mano de obra (jornalero).
6. Leyes sociales / Ley 14.411 (Aporte Unificado).
7. Garantías con perfil variable en el tiempo (2 ejemplos numéricos completos).
8. Fórmula paramétrica.
9. Licitaciones — TOCAF y tipos de contrato.
10. Garantías y Seguros (teórico general).
11. Punto de Equilibrio y costos fijos/variables (incluye apalancamiento operativo).
12. Costo Financiero — Valor Neto Actualizado (VNA).
13. Movimiento de suelos (viajes de camión, con definiciones formales Ce/Cc/Ca).
14. Suministros / INCOTERMS.
15. Clasificación de costos por Naturaleza.
16. Consumo de mampostería y revoques (ticholos + morteros de toma/impermeable/grueso/fino).

**Pendientes de agregar** (aparecerán al resolver exámenes más viejos): metraje de tanques/escaleras/zapatas aisladas, planilla de armado de losas en "cruz" (sigue sin legend 100% clara pese a 3 intentos: Ene-2026, Dic-2024, Jul-2024), Estado Económico-Financiero como ejercicio numérico completo (por ahora solo conceptual, ver Feb-2025).

## Dónde está cada cosa
- `Soluciones/<examen>/RESOLUCION.md` — desarrollo paso a paso de cada examen resuelto.
- `RESUMEN EXAMEN/Ejercicios_tipo/GUIA_EJERCICIOS_TIPO.md` — la guía de estudio más importante, por tipo de ejercicio.
- `RESUMEN EXAMEN/Teorico/RESUMEN_TEORICO.md` — resumen de las clases teóricas, con tabla de frecuencia de temas.
- Este archivo (`_ESTADO.md`) — panorama general, actualizar al final de cada examen resuelto.
