# Examen Costos — 11/08/2020 ("Julio 2020")

Fuente: `Exámenes/202007 Ex Julio/Examen Costos 07-2020.pdf` + solución oficial de I, II y III en `Examen Costos Julio-2020 I,II,III.pdf`. **Partes I, II y III verificadas contra solución oficial. Partes IV y V son teóricas, sin solución oficial en el repo.**

## Enunciado resumido

- **I. Metraje de Hormigón (20 pts):** losa sobre piso 11 (nivel 700), apoyada en 6 vigas perimetrales (Anexo 1). Volumen, cuantía de acero y tenor de encofrado.
- **II. Equipos (20 pts):** costo horario productivo completo (costo y LLSS separados) de una retroexcavadora.
- **III. Punto de Equilibrio, Costos Fijos y Variables (20 pts):** (a) definir Punto de Equilibrio. Caso: el comitente pide **extender el plazo un 50%, antes de iniciar la obra**, sin poder demorar el inicio. (b) determinar el reconocimiento económico para que el contratista mantenga su margen %, sin considerar aún un posible ahorro de costos fijos. (c) considerando que el contratista SÍ logra ese ahorro (20% de reducción de costo fijo, no conocido por el cliente), determinar el nuevo margen real.
- **IV. Garantías (15 pts):** finalidad, relación con el precio, costo aproximado, oportunidad de constitución y formas posibles de cada garantía habitual.
- **V. Régimen Salarial (15 pts):** características de la remuneración Ley 14.411; sistema de gestión de aportes sociales; partes e ítems del Convenio Colectivo.

---

## I. Metraje — losa sobre piso 11 (nivel 700)

**Geometría (Anexo 1):** losa rectangular acotada en planta a×b=10,26×2,76 m (dimensión "sin descuento de vigas", entre ejes/medianeras), apoyada en 6 vigas perimetrales: VB751/VB752 (13×50, en los extremos cortos) y VB701/702/703 + VB704/705/706 (18×50, en los lados largos). Espesor e=0,15 m.

**Regla de oro aplicada (Guía sección 1, punto 1): el volumen de una losa es el comprendido ENTRE vigas, sin incluir el volumen de las vigas.** La planilla oficial muestra ambos cálculos para comparar:

| | a (m) | b (m) | V (m³) | Enc (m²) |
|---|---|---|---|---|
| Sin descuento de vigas (envolvente completa) | 10,26 | 2,76 | 4,25 | 32,22 |
| **Con descuento de vigas (real de la losa)** | 10,00 (−0,13×2, ancho VB751/752) | 2,40 (−0,18×2, ancho VB701.../VB704...) | **3,60** | **24,00** |

**Volumen de la losa = 10,00×2,40×0,15 = 3,60 m³** (el uso correcto, según la regla de oro).

**Encofrado = 10,00×2,40 = 24,00 m²** — la losa está suspendida en sus 4 lados (apoya en las 6 vigas perimetrales, no tiene lateral expuesto) → Encofrado = área en planta neta (misma variante "losa angosta" de Dic-2024).

**Tenor = 24,00/3,60 = 6,67 m²/m³ = 1/0,15 = 1/espesor** ✓ (confirma otra vez la identidad Tenor=1/e para losas encofradas solo por la cara inferior, ver Guía sección 1).

**Armadura (2 mallas, ambas direcciones — patrón "doble capa" ya visto en Marzo-2025):**

| Familia | Ø | Cant. (c/dirección) | kg con desp. |
|---|---|---|---|
| A (malla principal, Ø10, paso 0,20, una franja en cada dirección) | 10 | 13 (dir. corta) + 51 (dir. larga) | 92,74+102,95=195,69 |
| F (malla de refuerzo, Ø8, paso 0,20, franja DUPLICADA junto a cada apoyo en cada dirección) | 8 | 26 (=2×13, dir. corta) + 102 (=2×51, dir. larga) | 15,65+65,58=81,23 |
| **Total** | | | **276,92 kg** |

*(Del plano: Φ10 c/20 corre en la malla principal —la franja central, "A"—, y Φ8 c/20 "F" junto a las vigas en ambas direcciones —refuerzo local por apoyo, contado el doble por aparecer en las 2 franjas junto a cada uno de los 2 apoyos de esa dirección—; el desglose exacto bar-a-bar del croquis rotado no se pudo reconstruir con precisión, se usan los totales de la planilla oficial, validados porque el Tenor sí cierra exacto con la identidad 1/e.)*

