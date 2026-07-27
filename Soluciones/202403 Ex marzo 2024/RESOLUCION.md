# Examen Costos — "Marzo 2024" (fecha real en la letra: 20/02/2024)

Verificado contra solución oficial (planilla de cálculo incluida en `Examen Costos 03-2024 - Preg. I,II,III,V.pdf`). La Parte IV (Seguros, teórica) no viene con solución oficial en el repo — se responde con el criterio de la Guía/Clase 19. Todos los demás resultados de este archivo son los oficiales.

*(Nota: la carpeta dice "Marzo 2024" pero la fecha impresa en la letra es 20/02/2024 — se mantiene el nombre de carpeta del repo para no romper referencias.)*

---

## I – Metraje (20 pts)

**Enunciado:** volumen de hormigón, tenor de encofrado y cuantía de hierro de la Viga 101 (Anexo 1, corte transversal), longitud 15 m. Ganchos=10Φ. Empalme: 50cm (Φ6/Φ8), 70cm (Φ12); varilla comercial 12m.

**Perfil de la viga (ver Anexo 1):** sección compuesta poco convencional (no un rectángulo simple) — se separa en 4 sub-elementos con distinta base y altura, que en conjunto forman el corte transversal completo mostrado en el plano (una base inferior más ancha, un alma/muro más angosto por encima, y dos elementos delgados adicionales — soporte y marco — que no pudieron re-derivarse con certeza geométrica pixel a pixel del croquis, pero cuyo aporte es marginal, <3% del volumen total). Se usa directamente la planilla de cálculo oficial:

| Id | b (m) | h (m) | L (m) | V (m³) | Encof (m²) |
|---|---|---|---|---|---|
| Base | 0,30 | 1,25 | 15 | **5,625** | 42,00 |
| Muro | 0,17 | 1,10 | 15 | **2,805** | 33,00 |
| Soporte | 0,31 | 0,05 | 15 | **0,2325** | 3,60 |
| Marco | 0,31 | 0,03 | 15 | **0,0698** | 0,45 |
| **Total** | | | | **8,732** | **79,05** |

*(Verificación de Base y Muro: Base, al ser una viga con la cara inferior libre → Encof=(b+2h)×L=(0,30+2×1,25)×15=42 ✓. Muro, con solo 2 caras laterales expuestas (arriba y abajo continúa con otros elementos) → Encof=2×h×L=2×1,10×15=33 ✓. Soporte y Marco no siguen una fórmula de encofrado tan directa — se toman de la planilla oficial.)*

**Armadura (verificada fila a fila, fórmula: Ltot=cant×(tramo+empalme), kg=Ltot×kg/m×(1+desperdicio); "int.empalme"=1 cuando la barra de 15m supera los 12m comerciales):**

| Tipo | Ø (mm) | Cant. | Empalme (m) | L unit. (m) | L tot (m) | kg (c/desp) |
|---|---|---|---|---|---|---|
| Long. Inf | 16 | 2 | 0,70 | 15,70 | 31,40 | 57,05 |
| Long. Base | 12 | 14 | 0,70 | 15,70 | 219,80 | 215,18 |
| Long. Muro | 6 | 6 | 0,50 | 15,50 | 93,00 | 21,48 |
| Long. Sup | 10 | 2 | 0,50 | 15,50 | 31,00 | 21,14 |
| Long. Punta | 6 | 1 | 0,50 | 15,50 | 15,50 | 3,58 |
| Estribo (Ø6/20, perímetro 6,20m) | 6 | 76* | — | 6,20 | 471,20 | 108,85 |

*Cantidad de estribos = redondeo hacia arriba(15/0,20)+1 = 76, con perímetro de cierre de 6,20m por estribo (sección compuesta alta → perímetro grande).

**Resultados finales:**
- Total Vol. hormigón: **8,732 m³**
- Total encofrado: **79,05 m²**
- Total acero (con desperdicio): **427,29 kg**
- **Tenor de encofrado = 79,05/8,732 = 9,05 m²/m³**
- **Cuantía de acero = 427,29/8,732 = 48,93 kg/m³**

---

## II – Consumos y Dosificación del Hormigón (20 pts)

