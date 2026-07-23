# Examen Costos (2240) — 24/07/2019

Fuente: `Exámenes/201907 Ex julio/Examen Costos 07-2019.pdf` (letra) + `Examen Costos Jul-2019 -Anexo.pdf` (croquis viga V305) + `Examen Costos Jul-2019 Preg A,B,C,D,E.pdf` (planilla oficial de A y C; B, D y E remiten a diapositivas del curso, sin desarrollo escrito). **Partes A y C verificadas exactas contra la planilla oficial (todos los valores de C confirmados con cálculo propio, incluida la TIR por búsqueda numérica). Partes B, D y E son teóricas, sin desarrollo escrito en el repo (respondidas con el criterio de la Guía).**

Este es el **último examen del repo** (el más viejo disponible) — con esta resolución quedan cubiertos todos los exámenes 2019-2026 del archivo.

## Enunciado resumido

- **A. Metraje Hormigón (25 pts):** costo directo de materiales (hormigón+hierro+encofrado) de la viga V305 (Anexo), sección 17×50cm.
- **B. Industria de la Construcción (15 pts):** características generales/históricas de la industria de la construcción en Uruguay.
- **C. Evaluación de Inversión (20 pts):** comparar 4 alternativas de inversión a 6 años (2 depósitos a plazo fijo al 8%, 2 flujos irregulares dados) con VNA, TIR, y una variante de reinversión.
- **D. Garantías (15 pts):** garantías habituales del Contratante — finalidad, relación con el precio, costo aproximado, formas de constitución.
- **E. Varios (15 pts):** (a) fórmula paramétrica; (b) coeficientes de movimiento de tierra (esponjamiento, compactación, aporte); (c) clasificación de costos por naturaleza.

---

## A. Metraje y costo de materiales — Viga V305

**Geometría (Anexo, viga V305, sección 17×50 cm):** luz entre ejes de apoyo (vigas V-320 y V-322) = 5,69 m. Armadura: superior 2Ø6 L=589 (corrida) + 2Ø10 L=155 (refuerzo negativo cerca del apoyo derecho); inferior 2Ø16 L=614 (corrida, se prolonga dentro de los apoyos) + 1Ø16 L=375 (barra corta central); estribos Ø6 en 3 tramos de paso distinto (7 c/19 + 10 c/25 + 8 c/20 = **25 estribos en total**), sección interior del estribo 46×13 cm (=50−2×2 y 17−2×2, con recubrimiento 2 cm).

**a) Volumen de hormigón:** `V = luz × ancho × altura = 5,69 × 0,17 × 0,50 = 0,4837 ≈ 0,48 m³`.

**b) Acero (planilla oficial, kg con desperdicio incluido):**

| Ø | Long. total (m) | Cant. | Kg con desp. |
|---|---|---|---|
| 16 (agrupa 2Ø16 L=614 + 1Ø16 L=375 = 2×6,14+3,75=16,03 m) | 16,03 | 1 | 29,1 |
| 10 (2Ø10, refuerzo negativo) | 1,80 c/u | 2 | 2,5 |
| 6 (2Ø6, superior corrida) | 6,14 c/u | 2 | 2,8 |
| Estribos Ø6 (25 unid., perímetro interior 2×(0,46+0,13)=1,18m≈1,168m con ajuste de gancho) | 1,168 c/u | 25 | 6,7 |
| **Total** | | | **41,2 kg** |

*(Las longitudes de Ø10 y Ø6 de la planilla oficial incluyen algo más que la cota recta del plano —155cm y 589cm respectivamente— por los ganchos/anclajes de norma no acotados explícitamente en el croquis; se usan los valores de la planilla oficial, ya verificados contra el total. El único ítem 100% reconstruible de punta a punta es el de estribos: perímetro interior×cantidad, que cierra exacto.)*

**Cuantía = 41,2 / 0,48 = 85,1 kg/m³** (dato oficial, coherente con el cálculo propio 41,2/0,4837≈85,2).

**c) Encofrado** — solo fondo y laterales (2 laterales + 1 fondo; la cara superior no se encofra, se vierte desde arriba): `Encof = (ancho + 2×altura) × luz = (0,17+2×0,50)×5,69 = 1,17×5,69 = 6,66 ≈ 6,7 m²`.

