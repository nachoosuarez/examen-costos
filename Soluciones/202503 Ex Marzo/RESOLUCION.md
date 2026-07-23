# Examen Costos — Marzo 2025 (21/02/2025) — Resolución

Fuente: `Examen Costos 03-2025.pdf` (letra completa + Anexos I y II) y `Examen Costos 03-2025 - Preg. I,II,III,IV.pdf`
(este segundo archivo, pese al nombre, es la **planilla de solución oficial** de las partes I a IV con los
valores ya calculados — se usó para verificar el desarrollo). Partes V y VI no tienen solución oficial en el
repo; se resolvieron con criterio propio y se verificaron entre sí (tabla de venta total usada también en III).

Puntuación: I-20, II-10, III-20, IV-15, V-15, VI-10 (total 90 — así figura en la letra).

---

## I – Metraje (losa L102) — ✅ verificado contra solución oficial

**Datos de la letra:** recubrimientos despreciables; ganchos 10Φ; varillas comerciales de 12 m; empalme 50Φ;
tabla de densidad (kg/m) y desperdicio por diámetro (Anexo, incorporada más abajo).

**Lectura del plano (Anexo I, Planta Nivel I_100):** la losa L102 está entre las vigas V152/V153 (lado
horizontal) y V102/V105 (lado vertical). Las cotas acumuladas del plano dan, por diferencia entre ejes de
viga, el vano libre de la losa:

| Dirección | Cota mayor | Cota menor | Vano libre |
|---|---|---|---|
| Vertical (a) | 8,53 | 0,43 | **8,10 m** |
| Horizontal (b) | 11,71 | 6,17 | **5,54 m** |

- Espesor: **e = 0,15 m** (dato de detalle viga-losa).
- **Volumen hormigón** = a × b × e = 8,10 × 5,54 × 0,15 = **6,73 m³**.
- **Encofrado**: la losa es contenida lateralmente por las vigas (no se encofran laterales, solo cara
  inferior) → **44,87 m²** (= a×b + desarrollo de detalles del borde según plano).

**Armaduras** — la losa tiene dos capas de armado, típico de losa continua en dos direcciones:
- **Capa F (fondo/positiva)**: cubre todo el vano en ambas direcciones — Ø16 horizontal (paso 0,15,
  55 barras de 5,86 m) y Ø10 vertical (paso 0,23, 26 barras de 8,85 m).
- **Capa A (arriba/negativa, refuerzo sobre apoyos)**: barras cortas de Ø12 (2,25 m) que se colocan
  duplicadas — una franja junto a cada uno de los dos apoyos de la losa (por eso 138 barras horizontales
  y 52 verticales, el doble de lo que daría una sola franja).

| Ø | Uso | Cant. | L unit (m) | L tot (m) | kg c/desp |
|---|---|---|---|---|---|
| 16 | F horizontal | 55 | 5,86 | 322,30 | 585,62 |
| 10 | F vertical | 26 | 8,85 | 230,10 | 156,93 |
| 12 | A horizontal (refuerzo apoyos) | 138 | 2,25 | 310,50 | 303,98 |
| 12 | A vertical (refuerzo apoyos) | 52 | 1,55 | 80,60 | 78,91 |

**Total acero (kg con desperdicio) = 585,62+156,93+303,98+78,91 = 1.125,43 kg.**

### Resultados finales

| Magnitud | Valor |
|---|---|
| Volumen hormigón | **6,73 m³** |
| Encofrado | **44,87 m²** |
| Acero total | **1.125,43 kg** |
| **Tenor** (encof/vol) | **6,67 m²/m³** |
| **Cuantía** (acero/vol) | **167,20 kg/m³** |

