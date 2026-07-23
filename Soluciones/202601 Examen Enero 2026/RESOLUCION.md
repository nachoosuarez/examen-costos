# Examen Costos (2240) — 27/01/2026

No hay solución oficial en el repositorio para este examen (es el más nuevo). Esta resolución es de elaboración propia — se marcan claramente las partes con supuestos.

---

## I – Metraje (20 pts) — **PENDIENTE / parcial**

El Anexo 1 muestra una planta con Losa 1 y Losa 2 (apoyadas en vigas V151 a V158, V112, V115, V118, V121 y pilares P51/P52/P60/P61/P68/P69) más una planilla de armado de vigas (V151 a V155).

**Lo que se puede afirmar con certeza del plano:**
- Vigas 152 y 153: sección 20x55 (b=20cm, h=55cm) para ambas.
- Planilla de hierros de vigas (armadura inferior "A", superior "E", bastón "F der", estribos):
  - V152: A = 2Φ12, E = 2Φ20+1Φ16, estribos Φ8/25.
  - V153: A = 2Φ16, E = 2Φ10, F der = 2Φ12 (long. 120/120), estribos Φ8/25.
- Losa 1 y Losa 2: armadura de base (mostrada en cruces al centro de cada paño) con diámetros Φ8/Φ6 y separaciones 15/18/20 cm, más refuerzos superiores sobre apoyos indicados como "F:1Φ8/18", "F:1Φ10/20", "F:1Φ10/16" con tramos de 80/100 cm.
- Reglas generales a aplicar (de "Aclaraciones sobre errores comunes"): volumen de losa entre vigas (sin incluir vigas), encofrado de losa solo cara inferior fuera de vigas, cantidad de barras = redondear.hacia arriba(tramo/paso)+1, ganchos 10Φ donde no se especifican, empalmes 50Φ, varillas de 12 m.

**Por qué queda pendiente:** para completar a)/c)/d)/e)/f) hace falta decodificar las cotas acumuladas del plano (pares de números como 4065,9/4005,9; 1108,7/1088,7; 608,7/588,7; 188,7/168,7; 3400,5/3380,5; 3371,4/3281,4, etc.) que fijan los tramos exactos de losas y vigas, y para b) la notación en cruz de armado de losa (Φ8 arriba, Φ8 a la izquierda, caja con "15|20", "18" abajo) no tiene un legend explícito en el repo (se revisaron todas las Clases Teóricas y los exámenes con solución anteriores sin encontrar la misma convención). Antes de dar un número en negrita se prefiere dejarlo marcado como pendiente a resolver con más tiempo/una consulta al legajo del curso, en vez de arriesgar un resultado engañoso para el estudio.

**Próximo paso sugerido:** releer el Anexo 1 a alta resolución tramo por tramo (los pares de cotas probablemente son "cara de columna" vs "eje de columna" o "inicio/fin de barra"), y si es posible, contrastar la notación de la cruz de armado con el docente o con un ejemplo de clase que la explique.

---

## II – Consumos — **PENDIENTE** (depende de los metrajes de I)

La receta general (ver Guía de ejercicios tipo → "Consumos unitarios de hormigón armado") es:
- Mano de obra (hs/m³) = 1×(hs/m³ pasta) + tenor×(hs/m² encofrado) + cuantía×(hs/kg hierro), por oficio.
- Hormigón (m³/m³) = 1×(1+desperdicio%).
- Hierro (kg/m³) = cuantía (kg hierro / m³ hormigón).
- Chapón fenólico (unid/m³) = (tenor×(1+desperdicio%)) / (área_unitaria × reúsos).

Con los datos de mano de obra dados (Losa: pasta 1,50 Of.Carp / 3,00 Ayud hs/m³; encofrado 0,80/0,80 hs/m²; hierro 0,04/0,04 hs/kg — Viga: pasta 2,00/3,50; encofrado 1,10/1,10; hierro 0,04/0,04) y chapón fenólico 1,22m x 2,44m, desperdicio 15%, reúsos 7, esto se resuelve en cuanto se tenga el tenor y la cuantía de Losas/Vigas de la parte I.

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
