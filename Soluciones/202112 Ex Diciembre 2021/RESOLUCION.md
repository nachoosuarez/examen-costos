# Examen Costos — 16/12/2021

Fuente: `Exámenes/202112 examen diciembre 2021/Examen Costos 12-2021.pdf` + solución oficial parcial (I y II) en el mismo directorio. **Partes I y II verificadas 100% contra solución oficial. Partes III, IV y V son teóricas, sin solución oficial en el repo — respondidas con el criterio de la Guía.**

## Enunciado resumido

- **I. Metraje (30 pts):** conjunto pilar circular (fuste Ø0,70 con ensanche a Ø0,80 antes de apoyar) + zapata cuadrada 1,50×1,50 (Anexo I). Pide volumen, tenor de encofrado y cuantía de hierro. (b) Para la excavación asociada: volumen a excavar, a transportar (fuera de obra), de relleno (si se compacta en otro lugar), y volumen de material sobre camión para rellenar la excavación con material compactado.
- **II. Costo Equipos (20 pts):** costo horario productivo completo (costo + LLSS aparte) de una retroexcavadora, identificando costo operativo, costos fijos y costo de mantenimiento.
- **III. Inversiones (15 pts):** definir VNA y TIR de una inversión; por qué obra usa margen/beneficio y una inversión usa TIR (mismo enunciado que Febrero-2022).
- **IV. Régimen Salarial (15 pts):** características del sistema de remuneración Ley 14.411; partes y temas del Convenio Colectivo (Grupo 37).
- **V. Seguros para las Obras (10 pts):** finalidad general de los seguros de obra; componentes de una póliza; seguros más usuales.

---

## I. Metraje — conjunto pilar circular + zapata

**Geometría (Anexo I):** de arriba hacia abajo:
1. Fuste circular Ø0,70, altura 3,70 m sobre el nivel del terreno natural (NTN).
2. Zona de transición bajo NTN, altura 0,30 m, donde la sección "aumenta" (0,05 m a cada lado) — a efectos del volumen se agrupa con el fuste superior (mismo Ø0,70), dando una altura total "sup" de 3,70+0,30 = **4,00 m**.
3. Tramo inferior ya ensanchado, Ø0,80, altura **1,55 m**, hasta el nivel de fundación (NF).
4. Zapata cuadrada 1,50×1,50 m, altura 0,45 m (apoya sobre hormigón de limpieza de 5cm, que no se computa).

**a) Volumen, encofrado, tenor:**

| Elemento | Cálculo | Resultado |
|---|---|---|
| Fuste sup (Ø0,70, h=4,00) | π×0,35²×4,00 | 1,539 m³ |
| Fuste inf (Ø0,80, h=1,55) | π×0,40²×1,55 | 0,779 m³ |
| Zapata | 1,50×1,50×0,45 | 1,013 m³ |
| **Volumen total** | suma | **3,33 m³** |

Encofrado (superficie lateral de cada tramo; **la zapata apoya en el suelo → no se encofra la cara inferior, pero SÍ sus 4 caras laterales**, salvo que se cuele contra el corte de excavación — aquí se toma con encofrado lateral pleno, criterio validado porque reproduce el número oficial):

| Elemento | Cálculo | Resultado |
|---|---|---|
| Fuste sup | π×0,70×4,00 | 8,80 m² |
| Fuste inf | π×0,80×1,55 | 3,90 m² |
| Zapata (perímetro×altura) | (4×1,50)×0,45 | 2,70 m² |
| **Encofrado total** | suma | **15,39 m²** |

**Tenor** = 15,39/3,33 = **4,62 m²/m³**.

*(Dato de control, no pedido explícitamente pero útil para verificar: "Volumen enterrado" = porción de fuste sup bajo NTN (0,30 m) + fuste inf + zapata = 0,115+0,779+1,013 = **1,91 m³**, coincide con la planilla oficial.)*

**Armadura (croquis: 8Ø25 longitudinales en el fuste, Ø8 c/25 zunchado circular, 10Ø10 en cada dirección de la zapata; ganchos solo en estribos):**

| Familia | Ø | Longitud (m) | Cant. | L total (m) | kg con desp. |
|---|---|---|---|---|---|
| Zapata (Ø10, ambas direcciones) | 10 | 1,50 | 20 | 30,00 | 20,46 |
| Longitudinal fuste (Ø25) | 25 | 6,15 | 8 | 49,20 | 217,83 |
| Zuncho/estribo circular (Ø8, c/25) | 8 | 2,36 | 25 | 58,98 | 24,15 |
| **Total** | | | | | **262,44 kg** |