**¿Son esperables?** El tenor (6,67 m²/m³) está dentro del rango típico de una losa suspendida de este
espesor (rango usual ~5-8 m²/m³, ver guía de metraje). La **cuantía (167,2 kg/m³) es alta** para una losa
simple (lo típico ronda 80-120 kg/m³): se justifica porque **hay doble capa de armado en ambas
direcciones** (fondo + refuerzo negativo duplicado sobre los dos apoyos), lo cual es esperable en una
losa continua de varios paños con momentos negativos importantes sobre vigas — **no es un error**, es
consecuencia directa de la geometría de armado que muestra el plano.

---

## II – Costo de Componentes del Hormigón — ✅ verificado contra solución oficial

Relación en volumen 4 : 2,5 : 1 (grueso : fino : cemento); a/c = 0,40 lt/kg; densidad aparente cemento
1.400 kg/m³.

**Paso a paso (método de la guía, tipo 3):**
1. Volumen real de cada componente = vol. aparente × coef. de aporte:
   - Grueso: 4 × 0,50 = 2,000 · Fino: 2,5 × 0,60 = 1,500 · Cemento: 1 × 0,47 = 0,470 → **Σ = 3,97**.
2. Fracción normalizada a 1 m³ real: Grueso 2,00/3,97=0,504 · Fino 1,50/3,97=0,378 · Cemento
   0,47/3,97=0,118.
3. Volumen aparente para 1 m³ de hormigón = fracción × vol. aparente propio / Σaparentes:
   Grueso 0,883 m³ · Fino 0,552 m³ · Cemento 0,221 m³ (equivalente a **309 kg de cemento** con la
   densidad dada: 0,221×1.400=309,4 kg).
4. Agua: relación a/c=0,40 sobre 309 kg de cemento → **≈124 lt** (verificado también con la
   equivalencia del enunciado: 20 lt agua ↔ 35,714 lt cemento ↔ 50 kg cemento, es decir 0,56 lt agua
   por cada lt de cemento).
5. Costo: Grueso 0,883 m³×500=441,50 $ · Fino 0,552 m³×400=220,80 $ · Cemento 309 kg×12 $/kg
   (300$/bolsa de 25kg = 12$/kg) = 3.708,00 $ · Agua sin costo asignado.

**Costo total = 441,50 + 220,80 + 3.708,00 = $ 4.370,30 por m³ de hormigón.**

---

## III – Ajuste de Precios

### a) Finalidad y expresión genérica

Las fórmulas paramétricas **trasladan al precio contractual las variaciones de costo de los insumos
principales entre la fecha de oferta (mes 0) y la fecha de obra (mes n)**, evitando que contratista o
contratante asuman un riesgo que no controlan (inflación de insumos vs. contrato a precio fijo).

Expresión genérica completa:

`Pn = P0 × [ a·(J n/J0) + b·(M1n/M10) + c·(M2n/M20) + ... + z·(Zn/Z0) ]`

donde: `Pn`/`P0` = precio ajustado/base; cada coeficiente (a, b, c, ..., z) es la **incidencia porcentual**
del insumo respectivo sobre el precio total, con `a+b+c+...+z = 1`; `J` = índice de mano de obra; `M1,
M2, ...` = índices de materiales representativos; los índices `n`/`0` son los valores del índice en el mes
de pago y en el mes base, respectivamente.

### b) Fórmula propuesta para los hormigones armados