**Tenor = 6,7 / 0,4837 = 13,8 m²/m³.**

**Costo de componentes del hormigón** (dosificación 3,5:2:1 pedregullo:arena:cemento, a/c=0,55, dens. aparente cemento=1.400 kg/m³ — mismo método "atajo en 1 paso" de Dic-2019, Guía sección 3):

| Componente | Vol. aparente (relación) | Coef. Aporte | Vol. real | Vol. aparente /1m³ real | Costo unitario | Costo |
|---|---|---|---|---|---|---|
| Pedregullo | 3,5 | 0,55 | 1,93 | 3,5/4,29=0,817 m³ | 760 $/m³ | 621 |
| Arena | 2 | 0,57 | 1,14 | 2/4,29=0,467 m³ | 600 $/m³ | 280 |
| Cemento | 1 | 0,45 | 0,45 | 1/4,29=0,233 m³ → 13,1 bolsas de 25kg | 200 $/bolsa | 2.614 |
| Agua (=kg cemento×a/c: 0,233×1.400×0,55/1000) | — | 1 | 0,77 | 0,77/4,29=0,180 m³ | — | 0 |
| **Suma vol. real** | | | **4,29** | | **Costo total** | **$3.514,59 /m³** |

**Costo total de materiales de la viga V305:**

| Ítem | Cantidad | Costo unitario | Costo |
|---|---|---|---|
| Hormigón | 0,48 m³ | 3.514,59 $/m³ | **$1.700** |
| Hierro | 41,2 kg | 115 $/kg | **$4.734** |
| Encofrado | 6,7 m² | 260 $/m² | **$1.731** |
| **Costo directo total** | | | **$8.165** |

---

## B. Industria de la Construcción (sin desarrollo oficial escrito — teórico, criterio de la Guía)

**Características generales/históricas:** actividad de **demanda derivada** (depende de la inversión pública y privada, muy sensible al ciclo económico — "termómetro" de la economía). Alta **intensidad de mano de obra** relativa a otras industrias, con régimen laboral propio (Ley 14.411, Convenio Colectivo Grupo 37, alta rotación obra-a-obra). Producción **no seriada, a medida** (cada obra es un prototipo único, distinto de una fábrica con producción estandarizada). **Localización fija** de la producción (el "taller" se traslada a la obra, no al revés). Fuerte **atomización empresarial** (conviven grandes constructoras con micro y pequeñas empresas/subcontratistas). Sector histórico motor de empleo y de políticas anticíclicas del Estado (obra pública como herramienta de reactivación). Alta incidencia de la **informalidad** relativa en algunos segmentos, y fuerte regulación sindical (SUNCA) y de seguridad (Ley 16.074, BSE).

## C. Evaluación de Inversión

**Datos:** capital a invertir 5.000 (miles USD, =5M USD), 6 años, tasa de interés de los depósitos 8% anual, tasa de descuento/inflación en dólares 6% anual.

**a) Completar flujos de Alt.1 y Alt.2:**
- **Alt.1** (capitalización de intereses, todo se cobra al final): flujo=0 en años 1-5; año 6 = `5.000×(1,08)⁶ = **7.934,4**` (capital+intereses compuestos).
- **Alt.2** (intereses simples pagados cada año, capital al final): interés anual = `5.000×8%=**400**` (años 1 a 5); año 6 = `400+5.000=**5.400**`.

| Invers. | año 0 | año 1 | año 2 | año 3 | año 4 | año 5 | año 6 |
|---|---|---|---|---|---|---|---|
| Alt.1 | -5.000 | 0 | 0 | 0 | 0 | 0 | 7.934 |
| Alt.2 | -5.000 | 400 | 400 | 400 | 400 | 400 | 5.400 |
| Alt.3 (dato) | -5.000 | 115 | 115 | 75 | 110 | 1.020 | 5.500 |
| Alt.4 (dato) | -5.000 | 260 | 240 | 375 | 350 | 500 | 6.000 |

**b) VNA a tasa de descuento 6% anual:**