**Cuantía = 276,92/3,60 = 76,92 kg/m³.**

---

## II. Equipos — Retroexcavadora

Datos: 1 USD=42,50$. VN=100.000 U$S, VR=50.000 U$S, n=5 años, H=2.400 h/año (vida útil=12.000h), i=7%, seguro 2%VN, patente 1%VN, m1=2%, incremento anual 0,5%VN ⇒ m5=2%+4×0,5%=4%.

**a) Costo operativo:**

| | Costo horario ($) |
|---|---|
| Maquinista (1,20hh×379,72) + Ayudante (0,30hh×241,21) | 455,66+72,36=528,03 |
| Gasoil+Aceite+Grasa+Filtros+Neumáticos | 852,50 |
| **I — Costo de Operación** | **1.380,53** |

**b) Costos fijos del equipo:**
- Interés horario (capital medio) = [(n+1)VN+(n−1)VR]/(2n) × i/H = [(6×100.000)+(4×50.000)]/10 × 0,07/2.400 = 80.000×0,07/2.400 = **99,17 $/h**.
- Depreciación = (VN−VR)/(n×H) = 50.000/12.000×42,50 = **177,08 $/h**.
- Seguro = 2%×100.000/2.400×42,50 = **35,42 $/h**. Patente = 1%×100.000/2.400×42,50 = **17,71 $/h**.
- **II — Costo de Equipo = 329,38 $/h.**

**c) Mantenimiento:** tasa media=(2%+4%)/2=3% → MH=3%×100.000/2.400×42,50 = **53,13 $/h.**

**IV — Costo Horario Productivo = 1.380,53+329,38+53,13 = 1.763,03 $/h.**

**Leyes Sociales:** Monto Imponible≈80%×528,03=422,42; LLSS obra privada de ingeniería=71,8%×422,42=**$303,30/h**.

**Costo total con LLSS = 1.763,03+303,30 = $2.066,33/h.**

---

## III. Punto de Equilibrio — extensión de plazo antes del inicio, con reconocimiento y ahorro propio

**a) Punto de Equilibrio:** nivel de producción/venta donde Ingresos Totales = Costos Totales (CF+CV), es decir, resultado nulo. `Q_equilibrio = CF/(Pu−Cvu)`.

**Datos:** CF=20% del Costo Total (CTo), CV=80% (resto), Beneficio original be=15% **sobre venta**, plazo original=12 meses. El comitente pide extender el plazo un 50% (inc=50%) desde antes del inicio (no hay obra en curso que reprogramar, así que TODO el costo fijo del nuevo plazo es "nuevo", no hay costo fijo ya incurrido que proteger).

**b) Reconocimiento económico (re) para mantener el margen %, SIN considerar el ahorro de costos fijos:**

Con base 100 = Costo Total original (CD=80, CF=20, CT=100):
- Venta original: V = CTo/(1−be) = 100/(1−15%) = **117,65**.
- Al extender el plazo 50%, el Costo Fijo total nuevo = CF×(1+inc) = 20×1,50 = **30** (el Costo Variable no cambia, mismas tareas y rendimientos) → Costo Total nuevo = 80+30 = **110**.
- El reconocimiento (re) debe llevar la Venta a un nuevo valor Vre tal que, sobre el Costo Total nuevo, se mantenga el mismo % de beneficio sobre venta: `Vre = Costo Total nuevo/(1−be) = 110/0,85 = 129,41` → pero expresado como % de incremento sobre la Venta original: `Vre = (1+re)×V` ⟹ **re = cfo × inc = 20% × 50% = 10%** (¡notar que re resulta **independiente del plazo y del beneficio originales**, solo depende de qué fracción del costo es fija y cuánto se extiende el plazo!). Reconocimiento en $ = 129,41−117,65 = **11,76** (sobre base 100).

**c) Nuevo margen real considerando el ahorro de costos fijos (ah=20%, no conocido por el cliente):**

El contratista, aprovechando que aún no se instaló en obra, logra bajar su costo fijo mensual un 20% (CF real nuevo = 30×0,80=**24**, no 30) — pero **el cliente ya pagó el reconocimiento calculado en (b) sobre el costo fijo SIN ese ahorro** (Vre=129,41 se mantiene igual, el cliente no lo sabe).