**Paso previo — armar la tabla base de costo directo** (mismos insumos de la parte VI, el "detalle
resumen general" al que remite el enunciado):

| Insumo | Monto $ | Incidencia s/venta |
|---|---|---|
| Mano de Obra | 660.000 | 20,86% |
| Cemento | 234.000 | 7,39% |
| Arena | 399.000 | 12,61% |
| Piedra partida | 433.000 | 13,68% |
| Hierro | 288.000 | 9,10% |
| Madera pino Brasil | 180.000 | 5,69% |
| Varios | 100.000 | 3,16% |
| **Costo directo** | **2.294.000** | 72,49% |
| Gastos Indirectos | 396.000 | 12,51% |
| Beneficio (15% s/venta) | 474.706 | 15,00% |
| **Venta Total** | **3.164.706** | 100,00% |

(Venta Total = (Costo directo + G.Indirectos) / (1 − 0,15) = 2.690.000/0,85 = **$3.164.706**.)

**Elección de índices** (Anexo II, Boletín Cámara de la Construcción) y coeficientes redondeados a
sumar 100% (criterio propio para Gastos Indirectos+Beneficio: se ajustan con el **Índice de Precios al
Consumo — IPC**, código E03, por ser costos de estructura/gestión de la empresa más ligados a la
economía general que a un insumo puntual de obra):

| Símbolo | Código | Insumo/índice | Coef. propuesto |
|---|---|---|---|
| J | D02 | Índice de Mano de Obra (ICC) | 21% |
| M1 | B09 | Portland gris, bolsa 25kg en planta | 7% |
| M2 | B04 | Arena Gruesa | 13% |
| M3 | B12 | Pedregullo doble lavado y clasificado | 14% |
| M4 | B02 | Acero Tratado ADM 420 | 9% |
| M5 | B10 | Madera para encofrado de pino nacional | 6% |
| CV | E03 | Índice de Precios al Consumo (Gastos Indirectos + Beneficio) | 30% |
| **Σ** | | | **100%** |

`Pn/P0 = 0,21·(Jn/J0) + 0,07·(M1n/M10) + 0,13·(M2n/M20) + 0,14·(M3n/M30) + 0,09·(M4n/M40) + 0,06·(M5n/M50) + 0,30·(CVn/CV0)`

Nota: es una de varias soluciones válidas — la planilla oficial muestra 4 variantes posibles (con distinto
peso relativo entre IPC y Dólar interbancario para el rubro de Gastos Indirectos+Beneficio). Lo esencial
es que: (1) cada insumo relevante tenga su propio índice específico, (2) los coeficientes sumen 100%, y
(3) el rubro de indirectos/beneficio se cubra con un índice general (IPC y/o dólar), no con un índice de
insumo de obra.

---

## IV – Punto de Equilibrio

### a) Definición

El **Punto de Equilibrio** es el nivel de producción/venta en el cual los **Ingresos Totales igualan a los
Costos Totales** (Costos Fijos + Costos Variables), es decir, el resultado (ganancia) es nulo. Por debajo
de ese nivel la empresa pierde dinero; por encima, gana. Se calcula como `Q_equilibrio = CF / (Pu − Cvu)`
(cantidad) siendo Pu el precio unitario de venta y Cvu el costo variable unitario.

### b) Caso — campaña de publicidad

**Situación base (sin publicidad):** la fábrica está en su propio punto de equilibrio → `VT1 = CT1 = CF1 + CV1`.

**Con publicidad:**
- Ventas: +20% en cantidad y +5% en precio unitario → `VT2 = 1,20 × 1,05 × VT1 = 1,26 × VT1 = 1,26·CV1 + 1,26·CF1`
  (porque VT1=CF1+CV1, y al no cambiar la composición de costos base, ambos términos escalan igual dentro de VT1).
- Costos: CV sube 20% (proporcional a la mayor cantidad vendida) y CF sube 10% (costo de la campaña) →
  `CT2 = 1,20·CV1 + 1,10·CF1`.

**Conviene si VT2 > CT2:**

```
1,26·CV1 + 1,26·CF1 > 1,20·CV1 + 1,10·CF1
0,06·CV1 + 0,16·CF1 > 0
```

Como CV1 y CF1 son siempre positivos (son costos), la desigualdad **se cumple siempre**.

**Conclusión: conviene aceptar la propuesta en cualquier escenario**, porque el aumento combinado de
cantidad y precio (+26% en ventas) supera cómodamente al aumento de costos (variable +20%, fijo
+10%), sin importar la proporción entre CF1 y CV1 de partida. (Verificado numéricamente con valores
arbitrarios CV1=1.000, CF1=500: VT2−CT2=140 = 0,06×1.000+0,16×500=140 ✓.)

---

## V – Inversiones

### a) VNA (Valor Neto Actualizado)

Es la suma algebraica de todos los flujos de fondos (ingresos menos egresos) de un proyecto de
inversión, **traídos a valor presente** descontándolos a una tasa de interés/descuento dada:
`VNA = Σ Flujo_t / (1+i)^t`, para t = 0 (momento de la inversión) hasta n (horizonte del proyecto). Si
VNA > 0 el proyecto genera valor por encima de la tasa exigida; si VNA < 0, no la alcanza; si VNA = 0 la
tasa usada coincide exactamente con la rentabilidad del proyecto (es su TIR).

### b) TIR (Tasa Interna de Retorno)

Es la **tasa de descuento que hace VNA = 0** para el flujo de fondos del proyecto: es la rentabilidad
"propia" (intrínseca) de la inversión, medida en % anual, sin referencia a una tasa externa. Se usa para
comparar la rentabilidad del proyecto contra el costo de oportunidad del capital (u otra tasa de
referencia, ej. tasa de interés bancaria): si TIR > tasa de referencia, conviene invertir.

### c) Obra: margen/beneficio — Inversión: TIR

Una **obra** es, en general, una **operación de corto/mediano plazo con un único desembolso de
recursos propios acotado** (capital de trabajo) contra un ingreso por certificados durante el plazo de
ejecución: el resultado relevante es cuánto queda de **ganancia sobre el precio de venta** (margen %),
sin que el valor tiempo del dinero sea el factor determinante del negocio.

Una **inversión** implica comprometer un capital significativo **durante varios períodos**, con flujos de
ingresos y egresos distribuidos en el tiempo (a veces años): ahí sí el momento en que ocurre cada flujo
importa mucho (el dinero hoy vale más que el mismo monto en el futuro), por lo que se necesita una
métrica que capture la **rentabilidad del capital invertido en el tiempo** — eso es exactamente lo que
mide la TIR (y el VNA), a diferencia del margen simple que no considera cuándo ocurren los flujos.

---

## VI – Suministros

Para que los suministros de una obra estén correctamente:

**a) Identificados:** especificación técnica completa y sin ambigüedad (marca/modelo o normas
equivalentes, memoria descriptiva), cantidad de proveedores/alternativas de mercado consultadas,
ensayos o certificaciones exigibles, lugar y condiciones de entrega (obra/depósito), necesidad o no de
contrato de suministro formal, plazos de fabricación si es un producto no estándar (importado o a
medida).

