# Examen Costos (2240) — 27/01/2026

No hay solución oficial en el repositorio para este examen (es el más nuevo). Esta resolución es de elaboración propia — se marcan claramente las partes con supuestos.

---

## I – Metraje (20 pts) — **RESUELTO CON SUPUESTOS EXPLÍCITOS** (sin solución oficial para verificar)

**⚠️ Nivel de confianza, léase antes de usar estos números para estudiar:**
- **Alto:** geometría (vanos de losas y longitud de vigas) — se validó por dar números redondos "limpios" (6,00m / 4,80m / 4,00m) al aplicar el método de decodificación de cotas explicado abajo, lo cual es una fuerte señal de que la lectura es correcta.
- **Alto:** volumen/encofrado/tenor de Vigas 152 y 153 (no dependen del espesor de losa, que es el único dato faltante).
- **Medio-alto:** decodificación de la notación en "cruz" del armado de losa (extiende un patrón ya confirmado contra planillas oficiales en Feb-2024/Jul-2022, con un número extra sin explicar — ver abajo).
- **Medio:** kg de acero de vigas (arranque/gancho de las barras "A"/"E" y la lectura exacta del bastón "F der" son una interpretación razonable de la planilla de armado, no 100% verificable sin la solución oficial).
- **Bajo / con supuesto fuerte:** volumen y tenor de las LOSAS, y cuantía de acero — el plano **no trae el espesor de la losa en ningún lado** (se revisó el Anexo 1 completo, el enunciado y la planilla de vigas; no hay ninguna nota "e=..."). Se usa un espesor ilustrativo de 0,15 m solo para dar un número completo — **reemplazar por el valor correcto en cuanto se consiga** (ej. de los apuntes de clase o preguntando).

### Decodificación de las cotas del plano (método nuevo, no visto en exámenes anteriores)

El Anexo 1 usa un sistema de **cotas acumuladas** (no cotas de tramo): cada línea de referencia (vertical u horizontal) tiene escrito, una sola vez a lo largo de toda su longitud, un número que es su posición en un eje de coordenadas del proyecto (parecido a un replanteo topográfico), **no** la distancia a la línea vecina. Para obtener cualquier distancia hay que **restar dos cotas de la misma familia de líneas**.

Se identificaron dos "familias" superpuestas en cada columna de líneas verticales: una junto a cada **pilar** (da el ancho del pilar) y otra junto al **tramo de viga** entre pilares (da el ancho de la viga) — por eso a veces se repite un par de números idéntico en varios pilares de la misma línea (P51/P60/P68 comparten sección 60x20, entonces los 3 repiten "4065,9 / 4005,9", Δ=60,0 ✓) y aparece un par distinto a lo largo del tramo de viga entre ellos ("4020,5 / 4000,5", Δ=20,0 ✓, coincide con el ancho de V153/V152).

**Verificación cruzada (todas las Δ dan exactamente el ancho conocido del elemento, buena señal de que la lectura es correcta):**

| Par de cotas | Δ | Elemento que confirma |
|---|---|---|
| 4065,9 / 4005,9 (junto a P51, P60, P68) | 60,0 | Ancho de pilar P51/P60/P68 (60x20) |
| 4020,5 / 4000,5 (tramo de V153, V152) | 20,0 | Ancho de viga V153/V152 (20x55) |
| 1108,7 / 1088,7 (junto a P51/V112) | 20,0 | Ancho de viga V112 (20x55) |
| 608,7 / 588,7 (junto a V115) | 20,0 | Ancho de viga V115 (20x55) |
| 188,7 / 168,7 (junto a V118) | 20,0 | Ancho de viga V118 (20x55) |
| 3400,5 / 3370,5 (junto a P52) | 30,0 | Ancho de pilar P52 (30x90) |
| 3400,5 / 3380,5 (tramo de V158, V157) | 20,0 | Ancho de viga V158/V157 (20x55) |
| 3371,4 / 3281,4 (junto a P61/P69) | 90,0 | Ancho de pilar P61 (90x20) / P69 (90x35) |