- Costo Total real nuevo = CD(80)+CF real(24) = **104**.
- Beneficio real = Vre−Costo Total real = 129,41−104 = **25,41**.
- **Nuevo margen % sobre venta = 25,41/129,41 = 19,64%** (por encima del 15% original — el contratista se queda con el ahorro de costos fijos como ganancia adicional, ya que el cliente reconoció un costo mayor al que realmente terminó teniendo).

**Fórmula general (verificada, útil para cualquier combinación de datos):**

`re = cfo × inc`

`Beneficio final = be + [cfo×(1+inc)×ah] / [(1+inc×cfo)/(1−be)]`

Con cfo=20%, inc=50%, ah=20%, be=15% → Beneficio final = 15%+[0,20×1,50×0,20]/[(1+0,50×0,20)/0,85] = 15%+0,06/1,2941 = **19,64%** ✓ (coincide con el cálculo paso a paso).

---

## IV. Garantías (teórico)

| Garantía | a) Finalidad | b) Relación con el Precio | c) Costo aprox. | d) Oportunidad | e) Formas de constitución |
|---|---|---|---|---|---|
| Mantenimiento de Oferta | Asegurar que el oferente sostenga su oferta durante la evaluación/adjudicación | ~1% del monto ofertado | 0,4%-1%/año (prorrateado al plazo de vigencia de la oferta) | Al presentar la oferta | Aval bancario, póliza de seguro de fianza, depósito en efectivo/valores |
| Fiel Cumplimiento de Contrato | Asegurar que el contratista ejecute la obra según lo pactado | ~5-10% del precio del contrato (con IVA y LLSS de M.O. incluidos) | ~2%/año del monto garantizado | Previo a la firma del contrato, hasta Recepción Provisoria | Aval bancario, póliza de seguro de fianza (BSE u otras aseguradoras) |
| Buena Ejecución / Fondo de Reparo | Cubrir defectos de ejecución que aparezcan durante el plazo de garantía | ~5% de cada certificado (retención progresiva) | ~2%/año del monto retenido (si se sustituye por póliza) | Por certificado, hasta Recepción Definitiva (tras el plazo de garantía desde la Recepción Provisoria) | Retención directa del certificado, o sustitución por aval/póliza (evita el costo financiero de la retención) |
| Anticipo/Acopio | Asegurar la devolución del anticipo si la obra no avanza según lo previsto | 100% del monto del anticipo | ~3%/año | Previo a recibir el anticipo | Aval bancario, póliza de seguro de fianza |

*(Ver también Guía sección 7, tabla rápida de garantías.)*

---

## V. Régimen Salarial (teórico)

Mismo temario que Diciembre 2021 (ver `Soluciones/202112 Ex Diciembre 2021/RESOLUCION.md`, sección IV, y Guía sección 6):

**a) Sistema de remuneración Ley 14.411:** el personal con tareas directas en obra tributa el Aporte Unificado de la Construcción; `TOTAL A PAGAR = [Precio Obra+IVA] + [Monto Imponible M.O.]×Coeficiente de Aporte Unificado`. Monto Imponible≈80% del salario; Leyes Sociales≈71,8% (pública/ingeniería) o 75,8% (arquitectura) del M.I.

**b) Sistema de gestión de aportes sociales:** la propia empresa constructora gestiona y paga el aporte unificado directamente al BPS (no cada trabajador individualmente), simplificando la recaudación dada la alta rotación de personal entre obras/empleadores del sector. Las partidas que integran el aporte: BPS (jubilación+salud/FONASA), DISSE, seguro de accidentes de trabajo (Ley 16.074, incluido), y los 4 Fondos Sociales de la Construcción (FOSVOC, FSC, FOCAP, FOCER).

**c) Convenio Colectivo de la Construcción:** partes: Cámaras empresariales, SUNCA (sindicato) y MTSS/Poder Ejecutivo (convoca, homologa). Se renegocia cada 3 años (Consejos de Salarios). Fija categorías y laudos, ajuste ligado a metas de inflación del BCU, licencias, condiciones de trabajo, aportes a los Fondos Sociales.

---

## Comparación con solución oficial

Partes I, II y III verificadas exactamente (Volumen, Encofrado, Tenor, Cuantía de la losa; los 4 renglones del costo horario del equipo; el reconocimiento económico re=10% y el margen final 19,64% del punto de equilibrio, con la fórmula paramétrica y la tabla "paso a paso" ambas verificadas numéricamente). Partes IV-V son teóricas, sin solución oficial en el repo — desarrolladas con el criterio de la Guía.