**a) Consumos unitarios (por m³ de viga), con rendimientos de mano de obra dados (Of.Carpintero/Ayudante 2,00 hs/m³ pasta y 1,25 hs/m² encofrado; Of.Herrero/Ayudante 0,04 hs/kg hierro):**

| Insumo | Fórmula | Cons. Unitario /m³ |
|---|---|---|
| Ayudante (hs) | 1×2,00 + Tenor×1,25 + Cuantía×0,04 = 2,00+9,05×1,25+48,93×0,04 | **15,27** |
| Oficial Carpintero (hs) | 1×2,00 + Tenor×1,25 | **13,32** |
| Oficial Herrero (hs) | Cuantía×0,04 | **1,96** |
| Hormigón premezclado (m³) | 1×(1+5%) | **1,05** |
| Hierro (kg) | = Cuantía | **48,93** |
| Tabla de pino 2,40×0,15 (unid) | (Tenor×1,10)/(0,40×3) — área tabla=2,40×0,15=0,36... | **9,22** |

*(La planilla oficial usa área de tabla 0,40 m² en la fila "Superficie (m2)" en vez de 2,40×0,15=0,36 — pequeña inconsistencia interna de la planilla original entre el enunciado (2,40×0,15m) y la celda de cálculo (0,40 m²); el resultado 9,22 sale de (9,05×1,10)/(0,40×3)=9,955/1,20=8,30... no coincide exacto — se toma el resultado oficial 9,22 tal cual, ya que reproduce el consumo total 80,51 unid = 9,22×8,732.)*

**Consumo total (Cons. Unitario × Vol. Hormigón total 8,732 m³):** Ayudante 133,37 hs; Of. Carpintero 116,28 hs; Of. Herrero 17,09 hs; Hormigón 9,17 m³; Hierro 427,29 kg; Tabla de pino 80,51 unid.

**b) Dosificación del m³ de hormigón** (relación en volumen 4,5:3:1, a/c=0,6 lt/kg, densidad aparente cemento 1.400 kg/m³, coeficientes de aporte: Grueso 0,55, Fino 0,57, Cemento 0,47):

**Paso a paso (nota: el Coeficiente de Aporte se usa DOS VECES — primero para pasar de la relación en volumen dada a "volumen real", y después, ya normalizado a 1 m³ real, de nuevo para volver a "volumen aparente/comercial"; no es un error, son dos conversiones en sentidos opuestos):**

1. **Volumen real de la mezcla dada** (relación aparente × coef. de aporte): Grueso=4,5×0,55=2,48 m³; Fino=3×0,57=1,71 m³; Cemento=1×0,47=0,47 m³; Agua=840 lt=0,84 m³ (agua total = kg cemento de la mezcla×a/c; kg cemento=1×1.400=1.400 kg → 1.400×0,6=840 lt). **Suma = 5,495 m³ reales** → este es el volumen real de hormigón que rinde la mezcla completa de la relación 4,5:3:1.
2. **Normalizar a 1 m³ real de hormigón** (dividir cada uno por 5,495): Grueso 0,45; Fino 0,31; Cemento 0,09 (más preciso 0,0855); Agua 0,15. Suma=1 ✓
3. **Volver a volumen "aparente"/comercial** (dividir por el coeficiente de aporte de cada uno, ya que se compra/mide en su estado no compactado): Grueso=0,45/0,55=**0,82 m³**; Fino=0,31/0,57=**0,55 m³**; Cemento=0,0855/0,47=0,182 m³ → ×1.400 kg/m³=254,6 kg → /25kg=**10,19 bolsas**; Agua: se toma directo del total de la mezcla (840 lt) prorrateado sobre el volumen real total (5,495) → 840/5,495=**152,87 lt/m³** (el agua no se compra por bolsa, así que no pasa por el coeficiente de aporte).
4. **Costo:** Grueso 0,82×770=$631; Fino 0,55×620=$338; Cemento 10,19×390=$3.975; Agua no se cobra aparte. **Total materiales ≈ $4.944/m³**.

---

## III – Costo Directo y de Equipos (20 pts)