**Vano libre de cada losa = diferencia entre la cota de la cara de viga más cercana al paño, en cada dirección** (usando las cotas de tramo de viga, no las de pilar, porque son las que realmente delimitan el paño de losa):
- Dirección X (ancho, Este-Oeste): cara este de V153/V152 (4000,5) − cara oeste de V158/V157 (3400,5) = **600,0 cm = 6,00 m** (igual para Losa 1 y Losa 2, comparten la misma línea de pilares).
- Dirección Y (largo, Norte-Sur) Losa 1: cara sur de V112 (1088,7) − cara norte de V115 (608,7) = **480,0 cm = 4,80 m**.
- Dirección Y Losa 2: cara sur de V115 (588,7) − cara norte de V118 (188,7) = **400,0 cm = 4,00 m**.

*(Los tres resultados dan exactos en centímetros, sin decimales sueltos — a pesar de que las cotas originales sí tienen decimales — lo cual es una validación fuerte de que el método de lectura es el correcto.)*

**Áreas:** Losa 1 = 6,00×4,80 = **28,80 m²**. Losa 2 = 6,00×4,00 = **24,00 m²**.

**Longitud de Vigas 152 y 153** (edge beams del lado Oeste, apoyadas en V112/V115/V118 igual que la losa que bordean): V153 (borde oeste de Losa 1) = 4,80 m. V152 (borde oeste de Losa 2) = 4,00 m — mismas longitudes que el vano Y de la losa que bordean, porque están acotadas por los mismos ejes V112/V115/V118.

### d), e), f) — Vigas 152 y 153 (20x55, b=0,20m h=0,55m)

Datos de armado tomados de la planilla de vigas del Anexo 1 (página aparte del examen): V152 → A(inferior)=2Φ12, E(superior)=2Φ20+1Φ16, estribos Φ8/25. V153 → A=2Φ16, E=2Φ10, F der(bastón)=2Φ12 (long. 120/120), estribos Φ8/25. **Supuesto:** barras A/E se consideran de largo=longitud de viga + 2×gancho 10Φ en cada extremo (no se especifica en la planilla si continúan a otro tramo); estribos con gancho de cierre 2×10Φ8; F der tratado como bastón de 2,40m total (120+120cm) por barra.

| Viga | L (m) | Vol (m³) | Encof (m²) | Tenor (m²/m³) |
|---|---|---|---|---|
| V152 | 4,00 | **0,440** | **5,20** | **11,82** |
| V153 | 4,80 | **0,528** | **6,24** | **11,82** |

*(Encof=(b+2h)×L, viga suspendida con las 2 caras laterales + cara inferior encofradas, cara superior libre para hormigonar; Tenor dentro del rango típico de vigas 8-12 m²/m³ ✓.)*

**Acero (kg, por diámetro):**

| Viga | Φ8 (estribos) | Φ10 | Φ12 | Φ16 | Φ20 | Total |
|---|---|---|---|---|---|---|
| V152 | 11,56 | — | 8,30 | 7,85 | 25,00 | **52,71 kg** |
| V153 | 14,28 | 6,82 | 4,70 | 18,61 | — | **44,40 kg** |

### b) Decodificación de la notación en "cruz" del armado de losa

El símbolo al centro de cada paño tiene forma `Φ(arriba) / Φ(izq.) [caja: nº1] nº2 / nº3(abajo)`. Ej. Losa 1: `Φ8 arriba / Φ8 izq. — [15] 20 / 18 abajo`; Losa 2: `Φ8 arriba / Φ6 izq. — [15] 18 / 18 abajo`.

Extiende el patrón ya confirmado contra planilla oficial en Feb-2024/Jul-2022 (ver Guía sección 1): **diámetro de ARRIBA + paso de ABAJO** = una familia de barras (acá siempre Φ8/18 en las 3 losas del plano); **diámetro de IZQUIERDA + paso ENCERRADO EN LA CAJA** = la otra familia. El número que queda SUELTO fuera de la caja (20 en Losa 1, 18 en Losa 2) **no se pudo explicar** — mismo fenómeno ya documentado en Feb-2024 (ahí sobraba un "16" sin poder emparejarlo con nada de la planilla oficial), así que se lo descarta siguiendo el mismo criterio que validó ese examen.

