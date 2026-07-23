# Examen Costos — Febrero 2025 (29/01/2025) — Resolución

Fuente: `Examen Costos 02-2025.pdf` (letra completa + Anexo I) y `Examen Costos 02-2025 - Preg. I,II,III.pdf`
(planilla de solución oficial de las partes I a III con los valores ya calculados, usada para verificar el
desarrollo). Partes IV, V y VI no tienen solución oficial en el repo; se resolvieron con criterio propio a
partir de la letra y del resumen teórico (Clase 19, Clase 9, Clase 2 y Clase 20).

Puntuación: I-25, II-15, III-20, IV-10, V-10, VI-10 (total 90). Aprobación: 50 puntos.

---

## I – Metraje Hormigón (muro de contención en L, 30 m de longitud) — ✅ verificado

**Datos:** recubrimientos despreciables; varillas comerciales de 12 m; empalme 50Φ; tabla de
densidad/desperdicio por diámetro (incluye Φ19 y Φ22, no usados en este muro).

**Geometría (Anexo I, corte transversal del muro, en metros; separaciones en cm):**
- **Base (zapata)**: ancho b=3,00 m, espesor h=0,40 m, longitud 30 m (apoya en el suelo → **no se
  encofra la cara inferior**, solo las dos caras laterales).
- **Muro (pantalla vertical)**: espesor 0,40 m, altura 3,95 m, longitud 30 m (elemento libre → **se
  encofran ambas caras**).

| Elemento | V (m³) = L×b×h | Encofrado (m²) |
|---|---|---|
| Base | 30×3,00×0,40 = **36,00** | 2 caras laterales × 0,40×30 = **24,00** |
| Muro | 30×0,40×3,95 = **47,40** | 2 caras × 3,95×30 = **237,00** |
| **Total** | **83,40 m³** | **261,00 m²** |

**Armaduras** — dos familias, según el plano de detalle:

*a) Barras "longitudinales"* (corren a lo largo de los 30 m del muro, dentro de la sección transversal,
espaciadas cada 0,20 m verticalmente): Ø10/20 horizontal-izquierda (cara interior del muro), Ø12/20
horizontal-derecha (cara exterior del muro), Ø12/20 superior e Ø10/20 inferior (base). Como la barra
comercial es de 12 m y el muro mide 30 m, cada tramo lleva **2 empalmes de 50Φ** por barra continua
(3 tramos de 12+12+6m ≈ 2 empalmes). Cantidad de barras = redondeo hacia arriba(altura del
elemento/paso)+1:

| Id | Ø | Tramo (altura, m) | Paso (m) | Cant. | L base (m) | + 2 empalmes 50Φ | L/barra (m) | L tot (m) | kg c/desp |
|---|---|---|---|---|---|---|---|---|---|
| Long-izq | 10 | 3,95 (muro) | 0,20 | 21 | 30,00 | +2×0,50=1,00 | 31,00 | 651,00 | 443,98 |
| Long-der | 12 | 3,95 (muro) | 0,20 | 21 | 30,00 | +2×0,60=1,20 | 31,20 | 655,20 | 641,44 |
| Long-sup | 12 | 3,00 (base) | 0,20 | 16 | 30,00 | +2×0,60=1,20 | 31,20 | 499,20 | 488,72 |
| Long-inf | 10 | 3,00 (base) | 0,20 | 16 | 30,00 | +2×0,50=1,00 | 31,00 | 496,00 | 338,27 |

*b) Barras "transversales"* (son la armadura del corte, repetida cada 0,20 m a lo largo de los 30 m del
muro): Ø10/20 vertical-izquierda, Ø16/20 vertical-derecha (armadura principal del muro, mayor
diámetro por ser la que resiste el momento flector de empuje de tierras), Ø16/20 horizontal-superior y
Ø10/20 horizontal-inferior (armadura de la base). Cantidad = redondeo hacia arriba(30/0,20)+1 = 151
barras (una cada 0,20 m a lo largo del muro, sin empalme porque cada una es más corta que 12 m):