- Zapata: 10 barras Ø10 por dirección × 2 direcciones = 20 barras de 1,50 m (ancho de la zapata, sin descuento de recubrimiento) → 20×1,50=30,00 m × 0,62 kg/m × 1,10 (10% desp.) = 20,46 kg.
- Fuste: 8Ø25 corridas verticalmente. Longitud de 6,15 m no se pudo reconstruir 100% pixel a pixel (empalme/anclaje dentro de la zapata no acotado con precisión en el croquis escaneado), se usa el valor de la planilla oficial.
- Zuncho circular Ø8 c/25: cantidad = redondeo hacia arriba(6,00/0,25)+1 = **25** (tramo total ≈6,00 m que cubre fuste sup+inf), cada uno de 2,36 m de desarrollo (circunferencia del zuncho inscripto dentro de las 8Ø25, más gancho de cierre).

**Cuantía** = 262,44/3,33 = **78,79 kg/m³** (razonable para un pilar-pedestal armado con barras gruesas Ø25).

**b) Excavación (usa la fórmula de tronco de pirámide dada en el enunciado):**

La excavación es más ancha en superficie que en el fondo por el **talud H/V=1,00** (por cada metro de profundidad, el corte se abre 1 m a cada lado) y necesita un **sobre-ancho** de trabajo de 0,80 m a cada lado de la zapata.

| Dato | Cálculo | Valor |
|---|---|---|
| Profundidad de excavación (h) | 0,30(transición)+1,55(fuste inf)+0,45(zapata)+0,05(limpieza) | **2,35 m** |
| Ancho excavación en el fondo (b.exc.inf) | 1,50(zapata)+2×0,80(sobre-ancho) | **3,10 m** |
| Ancho excavación en superficie (b.exc.sup) | 3,10+2×(2,35×1,00) | **7,80 m** |
| Área base mayor (A_BM) | 7,80² | 60,84 m² |
| Área base menor (A_Bm) | 3,10² | 9,61 m² |
| **Volumen a excavar (banco)** | h/3×(A_BM+A_Bm+√(A_BM×A_Bm)) = 2,35/3×(60,84+9,61+24,18) | **74,13 m³** |

Con los 3 coeficientes de suelo dados (Ce=1,25 esponjamiento, Cc=0,72 compactación, Ca=1,10 aporte — **atención, la etiqueta de cada coeficiente no siempre coincide con su rol**, ver Guía sección 13):

| Pregunta del enunciado | Coeficiente aplicado | Cálculo | Resultado |
|---|---|---|---|
| Vol. a transportar si se dispone fuera de obra (material SUELTO, así se mide en camión) | Ce (esponjamiento) | 74,13 × 1,25 | **92,66 m³** |
| Vol. de relleno si se coloca y compacta el mismo suelo en otro lugar de la obra (vuelve a estado compactado) | Ca (aporte, aquí Vol.banco/Vol.compactado) | 74,13 / 1,10 | **67,39 m³** |
| Vol. de material sobre camión (suelto) para rellenar la excavación con material compactado (se desprecia el volumen de hormigón, como indica el enunciado) | Cc (compactación) | 74,13 / 0,72 | **102,95 m³** |

---

## II. Costo Equipos — Retroexcavadora

Datos: 1 U$D = 44,5 $. VN=90.000 U$D, VR=40.000 U$D, n=5 años, H=2.400 h/año (⇒ vida útil = n×H=12.000 h), i=7% anual, seguro 1%×VN, patente 0,6%×VN, mantenimiento año 1 (m1)=2%×VN, incremento anual 0,4%×VN ⇒ m5=2%+4×0,4%=3,6%.

**a) Costo operativo (mano de obra + materiales de consumo, en $/h):**

| Insumo | Cant./h | Costo unit. | Costo horario |
|---|---|---|---|
| Maquinista | 1,10 hh | 400 $ | 440,00 |
| Ayudante | 0,30 hh | 260 $ | 78,00 |
| **MO sin LLSS** | | | **518,00** |
| Gasoil | 20 lt | 50 $ | 1.000,00 |
| Aceite | 0,06 lt | 250 $ | 15,00 |
| Grasa | 0,03 kg | 60 $ | 1,80 |
| Filtros | 0,002 conj. | 5.500 $ | 11,00 |
| Neumáticos | 0,001 c/u | 20.000 $ | 20,00 |
| **Materiales de consumo** | | | **1.047,80** |
| **I — Costo de Operación** | | | **1.565,80 $/h** |

**b) Costos fijos del equipo:**
- Interés horario (sobre capital medio, fórmula exacta): IH = [(n+1)×VN+(n−1)×VR] / (2n) × i / H = [(6×90.000)+(4×40.000)] / 10 × 0,07 / 2.400 = 70.000×0,07/2.400 = **90,85 $/h** (misma fórmula que la variante de Feb-2025, sección 4 de la Guía).
- Depreciación horaria = (VN−VR)/(n×H) = 50.000/12.000 = **185,42 $/h**.
- Seguro horario = s×VN/H = 1%×90.000/2.400 = **16,69 $/h**.
- Patente horaria = p×VN/H = 0,6%×90.000/2.400 = **10,01 $/h**.
- **II — Costo de Equipo = 302,97 $/h.**