Con esa lectura: Losa 1 → familia "arriba" Φ8/paso 0,18m (barras corriendo Este-Oeste, largo=vano X=6,00m); familia "izquierda" Φ8/paso 0,15m (barras Norte-Sur, largo=vano Y=4,80m). Losa 2 → familia "arriba" Φ8/0,18m (E-O, largo 6,00m); familia "izquierda" Φ6/0,15m (N-S, largo 4,00m).

Además el plano trae refuerzo negativo explícito (sin ambigüedad, rotulado directo) sobre los 3 ejes de viga: **F:1Φ8/18** sobre V112 (tramo 0,80m hacia el interior de Losa 1) y **F:1Φ10/20** sobre V115 y V118 (tramo 1,00m hacia cada losa adyacente).

**a) Volumen y c) Tenor de encofrado (dependen del espesor "e", NO dado en el plano):**

`Vol = Área × e`. Losa contenida por vigas en los 4 lados (igual que Feb-2024/Dic-2024) → **Tenor = 1/e** (atajo, Encof=Área directamente sin necesidad de e). Encofrado: Losa 1 = 28,80 m²; Losa 2 = 24,00 m².

Con un espesor **ilustrativo e=0,15m** (supuesto, no dado — ajustar si se consigue el valor real):

| Losa | Área (m²) | Vol (m³, e=0,15) | Encof (m²) | Tenor (m²/m³) |
|---|---|---|---|---|
| Losa 1 | 28,80 | 4,32 | 28,80 | 6,67 |
| Losa 2 | 24,00 | 3,60 | 24,00 | 6,67 |

**b) Acero (kg), cruz + refuerzo negativo F:**

| Losa | Φ6 | Φ8 | Φ10 | Total |
|---|---|---|---|---|
| Losa 1 | — | 149,39 (cruz) + 12,61 (F/V112) = **162,00** | 23,26 (F/V115) | **185,26 kg** |
| Losa 2 | 37,88 (cruz) | 58,97 (cruz) | 23,26 (F/V115) + 23,26 (F/V118) = **46,51** | **143,36 kg** |

*(Cuantía con e=0,15 ilustrativo: Losa 1 ≈ 185,26/4,32 = 42,9 kg/m³; Losa 2 ≈ 143,36/3,60 = 39,8 kg/m³ — algo por debajo del rango típico 60-80 kg/m³ de la tabla de referencia, coherente con ser una losa de vanos grandes (6,00m) con armado relativamente espaciado (15-20cm); si el espesor real fuera menor a 0,15m la cuantía subiría proporcionalmente.)*

---

## II – Consumos (10 pts) — **RESUELTO** (usa los mismos supuestos/espesor ilustrativo de la Parte I)

Fórmulas (ver Guía → "Consumos unitarios de hormigón armado"): Mano de obra (hs/m³)=1×(hs/m³ pasta)+tenor×(hs/m² encof)+cuantía×(hs/kg hierro); Hormigón (m³/m³)=1×(1+5%); Hierro (kg/m³)=cuantía; Chapón fenólico (unid/m³)=(tenor×(1+15%))/(1,22×2,44×7).

Usando los valores **combinados** (Losa 1+Losa 2 juntas, y V152+V153 juntas, ya que la planilla de mano de obra del enunciado da un solo consumo genérico "Losa"/"Viga", no por elemento individual): Losa combinada → Vol=7,92 m³ (e=0,15 ilustrativo), Tenor=6,67 m²/m³, Cuantía≈41,5 kg/m³. Viga combinada → Vol=0,968 m³, Tenor=11,82 m²/m³, Cuantía≈100,3 kg/m³.

| Insumo | Cálculo Losa | Losa | Cálculo Viga | Viga |
|---|---|---|---|---|
| Of. Carpintero (hs/m³) | 1,50×1 + 0,80×6,67 | **6,84** | 2,00×1 + 1,10×11,82 | **15,00** |
| Ayudante (hs/m³) | 3,00×1 + 0,80×6,67 + 0,04×41,5 | **10,00** | 3,50×1 + 1,10×11,82 + 0,04×100,3 | **20,51** |
| Of. Herrero (hs/m³) | 0,04×41,5 | **1,66** | 0,04×100,3 | **4,01** |
| Hormigón premezclado (m³/m³) | 1×1,05 | **1,05** | 1×1,05 | **1,05** |
| Acero (kg/m³) | =cuantía | **41,5** | =cuantía | **100,3** |
| Chapón fenólico (unid/m³) | (6,67×1,15)/(2,9768×7) | **0,367** | (11,82×1,15)/(2,9768×7) | **0,650** |