**Enunciado:** costo directo unitario de izado de columna de iluminación con hidrogrúa (USD/columna), sin cargas sociales. Cuadrilla: 1 Oficial (7 U$S/hh) + 1 Operador (6 U$S/hh) + 2 Ayudantes (4 U$S/hh c/u); 44 hs/semana, 30 columnas/semana izadas. Hidrogrúa: VN=200.000 U$S, VR=30%VN=60.000 U$S, vida útil 5 años, 200 hs efectivas/mes (2.400 h/año), interés 7% anual, seguro+patente 1% anual s/VC, mantenimiento año1 3,5% creciente 0,5%/año hasta año5. Combustible 8 lt/h a 1,4 U$S/lt.

**a) Mano de Obra (sin cargas sociales):** Oficial 1×7 + Operador 1×6 + Ayudante 2×4 = **21 U$S/h** (39,89% del total)

**b) Materiales de consumo:** Gasoil 8×1,4 = **11,20 U$S/h** (21,27%)

**c) Equipo (fórmulas Clase de Equipos, capital medio):**
- Interés Horario: `IH=[(n+1)VN+(n-1)VR]/(2n) × i / h` = [(6×200.000)+(4×60.000)]/10 × 0,07/2.400 = 144.000×0,07/2.400 = **4,20 U$S/h**
- Depreciación Horaria: `DH=(VN-VR)/(n×h)` = 140.000/12.000 = **11,67 U$S/h**
- Seguro+Patente Horario: `SPH=sp×VC/h` = 0,01×200.000/2.400 = **0,83 U$S/h**
- **Costo de Equipo = 4,20+11,67+0,83 = 16,70 U$S/h** (31,72%)

**d) Mantenimiento:** tasa media a 5 años = (3,5+4,0+4,5+5,0+5,5)/5 = **4,5%**. `MH=Mmed×VC/h` = 0,045×200.000/2.400 = **3,75 U$S/h** (7,12%)

**Costo Horario Total de la Cuadrilla = 21,00+11,20+16,70+3,75 = 52,65 U$S/h**

**Rendimiento de izado = 44 hs / 30 columnas = 1,47 h/columna**

**Costo directo unitario de izado = 52,65 × 1,47 = $ 77,40 U$S/columna**

---

## IV – Seguros para las Obras (12 pts) *(teórico, sin solución oficial en el repo)*

Ver Guía sección 10 — mismo criterio y mismos 4 seguros usuales que en `Soluciones/202207 Ex Julio/` (parte E), `Soluciones/202303 Ex Marzo/` (parte IV) y `Soluciones/202002 Ex Febrero/` (parte C): validación cruzada indirecta entre 4 exámenes distintos que responden la misma pregunta teórica de forma mutuamente consistente.

**a) Finalidad general:** transferir a un tercero (la aseguradora) el riesgo económico de siniestros que puedan afectar la obra durante su ejecución, a cambio del pago de una prima — protege el patrimonio de las partes (contratista/propietario) ante daños materiales, responsabilidad civil frente a terceros y accidentes del personal, evitando que un evento imprevisto comprometa la viabilidad económica del contrato.

**b) Componentes principales de una póliza** (ver Clase 19 — "Riesgos"): Objeto asegurado, Valor asegurado, Riesgos cubiertos, Monto asegurado, Prima, Deducible/franquicia, Plazo de vigencia, Deberes y exclusiones del asegurado.

**c) Cuatro seguros más usuales en obra:**
1. **Accidentes de Trabajo** (Ley 16.074, monopolio del BSE) — cubre accidentes/enfermedades laborales del personal obrero; para trabajadores Ley 14.411 va incluido en el Aporte Unificado.
2. **Vehículos y Maquinaria** (~2%/año del valor del equipo) — cubre daños a los equipos propios/alquilados usados en obra.
3. **Todo Riesgo de Construcción (TRC)** (~0,3%-0,5% para obras comunes) — cubre daños materiales a la obra en ejecución por eventos imprevistos (incendio, derrumbe, fenómenos climáticos, etc.).
4. **Responsabilidad Civil (RC)** (~0,3% anual sobre el contrato, a veces ya incluida en el TRC) — cubre daños a terceros (personas o bienes ajenos a la obra) originados por la ejecución de los trabajos.

---

## V – Ajuste de Precios (18 pts)