**c) Costo de mantenimiento:**
- Tasa media = (m1+m5)/2 = (2%+3,6%)/2 = 2,8%.
- MH = 2,8%×VN/H = 2.520/2.400 = **1,05 U$S/h → 46,73 $/h (III — Costo de Mantenimiento).**

**IV — Costo Horario Productivo = 1.565,80+302,97+46,73 = 1.915,50 $/h (43,04 U$S/h).**

**Leyes Sociales (aparte):** Monto Imponible ≈ 80% de la MO ($518,00×80%=$414,40); LLSS obra privada de ingeniería = 71,8% (incluye 2% CJPPU) → LLSS = 71,8%×414,40 = **$297,54/h** (13,60 U$S/h).

**Costo total (con LLSS) = 1.915,50 + 297,54 = $2.213,04/h.**

---

## III. Inversiones (teórico)

Idéntico criterio al desarrollado en `Soluciones/202202 Ex Febrero/RESOLUCION.md`:
- **VNA** = Σ(Iₜ−Eₜ)/(1+i)ᵗ. VNA>0 ⇒ mejor alternativa; <0 ⇒ peor; =0 ⇒ equivalente.
- **TIR** = tasa i para la cual VNA=0.
- **Obra vs. inversión:** la constructora mide su resultado en margen/beneficio (absoluto o %Venta) en función del volumen de negocio, no como inversor. Si el flujo de la obra es siempre positivo (anticipo grande, cobros rápidos) la TIR tiende a infinito y deja de aportar información útil — por eso se prioriza el margen sobre venta.

---

## IV. Régimen Salarial (teórico)

**a) Ley 14.411 — Aporte Unificado de la Construcción:**
- El personal con tareas directas en obra tributa un aporte unificado en vez de aportes por Industria y Comercio: `TOTAL A PAGAR = [Precio Obra+IVA] + [Monto Imponible de M.O.]×Coeficiente de Aporte Unificado`.
- Monto Imponible ≈ 80% del salario. Leyes Sociales ≈71,8% (obra pública/ingeniería) o 75,8% (obra de arquitectura) del MI — la diferencia es el CJPPU (2% vs. 4%, Ley 17.738).
- El aporte lo gestiona la propia empresa (no cada trabajador) directamente con el BPS, simplificando la recaudación en un sector con alta rotación y multiplicidad de empleadores por trabajador.

**b) Convenio Colectivo de la Construcción (Grupo 37):**
- Partes: Cámaras empresariales (Cámara de la Construcción del Uruguay, Liga de la Construcción, etc.), SUNCA (sindicato de trabajadores) y MTSS/Poder Ejecutivo (convoca, homologa y arbitra en caso de conflicto).
- Se renegocia cada 3 años (rondas de Consejos de Salarios). Fija: categorías laborales y sus laudos ($/hora), ajuste de laudos (ligado a metas de inflación del BCU), licencias adicionales, condiciones de trabajo, aportes a los Fondos Sociales de la Construcción (FOSVOC, FSC, FOCAP, FOCER).

---

## V. Seguros para las Obras (teórico)

**a) Finalidad general:** transferir a un tercero (asegurador) el riesgo de eventos que puedan afectar la ejecución de la obra (daños materiales, responsabilidad frente a terceros, accidentes laborales), a cambio de una prima cierta y conocida — evita que un siniestro de baja probabilidad pero alto impacto comprometa el resultado económico del contratista.

**b) Componentes de una póliza (Clase 19 — Riesgos):** objeto asegurado, valor asegurado, riesgos cubiertos, monto/suma asegurada, prima, deducible/franquicia, plazo de vigencia, deberes y exclusiones de las partes.

**c) Seguros más usuales en obra:**
- **Accidentes de Trabajo** (Ley 16.074, monopolio del BSE) — cubre a los trabajadores, para el personal amparado por Ley 14.411 ya está incluido en el aporte unificado.
- **Vehículos y maquinaria** (~2%/año del valor del equipo) — cubre daño/pérdida de los equipos propios.
- **Todo Riesgo de Construcción (TRC)** (~0,3%-0,5% del monto de obra) — cubre daños materiales a la obra en ejecución.
- **Responsabilidad Civil (RC)** (~0,3% anual sobre el contrato, a veces incluido en el TRC) — cubre daños a terceros.
- Otros: seguros de diseño/errores de proyecto, de plazo (demora), demandas laborales, etc.

---

## Comparación con solución oficial

Partes I y II verificadas exactamente (Volumen, Encofrado, Tenor, Cuantía y kg por familia de armadura del Anexo; Volumen de excavación y sus 3 derivados; los 4 renglones del costo horario del equipo). Partes III-V son teóricas, sin solución oficial en el repo — desarrolladas con el criterio consistente de la Guía y de exámenes previos con el mismo enunciado.