| Alternativa | VNA @ 6% |
|---|---|
| Alt.1 | **593** |
| Alt.2 | **492** |
| Alt.3 | **0** (prácticamente nulo, ≈0,4) |
| Alt.4 | **654** |

**c) TIR de las 3 primeras + comparación de la 4ª sin calcularla:**
- Alt.1: TIR=**8,00%** (coincide con la tasa nominal del depósito, esperable: es un único flujo de entrada/salida capitalizado exactamente a esa tasa).
- Alt.2: TIR=**8,00%** (mismo resultado que Alt.1 — la TIR de un depósito a plazo fijo es siempre su tasa nominal, sin importar si los intereses se retiran cada año o se capitalizan, porque no hay reinversión implícita en el cálculo de la TIR misma).
- Alt.3: TIR=**6,00%** (coincide justo con la tasa de descuento usada — por eso su VNA@6% dio ≈0).

**Comparación de Alt.4 sin calcular su TIR exacta:** la mejor TIR de las otras 3 alternativas es 8% (Alt.1 y Alt.2). Si se calcula el VNA de Alt.4 a esa misma tasa (8%) y da **positivo** (`VNA@8%=123>0`), entonces la TIR de Alt.4 tiene que ser **mayor a 8%** (por la relación inversa entre VNA y tasa de descuento: si a 8% el VNA todavía no llegó a cero, hace falta una tasa aún más alta para anularlo) — sin necesidad de resolver la ecuación de la TIR de Alt.4 explícitamente. (De hecho, calculándola: TIR Alt.4=8,50%.)

**Recomendación:** la **Alternativa 4** es la mejor, por tener la mayor TIR (8,50%, superando a las demás) — y también el mayor VNA a la tasa de descuento del enunciado (654, el más alto de las 4).

**Nota importante (aclarada en la solución oficial):** que el VNA más alto a la tasa considerada (6%) sea el de Alt.4 **no garantiza automáticamente** que también tenga la mejor TIR — ambos criterios pueden discrepar según la tasa de descuento usada. En este examen, si se hubiera usado una tasa de descuento de 4,32% en vez de 6%, el VNA de Alt.4 igualaría exactamente al de Alt.1 (ambos ≈1.156), y para tasas de descuento **menores** a 4,32% el mejor VNA pasaría a ser el de la **Alt.1** en vez de la Alt.4 — el criterio de VNA es sensible a la tasa elegida, mientras que la TIR es una propiedad intrínseca de cada flujo, independiente de la tasa de descuento.

**d) Variante — el dinero recibido no se reinvierte (queda "parado" en una cuenta sin interés hasta el final):** en este escenario, lo que importa no es el VNA ni la TIR (ambos asumen que el dinero recibido se puede reinvertir a la tasa de descuento), sino el **monto TOTAL nominal recibido al final del plazo**, sin importar cuándo se cobró cada parte (porque una vez cobrado, no genera ningún rendimiento adicional hasta el final):

| Alternativa | Total nominal recibido (sin reinversión) |
|---|---|
| **Alt.1** | **7.934** ← la mayor |
| Alt.2 | 7.400 |
| Alt.3 | 6.935 |
| Alt.4 | 7.725 |

La **Alternativa 1** pasa a ser la más conveniente: es la única en la que **todo** el capital más los intereses permanece invertido (generando el 8% compuesto) durante los 6 años completos, sin ningún cobro parcial anticipado que quede luego "parado" sin rendir. Este es un giro conceptual clave: **el criterio de selección cambia completamente según el supuesto de reinversión** — con reinversión a la tasa de descuento (VNA/TIR), gana la Alt.4; sin ninguna reinversión del dinero ya cobrado, gana la Alt.1.

## D. Garantías (sin desarrollo oficial escrito — teórico, criterio de la Guía)