**b) Cuantificados:** unidad de medida coherente con la de compra en plaza, criterio de desperdicio
aplicado (según el tipo de material y su forma de colocación), cantidad total requerida con su desglose
por etapa/rubro, y el plazo/cronograma de entrega necesario para no atrasar la obra ni sobre-acopiar.

**c) Valorados:** precio unitario **vigente** (cotización actualizada, no un precio histórico), en la unidad
definida en (b), incluyendo condición de entrega (fletes, seguros, aranceles si es importado — ver
INCOTERMS) y forma de pago/plazo, ya que ambos inciden en el costo financiero del suministro.

---

## Resumen de resultados

| Parte | Resultado clave |
|---|---|
| I | Vol. 6,73 m³ · Encof. 44,87 m² · Acero 1.125,43 kg · Tenor 6,67 m²/m³ · Cuantía 167,20 kg/m³ |
| II | Costo componentes hormigón = **$4.370,30/m³** |
| III | Fórmula paramétrica con 6 insumos específicos + 1 índice general (IPC), coef. suman 100% |
| IV | Conviene aceptar la campaña en todos los casos (0,06·CV1+0,16·CF1 > 0 siempre) |
| V | VNA, TIR y su rol diferencial obra vs. inversión — conceptual |
| VI | Identificación, cuantificación y valoración de suministros — conceptual |