| Id | Ø | L individual (m, leída del corte) | Cant. (a lo largo de 30 m, paso 0,20) | L tot (m) | kg c/desp |
|---|---|---|---|---|---|
| Vert-izq | 10 | 4,45 (altura muro 3,95 + espesor base 0,40 + gancho 10Φ=0,10) | 151 | 671,95 | 458,27 |
| Vert-der | 16 | 5,25 (armadura principal, mayor desarrollo/anclaje en la base) | 151 | 792,75 | 1.440,43 |
| Horiz-sup | 16 | 3,23 (ancho base 3,00 con gancho/anclaje en el borde) | 151 | 487,73 | 886,21 |
| Horiz-inf | 10 | 3,23 (ídem, cara inferior de la base) | 151 | 487,73 | 332,63 |

**Total acero (kg con desp) = 443,98+641,44+488,72+338,27+458,27+1.440,43+886,21+332,63 = 5.029,95 kg.**

### Resultados finales

| Magnitud | Valor |
|---|---|
| Volumen hormigón | **83,40 m³** |
| Encofrado | **261,00 m²** |
| Acero total | **5.029,95 kg** |
| **Tenor** (encof/vol) | **3,13 m²/m³** |
| **Cuantía** (acero/vol) | **60,31 kg/m³** |

Tenor y cuantía más bajos que en una losa (comparar con el examen de Marzo-2025): es coherente,
porque un muro de contención tiene menos superficie de encofrado relativa a su volumen (una sola
cara por lado, elementos macizos) y menos densidad de armado que una losa de edificio con doble
capa — valores típicos de muro/zapata en el orden de 3-5 m²/m³ y 50-90 kg/m³.

*(Nota: la planilla oficial titula esta tabla "Metrajes losa" — es un error de tipeo/plantilla reutilizada del
archivo, el elemento es claramente el muro de contención en L del Anexo I, no una losa.)*

---

## II – Costo de Componentes del Hormigón — ✅ verificado

Relación en volumen 4 : 2,5 : 1; a/c = 0,50 lt/kg; densidad aparente cemento 1.400 kg/m³.

**Paso a paso (mismo método que en Marzo-2025 y Dic-2025, guía tipo 3):**
1. Volumen real de cada componente = vol. aparente × coef. de aporte: Pedregullo 4×0,55=2,200 ·
   Arena 2,5×0,57=1,425 · Cemento 1×0,47=0,470.
2. Volumen real de agua a partir de a/c: se despeja junto con el cemento de forma que a/c=0,50 se
   cumpla sobre el cemento resultante (ver más abajo) → 0,700.
3. Suma de real (agregados+cemento+agua) = 2,200+1,425+0,470+0,700 = **4,795**.
4. Volumen aparente para 1 m³ de hormigón = vol. aparente propio / 4,795: Pedregullo 4/4,795=0,834
   m³ · Arena 2,5/4,795=0,521 m³ · Cemento 1/4,795=0,209 m³ → equivalente a 0,209×1.400=**292 kg
   de cemento**. Verificación cruzada: agua = a/c × cemento = 0,50×292=**146 lt** = 0,146 m³ = 0,700/4,795 ✓.
5. Costo: Pedregullo 0,834 m³×600=500,40 $ · Arena 0,521 m³×500=260,50 $ · Cemento 292 kg×10
   $/kg (250$/bolsa de 25kg=10$/kg)=2.920,00 $ · Agua sin costo asignado.

**Costo total = 500,40 + 260,50 + 2.920,00 = $ 3.680,90 por m³ de hormigón.**

---

## III – Costo Directo y de Equipos (retroexcavadora) — ✅ verificado

**Objetivo:** costo directo por m³ de excavación (sin LLSS de mano de obra).

### 1) Costo horario del equipo (retroexcavadora sola)

Datos: VN=100.000 U$S, VR=20.000 U$S (20% de VN), n=5 años, horas trabajadas 2.880 h/año (H total
de vida = 5×2.880=14.400 h), tasa interés anual i=6%, seguro+patente sp=2,0% anual sobre VN.

- **Interés Horario** `IH = [(n+1)·VN + (n-1)·VR] / (2n) · i / (horas/año)`
  = [(6×100.000)+(4×20.000)] /10 × 0,06 / 2.880 = 68.000×0,06/2.880 = **1,42 U$S/h**
  (68.000 U$S es el capital medio invertido a lo largo de la vida útil, según la fórmula del interés
  sobre saldo con depreciación lineal).
- **Depreciación Horaria** `DH = (VN-VR)/(n×horas/año)` = 80.000/14.400 = **5,56 U$S/h**.
- **Seguro + Patente Horario** `SPH = sp×VN/(horas/año)` = 0,02×100.000/2.880 = **0,69 U$S/h**.
- **II – Costo de Equipo = 1,42+5,56+0,69 = 7,67 U$S/h** (22,61% del total).