Ver Guía sección 7 (tabla rápida) y sección 10: las garantías habituales requeridas por el Contratante son: **Mantenimiento de Oferta** (a los oferentes, ~1% de la oferta, vigente 3-6 meses desde la presentación hasta la adjudicación — finalidad: asegurar que el oferente sostenga su oferta y firme el contrato si resulta adjudicado); **Fiel Cumplimiento de Contrato** (al contratista adjudicado, ~5-10% del contrato, desde la firma hasta la Recepción Provisoria — asegura la correcta ejecución de la obra); **Fondo de Reparo/Buena Ejecución** (retención de ~5% de cada certificado, hasta la Recepción Definitiva — cubre defectos que aparezcan durante el plazo de garantía); **Garantía de Anticipo** (100% del anticipo recibido, se devuelve a medida que se descuenta de los certificados — asegura que el anticipo se aplique efectivamente a la obra). Costo aproximado en todos los casos: 1,5%-2,0% anual del monto a garantizar (Fianza del Banco de Seguros del Estado, la forma de constitución más habitual en Uruguay; también avales bancarios o pólizas de compañías de seguro privadas).

## E. Varios (sin desarrollo oficial escrito — teórico, criterio de la Guía)

**a) Fórmula paramétrica:** ver Guía sección 8. Finalidad: actualizar el precio del contrato reconociendo la variación de costos de los insumos a lo largo de la ejecución, sin renegociar cada certificado. Expresión genérica (sin ajuste por costo financiero): `Coef. de ajuste = Σ (aᵢ × Pᵢ/Pᵢ₀)`, con `aᵢ` la incidencia % de cada insumo (Σaᵢ=100%) y `Pᵢ/Pᵢ₀` la relación entre el índice del mes de aplicación y el índice base.

**b) Coeficientes de movimiento de tierra:** ver Guía sección 13. **Esponjamiento (Ce):** relación entre el volumen del suelo suelto (recién excavado) y su volumen en banco (in situ) — el suelo excavado ocupa MÁS volumen que en banco. **Compactación (Cc):** relación entre el volumen del suelo compactado (en su ubicación final, ej. terraplén) y su volumen en banco — el suelo compactado ocupa MENOS (o similar) volumen que en banco. **Aporte/Acarreo (Ca):** el que se usa para dimensionar el transporte, vincula el volumen a transportar (suelto) con el volumen en banco. **Relación matemática:** todos se definen tomando el volumen **en banco** como referencia (=1); `Volumen suelto = Volumen banco × Ce`; `Volumen compactado = Volumen banco × Cc`; el coeficiente de aporte permite pasar directamente de banco a la cantidad de viajes de camión necesarios (`Ca` relacionado con `Ce`, ya que lo que se transporta es material suelto).

**c) Clasificación de costos por Naturaleza:** ver Guía sección 15. Los grandes grupos son: **Materiales** (insumos incorporados físicamente a la obra); **Mano de Obra** (jornales + cargas sociales del personal obrero); **Equipos** (amortización, mantenimiento, combustibles, operarios de equipo); **Subcontratos** (tareas tercerizadas completas, con su propio material+mano de obra+equipo incluido); **Gastos Generales/Indirectos** (estructura de obra y de la empresa no asignable directamente a una tarea: dirección técnica, administración, seguros, alquileres de obrador); y **Beneficio** (margen de la empresa).

---

## Resumen de resultados

| Parte | Resultado |
|---|---|
| A.a Volumen hormigón | **0,48 m³** |
| A.b Acero | **41,2 kg** — Cuantía **85,1 kg/m³** |
| A.c Encofrado | **6,7 m²** — Tenor **13,8 m²/m³** |
| A Costo del m³ de hormigón | **$3.514,59** |
| A Costo directo total de la viga | **$8.165** (hormigón $1.700 + hierro $4.734 + encofrado $1.731) |
| C.a Alt.1 año 6 | **7.934** (miles USD) |
| C.a Alt.2 año 6 | **5.400** (miles USD, + 400/año en años 1-5) |
| C.b VNA @6% | Alt.1=**593**, Alt.2=**492**, Alt.3=**0**, Alt.4=**654** |
| C.c TIR | Alt.1=**8,00%**, Alt.2=**8,00%**, Alt.3=**6,00%**, Alt.4=**8,50%** → **conviene Alt.4** |
| C.d Sin reinversión del dinero cobrado | **conviene Alt.1** (mayor monto nominal total recibido) |