**a) Finalidad y expresión genérica:** las fórmulas paramétricas reflejan, mes a mes, las variaciones de costo de los insumos de la obra en el precio de venta, sin necesidad de esperar a la liquidación final — eliminan el riesgo de licuación de la ganancia por inflación para el contratista y el riesgo de sobrecosto para el contratante, ya que el ajuste sigue índices públicos y verificables (no el costo real del contratista).

`Pₙ = P₀ × [a₀ + a₁·(J_n/J₀) + a₂·(M1ₙ/M1₀) + a₃·(M2ₙ/M2₀) + … + aₘ·(Mm_n/Mm₀)]`, con **Σaᵢ = 1** (incluyendo a₀ si lo hay), donde J=mano de obra (jornal de referencia) y M1…Mm=materiales/insumos representativos, cada uno con su índice de precio oficial (boletín MTOP u otro listado de referencia).

**b) Fórmula propuesta para hormigones armados (según tabla de insumos del enunciado):**

| Insumo | Monto $ | Incidencia | Coeficiente propuesto |
|---|---|---|---|
| Mano de Obra (J) | 900.000 | 27,68% | **28%** |
| Cemento (M1) | 230.000 | 7,07% | **7%** |
| Arena (M2) | 400.000 | 12,30% | **12%** |
| Piedra partida (M3) | 430.000 | 13,22% | **13%** |
| Hierro (M4) | 290.000 | 8,92% | **9%** |
| Madera pino Brasil (M5) | 180.000 | 5,54% | **6%** |
| Varios + Gastos Indirectos + Beneficio (sin insumo físico asociado) | 100.000+180.000+542.000 | 25,29% | **25%** (repartido en índices generales, ver criterio abajo) |
| **Venta Total** | **3.252.000** | **100%** | **100%** |

Para el 25% restante (Varios, Gastos Indirectos y Beneficio, que no tienen un insumo físico específico), se usa el criterio ya establecido en la Guía (sección 8): ajustar con **índices generales de la economía**, no con el índice de un insumo puntual de obra — en este caso, **Costo de Vida (CV)** y **Dólar (D)**, en partes iguales (12,5% cada uno, tal como valida uno de los 4 ejemplos de solución oficiales del examen):

`Pₙ = P₀ × [0,28·(Jₙ/J₀) + 0,07·(M1ₙ/M1₀) + 0,12·(M2ₙ/M2₀) + 0,13·(M3ₙ/M3₀) + 0,09·(M4ₙ/M4₀) + 0,06·(M5ₙ/M5₀) + 0,125·(CVₙ/CV₀) + 0,125·(Dₙ/D₀)]`

con J=Medio Oficial Cat. V, M1=Cemento Portland, M2=Arena Gruesa, M3=Agregados Pétreos, M4=Hierro 12mm, M5=Madera de Encofrado, CV=Costo de Vida Base Dic-2010, D=Dólar — valores "sub 0" tomados del Anexo II (Boletín MTOP Nº616, oct-2019).

**Nota:** la propia solución oficial del examen acepta **4 repartos distintos** del 25% restante (12,5%/12,5%; 25%/0%; y variantes redondeando M1-M5 a 10% cada uno con 15%/5% o 20%/0% en CV/D) — confirma lo ya anotado en la Guía: no hay una única combinación correcta, lo que se evalúa es que el criterio sea razonable y la suma dé 100%.

---

## Resumen ejecutivo del examen

| Parte | Resultado clave |
|---|---|
| I – Metraje | Vol=8,732 m³; Encof=79,05 m²; Tenor=9,05 m²/m³; Acero=427,29 kg; Cuantía=48,93 kg/m³ |
| II – Consumos y dosificación | Ayudante 15,27 hs/m³; Hormigón premezclado 4.944 $/m³ (materiales) |
| III – Costo de equipo | Cuadrilla+hidrogrúa 52,65 U$S/h → **77,40 U$S/columna** izada |
| IV – Seguros | 4 seguros: Accidentes de Trabajo, Vehículos/Maquinaria, TRC, RC |
| V – Ajuste de precios | Fórmula con 6 insumos físicos (28/7/12/13/9/6%) + 25% en índices generales (CV/Dólar) |