### 2) Costo de mantenimiento

Mantenimiento creciente por año (2,0%; 2,5%; 3,0%; 3,5%; 4,0% sobre VN) → **promedio 5 años = 3,0%**.
`MH = Mmed×VN/(horas/año)` = 0,03×100.000/2.880 = **1,04 U$S/h** (3,07% del total).

### 3) Costo de operación (mano de obra + combustible)

| Insumo | Cantidad | Costo unit. (U$S) | Costo horario (U$S/hm) |
|---|---|---|---|
| Operador | 1,10 hh/hm | 4,50 | 4,95 |
| Peón/Ayudante | 0,30 hh/hm | 2,50 | 0,75 |
| **Mano de Obra** | | | **5,70** (16,81%) |
| Gasoil | 15 lt/hm | 1,30 | 19,50 |
| **Materiales de Consumo** | | | **19,50** (57,51%) |
| **I – Costo de Operación** | | | **25,20 U$S/h** (74,32%) |

(Sin cargas sociales sobre la mano de obra, tal como pide el enunciado — coeficiente 0%.)

### 4) Costo horario total y costo directo de excavación

**IV – Costo Horario = Operación + Equipo + Mantenimiento = 25,20 + 7,67 + 1,04 = 33,91 U$S/hm.**

Rendimiento de excavación: 0,15 hm/m³ (dato).

**Costo directo unitario de excavación = 33,91 × 0,15 = 5,09 U$S/m³.**

---

## IV – Seguros para las Obras

### a) Finalidad general

Los seguros de obra buscan **transferir a un tercero (asegurador) el riesgo económico de eventos
adversos** que, de materializarse, generarían un desembolso o pérdida difícil de absorber con recursos
propios de la obra o de la empresa — a cambio de una prima cierta y conocida de antemano, la
empresa se protege de una pérdida incierta pero potencialmente muy grande.

### b) Componentes principales de una póliza (ver Clase 19, ya resumido en `RESUMEN_TEORICO.md`)

Objeto asegurado; valor del objeto; riesgos/eventos cubiertos; monto máximo de indemnización; prima
(costo del seguro); deducible (franquicia a cargo del asegurado); plazo de vigencia; deberes del
contratante (obligaciones que debe cumplir para que la póliza sea válida); exclusiones (eventos no
cubiertos).

### c) Los cuatro seguros más usuales en obra y qué cubren

1. **Accidentes de Trabajo** (Ley 16.074, monopolio BSE) — cubre accidentes/enfermedades
   profesionales del personal en obra; para el personal obrero amparado por la Ley 14.411 está
   incluido dentro del Aporte Unificado de la Construcción.
2. **Vehículos y Maquinaria** — cubre daños propios de los equipos/vehículos utilizados en la obra y
   daños a terceros causados por ellos (≈2% anual del valor del equipo).
3. **Todo Riesgo de Construcción (TRC)** — cubre daños materiales a la obra en ejecución por
   derrumbe, incendio, inundación, robo, etc. (≈0,3%-0,5% del monto del contrato en obras comunes).
4. **Responsabilidad Civil (RC)** — cubre daños a terceros (personas o propiedades ajenas a la obra)
   originados por la actividad de la obra/contratista (≈0,3% anual sobre el contrato, a veces ya
   incluido dentro del TRC).

---

## V – Régimen Salarial

### a) Sistema de remuneración amparado por la Ley 14.411

El personal con tareas directas en obra tributa el **Aporte Unificado de la Construcción** (en lugar del
régimen general de Industria y Comercio). El sistema retribuye principalmente **por tiempo trabajado**
(jornal, según categoría y el Laudo vigente — 44 hs semanales: lunes a jueves 9 hs, viernes 8 hs), y de
forma secundaria admite retribución por producción/destajo. Sobre la hora común de cada categoría
se agregan partidas complementarias (presentismo, tickets, ropa/transporte/herramientas, feriados,
horas extra, nocturnidad, etc. — ver detalle completo en la Guía de Ejercicios Tipo, sección 5). El Monto
Imponible (≈80% del jornal) tributa Leyes Sociales a una tasa que ronda 71,8%-75,8% según el tipo de
obra (ingeniería/arquitectura).

### b) Convenio Colectivo de la Construcción (Grupo 37)