*(Estos valores heredan la incertidumbre del espesor ilustrativo de la Parte I — recalcular con el espesor real en cuanto se consiga; el resto de la receta no cambia.)*

---

## III – Costo de equipos (15 pts) — **RESUELTO**

Retroexcavadora combinada. Datos: VN=50.000 U$D, VR=15.000 U$D, n=5 años, H=180 horas de uso al año, i=7% anual, s=2% anual, p=1% anual, K=70% (tasa leyes sociales sobre monto imponible), u=80% (monto imponible = 80% del jornal). 1 U$D = 38,5 $.

**Supuesto clave:** "H = Horas de uso = 180" se interpreta como horas de uso **anuales** (equipo de baja utilización — coherente con "obra privada de arquitectura" de poco porte), ya que todos los demás datos (i, s, p) son tasas anuales y no se da una cantidad de meses/año para anualizar un dato mensual. Vida útil total = n×H = 5×180 = **900 horas**.

**Supuesto sobre "Filtro":** la fila da Unidad "% s/lub", Cant/hora "50%" y Costo unitario "57,75 $" (=50%×115,5, el precio del litro de aceite). Se interpretó manteniendo la misma estructura que el resto de la tabla (cantidad × costo unitario): Filtro = 0,50 × 57,75 = 28,875 $/h.

### 1) Costos fijos

| Concepto | Fórmula | Resultado |
|---|---|---|
| Amortización | (VN-VR)/(n×H) = (50.000-15.000)/900 | 38,89 U$D/h = **1.497,22 $/h** |
| Seguro | s×VN/H = 0,02×50.000/180 | 5,56 U$D/h = **213,89 $/h** |
| Patente | p×VN/H = 0,01×50.000/180 | 2,78 U$D/h = **106,94 $/h** |
| Costo financiero | [(VN-VR)/2 × i]/H = (17.500×0,07)/180 | 6,81 U$D/h = **262,01 $/h** |
| **Total costos fijos** | | **2.080,07 $/h** |

### 2) Costo operativo (combustible + mano de obra directa)

| Insumo | Cálculo | $/h |
|---|---|---|
| Gasoil | 6 lt/h × 49,77 $/lt | 298,62 |
| Ayudante | 1,1 hh × 390 $/hh | 429,00 |
| Maquinista | 1,1 hh × 540 $/hh | 594,00 |
| **Total costo operativo** | | **1.321,62 $/h** |

### 3) Costo de mantenimiento (lubricantes + neumáticos)

| Insumo | Cálculo | $/h |
|---|---|---|
| Aceite lubricante | 0,66 lt/h × 115,5 $/lt | 76,23 |
| Grasa | 0,22 kg/h × 77 $/kg | 16,94 |
| Filtro | 0,50 × 57,75 $ | 28,875 |
| Neumáticos (TR) | (1/4.500 juego/h) × 4.200 U$D × 38,5 = 0,933 U$D/h | 35,93 |
| **Total costo de mantenimiento** | | **157,98 $/h** |

### Leyes Sociales (LLSS) — separadas

Monto imponible = u × jornal = 0,80 × jornal. LLSS = K × Monto imponible = 0,70×0,80×jornal = 0,56×jornal.

| | Jornal $/h | LLSS $/h |
|---|---|---|
| Ayudante | 429,00 | 240,24 |
| Maquinista | 594,00 | 332,64 |
| **Total LLSS** | | **572,88 $/h** |

### Resumen

| | $/h |
|---|---|
| Costos fijos | 2.080,07 |
| Costo operativo (sin LLSS) | 1.321,62 |
| Costo de mantenimiento | 157,98 |
| **Costo total de producción (sin LLSS)** | **3.559,67** |
| **LLSS (aparte)** | **572,88** |
| **Costo total de producción (con LLSS)** | **4.132,55 $/h** |

---

## IV – Mano de obra (15 pts) — **RESUELTO** (teórico)