Es un acuerdo **tripartito**: **Empresas** (cámaras empresariales), **Trabajadores** (SUNCA, sindicato
único) y el **MTSS/Poder Ejecutivo**, que actúa como mediador y homologa el acuerdo final. Se
renegocia cada 3 años. Principales aspectos que trata: escala de laudos por categoría y su ajuste
periódico (ligado a metas de inflación del BCU), licencias, condiciones de trabajo, aportes a los 4
Fondos Sociales de la Construcción (FOSVOC, FSC, FOCAP, FOCER — ver Guía sección 6), y reglas de
despido/indemnización propias del sector (alta rotación de personal entre obras).

### Características principales del mercado de la construcción en Uruguay

- **Régimen laboral especial**, distinto al régimen general, con convenio tripartito propio.
- **Alta incidencia de mano de obra no calificada o semicalificada.**
- **Alta rotación de personal**: solo ≈20% de los obreros son permanentes de una misma empresa
  entre obra y obra (el resto migra según la demanda de cada obra/zona).
- **Obra pública**: contratación por licitación abierta, regida por el TOCAF; baja planificación de largo
  plazo porque depende del ciclo de inversión pública/político.
- **Obra privada**: contratación por licitación cerrada (información reservada entre oferentes);
  fuertemente sensible al ciclo económico y, en algunas plazas (ej. Punta del Este), a la inversión
  extranjera.
- **Sector cíclico**, con fuerte estacionalidad e impacto directo del nivel de actividad económica
  general del país.

---

## VI – Estado Económico y Financiero

### a) Definiciones

- **Cronograma/Estado Económico**: `Ventas − Costos = Utilidad`. Mide la **rentabilidad** de la obra:
  cuánta ganancia deja el negocio en su conjunto, independientemente de cuándo ocurren los cobros
  y pagos en el tiempo. Su objetivo es la **economicidad/viabilidad económica** (utilidad positiva); el
  solo análisis del punto de equilibrio no alcanza para esto, se necesita ver el margen/beneficio real.
- **Cronograma/Estado Financiero**: `Ingresos − Egresos = Disponibilidad`. Mide si la empresa **tiene
  caja suficiente en cada momento** de la obra para afrontar sus pagos, considerando el desfasaje real
  en el tiempo entre cuándo se paga a proveedores/mano de obra y cuándo se cobra al cliente. Su
  objetivo es la **viabilidad financiera/equilibrio financiero** (disponibilidad ≥ 0 en todo momento).

### b) Importancia y qué controla cada uno

El **Estado Económico** controla que el negocio sea rentable en sí mismo (que la venta total supere al
costo total, dejando el margen/beneficio esperado) — es la visión de "cuánto se gana". El **Estado
Financiero** controla la **liquidez**: una obra puede ser económicamente rentable en el papel y aun así
fracasar si en algún mes los egresos (mano de obra, materiales, equipos, suministros con sus propios
plazos de pago) superan a los ingresos (cobros de certificados, típicamente rezagados 30-60 días
respecto al gasto) y la empresa se queda sin caja para pagar. Por eso se calcula además un **Costo
Financiero** (interés sobre el capital que la empresa debe adelantar mientras espera cobrar) — en el
ejemplo desarrollado en Clase 20, ese costo financiero resultó del orden de 0,03%-0,54% de la venta
según el anticipo pactado con el cliente (a mayor anticipo, menor necesidad de financiación y menor
costo financiero, acercándose a la "autofinanciación" de la obra). En definitiva: **económico = cuánto
se gana; financiero = si hay caja para bancarse el camino hasta ganarlo.**

---

## Resumen de resultados

| Parte | Resultado clave |
|---|---|
| I | Vol. 83,40 m³ · Encof. 261,00 m² · Acero 5.029,95 kg · Tenor 3,13 m²/m³ · Cuantía 60,31 kg/m³ |
| II | Costo componentes hormigón = **$3.680,90/m³** |
| III | Costo horario retroexcavadora 33,91 U$S/hm → costo directo excavación **5,09 U$S/m³** |
| IV | 4 componentes de póliza + 4 seguros usuales (AT, Vehículos/Maquinaria, TRC, RC) |
| V | Ley 14.411, Convenio Colectivo tripartito (Grupo 37), características del mercado uruguayo |
| VI | Estado Económico (Utilidad=Ventas−Costos) vs. Estado Financiero (Disponibilidad=Ingresos−Egresos) |