**a) Sistema de remuneración amparado por la Ley 14.411:**
El sector Construcción (Grupo 9 de la Actividad Nacional) tiene un régimen especial regulado principalmente por el decreto-ley N.º 14.411, complementado por el Convenio Colectivo tripartito homologado por el Poder Ejecutivo. Existen dos formas de retribución:
- **Por tiempo trabajado**: mensuales (encargados/capataces) o jornaleros (44 hs/semana: lunes a jueves 9 hs, viernes 8 hs), según Laudos del Consejo de Salarios vigentes por período. Se suman partidas: hora común, compensaciones por ropa/transporte/herramientas, incentivos por presentismo semanal (10,42%) y mensual (5%), media hora de descanso, horas extra (+100%), feriados no laborables (7 al año), horas de lluvia/barro/crecidas (topeadas por cuatrimestre), viáticos por distancia, suplemento por altura, horas nocturnas (+30%/+50%), tickets de alimentación, vestimenta de invierno/verano.
- **Por producción ("destajo")**: se paga por unidad de obra ejecutada (ej. m² de muro); poco usado en presupuestación convencional, no genera horas extra ni la mayoría de las compensaciones.

**b) Sistema de gestión de aportes sociales — Aporte Unificado de la Construcción:**
El personal con tareas directas en obra tributa el **Aporte Unificado de la Construcción** (en vez del régimen general de Industria y Comercio, que sí aplica a directores, administrativos, técnicos y profesionales sin tareas específicas en obra). Se calcula como:

`TOTAL A PAGAR = [Precio Obra + IVA] + [Monto Imponible de Mano de Obra] × (Coeficiente de Aporte Unificado según tipo de obra)`

El **Monto Imponible (MI)** ronda el 80% del salario del operario y las **Leyes Sociales** representan aprox. 71,8% (obra pública) o 75,8% (obra de arquitectura) del MI (incluye el 4% de CJPPU si es obra de arquitectura, o 2% si es de ingeniería, sobre Ley 17.738). Partidas del MI:
- Gravadas totalmente: jornal de laudo, presentismo semanal/mensual, horas extra, feriados no laborables, nocturnidad, horas en altura.
- No gravadas: ropa, herramientas, transporte, media hora de descanso, pasajes, horas de lluvia, tickets de alimentación.
- Parcialmente gravadas: sobre-laudo, viático, incentivo por producción — se suman como Remuneración Total (RT=a+b); si b<30% de RT no se grava, si b>30% se grava el 50% del excedente.

**c) Partes del Convenio Colectivo de la Construcción en Uruguay:**
Convenio tripartito entre **Empresas** (cámaras empresariales), **Trabajadores** (SUNCA) y **MTSS/Poder Ejecutivo** (que homologa). Se renueva cada 3 años y trata: laudos salariales y su ajuste (vinculado a metas de inflación del BCU), categorías, compensaciones, licencias, políticas de género e inclusión de personas con discapacidad, régimen de horas de lluvia/barro/crecidas, desgaste de herramientas, etc.

**d) Los 4 Fondos Sociales de la Construcción:**
1. **FOSVOC** (Fondo Social de Vivienda de Obreros de la Construcción): ayuda a la compra, construcción o reforma de vivienda de los obreros.
2. **Fondo Social de la Construcción (FSC)**: financia canastas familiares de fin de año, útiles escolares para hijos de obreros, cursos de computación, servicios odontológicos, capacitación.
3. **FOCAP**: cursos de capacitación técnica para trabajadores ocupados de la industria (soldadura, operación de maquinaria, etc.).
4. **FOCER** (Fondo de Cesantía y Retiro): cuentas individuales de ahorro por trabajador, con aportes patronales y personales, disponibles en su totalidad para el trabajador.

---

## V – Licitaciones (15 pts) — **RESUELTO** (teórico)

**a) Procedimientos para obras públicas según el TOCAF (Texto Ordenado de Contabilidad y Administración Financiera, Sección 2 Art. 33°):**

| Procedimiento | Monto |
|---|---|
| Compra Directa | hasta $630.000 ($987.000 en Gobiernos Departamentales) |
| Concurso de Precios | hasta $1.000.000 |
| Licitación Abreviada | hasta $10.000.000 |
| Licitación Pública | obligatoria por encima de $10.000.000 |

Existen excepciones a la Licitación Pública sin importar el monto: compras entre organismos estatales, procedimiento competitivo desierto, bienes/servicios de proveedor único, reparaciones de maquinaria no trasladable, urgencias/emergencias. Las contrataciones deben publicarse en ARCE y son controladas por el Tribunal de Cuentas.

**b) Tipos de contrato:**
- **i) Precio Global (ajuste alzado)**: precio fijo total por toda la obra, independiente de los costos reales. Ventaja: el cliente conoce el costo total desde el inicio (transfiere el riesgo de sobrecosto al contratista). Desventaja: poca flexibilidad ante cambios, el contratista incluye márgenes de seguridad. *Ejemplo: construcción de una vivienda unifamiliar con proyecto cerrado.*
- **ii) Precio Unitario**: se pactan precios por unidad de cada partida (ej. $/m³ de hormigón, $/m² de pavimento) y se paga según cantidades realmente ejecutadas. Ventaja: flexible ante variaciones de cantidades; se adapta a obras donde no se puede definir con precisión el metraje inicial. Desventaja: incertidumbre del costo final, requiere control riguroso de mediciones. *Ejemplo: obras viales o de saneamiento (redes de tuberías, cámaras) donde las cantidades reales de excavación/tubería se definen en obra.*
- **iii) Por Administración**: el contratista cobra los costos reales de la obra más un % o suma fija por su gestión. Ventaja: permite iniciar sin definir completamente el alcance, transparencia de costos. Desventaja: requiere control detallado de gastos, poco incentivo a reducir costos si no hay tope. *Ejemplo: reforma/remodelación con alcance impreciso al inicio (ej. reparación post-incendio de una estructura, donde no se conoce a priori el alcance real del daño).*

---

## VI – Garantías y Seguros (15 pts) — **RESUELTO** (teórico)

**a) Garantías requeridas por el Contratante:**

| Garantía | Momento | Monto usual | Plazo | Constitución |
|---|---|---|---|---|
| Mantenimiento de Oferta | previo/al presentar la oferta | ~1% del monto ofertado (o monto fijo) | 3 a 6 meses | aval bancario, póliza, depósito |
| Fiel Cumplimiento de Contrato | previo a la firma del contrato | ~5% del monto contratado | desde la firma hasta recepción provisoria | ídem |
| Fondo de Reparo (Buena Ejecución) | fraccionada, previo a cada certificado | ~5% de cada certificado | hasta recepción definitiva | retención en cada certificado |
| Sustitución de Fondo de Reparo | previo al inicio de obra | % equivalente a lo que se retendría | hasta recepción definitiva | evita el costo financiero de la retención |
| Anticipo o Acopio | previo a recibir el anticipo | 100% del anticipo | hasta devolución total (gradual, por certificado) | aval bancario/póliza (~3% anual del monto) |

Incidencia en el costo total: cada garantía tiene un costo de póliza/aval (entre 0,4% y 3% del monto garantizado según el tipo) que se traslada al presupuesto de la obra; sumadas, suelen representar un orden de 0,5%-1% del precio de venta de la obra.

**b) Componentes principales de un Seguro:** objeto asegurado, valor del objeto, riesgos/eventos cubiertos, monto máximo de indemnización, prima (costo), deducible, plazo de vigencia, deberes del contratante, exclusiones.

**Seguros necesarios en la construcción:**
1. **Accidentes de Trabajo** (obligatorio por Ley 16.074, monopolio del BSE): para obreros amparados en Ley 14.411 va incluido en el aporte unificado; personal técnico 2% de su salario; administrativo 0,6%.
2. **Vehículos y maquinaria**: cubre daños al equipo propio y a terceros; ~2% del valor del equipo/año.
3. **Todo Riesgo de Construcción (TRC)**: cubre derrumbe, incendio, inundación, accidentes sobre la obra y propiedad adyacente; 0,3%-0,5% del monto del contrato en obras comunes (más en obras marítimas/portuarias).
4. **Responsabilidad Civil (RC)**: cubre daños a terceros por la actividad del contratista; ~0,3% anual sobre el monto del contrato (muchas TRC ya incluyen un RC adicional limitado).
5. Otros: diseño, cumplimiento de plazos, cumplimiento de demanda, etc.
