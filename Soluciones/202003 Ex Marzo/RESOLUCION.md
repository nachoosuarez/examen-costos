# Examen Costos (2240) — 18/02/2020 ("Marzo 2020")

Fuente: `Exámenes/202003 Ex Marzo/Examen costos 03-2020 con Anexo y Cuadro CF.pdf` (letra + Anexo I) + `Examen Costos Mar-2020 I,II,III.pdf` (planilla oficial ya resuelta de I, II y III, usada como solución oficial). **Partes I, II y III verificadas exactas contra la planilla oficial. Partes IV y V son teóricas, sin solución oficial en el repo (respondidas con el criterio de la Guía).**

> **¡IMPORTANTE — discrepancia detectada con el material del curso 2026!** La Clase 4 (`CLASES TEORICAS/Clase 4 (3).pdf`, diapositivas 125-128) usa este MISMO ejercicio (muro de contención Marzo-2020) como ejemplo de clase, pero llega a números de encofrado y acero **distintos** a los de la planilla oficial de la Parte I de abajo:
> - **Encofrado:** la Clase 4 calcula `E=(0,2+2,4)×45=117 m²` (una sola cara CONTINUA para pata+muro juntos, como si fuera un único perfil vertical de 2,6m de alto encofrado de un solo lado) → Tenor=117/25,2=**4,6 m²/m³**. La planilla oficial del examen (usada abajo) da **126,00 m²** (pata con 2 caras=18,00 + muro con 1 cara=108,00) → Tenor=**5,00 m²/m³**.
> - **Acero (barra "horquilla" Ø12 c/20):** la Clase 4 usa una longitud unitaria de **6,56 m** (con un desarrollo explícito: 0,4+0,2+0,4+2,6+0,2+2,6+2×10Ø) → 226×6,56×0,89×1,10=**1.451,4 kg**, dando un Total de acero=**2.239,2 kg** y Cuantía=**88,9 kg/m³**. La planilla oficial (abajo) usa L=6,28m → Total=**2.177,28 kg**, Cuantía=**86,4 kg/m³**.
>
> **Ambos son legítimos** (la planilla oficial es la que efectivamente se usó para calificar el examen real de 2020; la Clase 4 es la forma en que el equipo docente ACTUAL explica el mismo ejercicio en 2026, con el criterio de "encofrado a una sola cara continua, incluida la pata" que puede ser el que se espera aplicar en el examen de este año). **Ante esta discrepancia, priorizar el criterio de la Clase 4 (más reciente) si el examen no aclara el criterio de encofrado de la pata**, pero tener presente que una planilla oficial de examen real puede diferir. La resolución completa de abajo sigue la planilla oficial (para poder verificar cada paso); ver la nota de la Guía sección 1 con el detalle de ambos números.

## Enunciado resumido

- **I. Metraje de Hormigón (25 pts):** volumen, cuantía de acero y tenor de encofrado de un muro de contención (croquis Anexo I): pata de fundación + muro vertical, longitud 45 m.
- **II. Costo Financiero (20 pts):** flujo de ingresos/egresos de una obra con anticipo del 20% (devuelto proporcionalmente en cada certificado). Elegir entre 2 líneas de crédito, calcular intereses totales y el monto máximo a usar.
- **III. Garantías (20 pts):** costo de garantías de Fiel Cumplimiento, Buena Ejecución (fondo de reparo) y Anticipo, para todo el plazo contractual + de garantía.
- **IV. Régimen Salarial (15 pts):** características del sistema de remuneración Ley 14.411; partes e ítems del Convenio Colectivo de la Construcción (Grupo 37).
- **V. Materiales (10 pts):** qué información se necesita para que los materiales estén correctamente identificados, cuantificados y valorados.

---

## I. Metraje — Muro de contención

**Geometría (Anexo I):** pieza de 45 m de longitud, ejecutada por trincheras (taludes verticales en el terreno, sin necesidad de entibado). Sección: pata (zapata corrida) de 0,40×0,20 m; muro vertical de 0,20 m de espesor × 2,40 m de altura. Armadura: `2Ø12` (longitudinal en la base de la pata), `2Ø12A` (bastones que anclan la pata al muro), `Ø12 c/20` (armadura principal del muro, en horquilla que sube desde la pata hasta arriba), `2Ø12E` (cierre/gancho en la coronación de esa horquilla), `Ø8 c/20` (armadura horizontal de repartición del muro). Diámetros/pesos: Ø8=0,39 kg/m (desperdicio 5%), Ø12=0,89 kg/m (desperdicio 10%). Varillas comerciales de 12 m, empalmes Ø8=0,50 m y Ø12=0,70 m.

**a) Volumen de hormigón:**

| Elemento | b (m) | h (m) | L (m) | V (m³) |
|---|---|---|---|---|
| Pata | 0,40 | 0,20 | 45,0 | 3,60 |
| Muro | 0,20 | 2,40 | 45,0 | 21,60 |
| **Total** | | | | **25,20** |

**b) Encofrado** (solo cara expuesta; la cara contra el talud de excavación no se encofra):

| Elemento | Cara encofrada | Encof (m²) |
|---|---|---|
| Pata | 2 caras laterales (h=0,20×L=45, ×2) | 18,00 |
| Muro | 1 cara vista (h=2,40×L=45) | 108,00 |
| **Total** | | **126,00** |

**Tenor = 126,00 / 25,20 = 5,00 m²/m³.**

**c) Acero.** Regla de oro: las barras que recorren los 45 m de longitud deben partirse en tramos de 12 m con empalmes (longitud efectiva = 45 + n_empalmes×long. de empalme):
- Longitud con empalmes Ø12 (4 tramos, 3 empalmes de 0,70 m): 45 + 3×0,70 = **47,1 m**.
- Longitud con empalmes Ø8 (4 tramos, 3 empalmes de 0,50 m): 45 + 3×0,50 = **46,5 m**.

| Familia | Ø | Paso | Cant. | L (m) | kg con desp. |
|---|---|---|---|---|---|
| Pata: `2Ø12` (base) + `2Ø12A` (bastón anclaje, ×2 por tener pata a ambos lados del eje) | 12 | — | 8 | 47,1 | 8×47,1×0,89×1,10 = **368,89** |
| Muro: `Ø8 c/20` horizontal (repartición) | 8 | 0,20 | 22 | 46,5 | 22×46,5×0,39×1,05 = **418,92** |
| Muro: `Ø12 c/20` horquilla vertical (anclada en pata como `2Ø12A`, sube y cierra arriba como `2Ø12E`) — 1 horquilla cada 0,20 m en los 45 m: 45/0,20+1 = 226 unidades, L≈6,28 m c/u (recorrido pata→muro→gancho de cierre) | 12 | 0,20 | 226 | 6,28 | 226×6,28×0,89×1,10 = **1.389,48** |
| **Total acero** | | | | | **2.177,28 kg** |

*(Verificado: 368,89+418,92+1.389,48 = 2.177,29 ≈ 2.177,28 kg de la planilla oficial, diferencia solo por redondeo.)*

**Cuantía = 2.177,28 / 25,20 = 86,40 kg/m³.**

---

## II. Costo Financiero

**Datos:** ingresos totales $20.000.000 (en miles: 20.000), egresos totales -17.000; anticipo=20% del precio, devuelto como quita del 20% en cada certificado posterior. Línea 1: límite $2.000.000, interés mensual 2,5%. Línea 2: límite $4.000.000, interés mensual 3%.

**a) Flujo con anticipo, sin costo financiero** (todos los valores en miles de $):

| | mes 0 | mes 1 | mes 2 | mes 3 | mes 4 | mes 5 | mes 6 |
|---|---|---|---|---|---|---|---|
| Ingresos sin anticipo | | | 4.000 | 4.500 | 4.000 | 4.000 | 3.500 |
| Anticipo (20% pagado en mes 0, devuelto como 20% de quita en cada certificado) | 4.000 | 0 | -800 | -900 | -800 | -800 | -700 |
| Ingresos netos | 4.000 | 0 | 3.200 | 3.600 | 3.200 | 3.200 | 2.800 |
| Egresos | -1.000 | -2.500 | -4.000 | -4.000 | -5.500 | | |
| **Flujo mensual** | **3.000** | **-2.500** | **-800** | **-400** | **-2.300** | **3.200** | **2.800** |
| **Flujo acumulado** | **3.000** | **500** | **-300** | **-700** | **-3.000** | **200** | **3.000** |

El máximo descubierto (sin intereses) es **-3.000** en el mes 4.

**b) Elección de línea de crédito:** como el máximo requerimiento financiero llega a $3.000.000, la **Línea 1 (límite $2.000.000) no alcanza a cubrir el déficit del mes 4**; hay que contratar la **Línea 2** (límite $4.000.000, interés 3% mensual), la única que cubre el pico de necesidad aunque tenga tasa más alta.

**c) y d) Intereses e importe máximo, agregando costo financiero mes a mes** (interés = 3% del saldo deudor acumulado del mes anterior, capitalizado):

| | mes 0 | mes 1 | mes 2 | mes 3 | mes 4 | mes 5 | mes 6 |
|---|---|---|---|---|---|---|---|
| Costo financiero | 0 | 0 | 0 | -9 | -21 | -90 | 0 |
| Flujo acumulado c/interés | 3.000 | 500 | -300 | -709 | **-3.030** | 80 | 2.880 |

**c) Total de intereses previstos = -120 (mil $).**

**d) Monto máximo a utilizar de la línea de crédito (incl. intereses) = -3.030 (mil $).**

---

## III. Garantías

**Datos de base:** Costo=$10.000.000; Beneficio=15% **sobre venta** ⇒ Venta sin IVA `P = Costo/(1-0,15) = $11.764.706`; IVA 22% = $2.588.235; Monto Imponible mano de obra=$2.000.000, Leyes Sociales 75,8% (incl. 4% caja profesionales) = $1.516.000. **Precio total (IVA y LLSS incl.) = $15.868.941.** Costo de constitución de cualquiera de las 3 garantías (Fianza BSE): **1,5% anual del monto a garantizar**, por el tiempo que está vigente.

**a) Fiel Cumplimiento** — monto fijo, 5% del precio final, vigente 12 meses (de Inicio a Recepción Provisoria):
`Monto = 5%×15.868.941 = $793.447` → `Costo = 793.447×1,5% = **$11.902**`.

**b) Buena Ejecución (fondo de reparo)** — se retiene 5% de cada certificado, por lo que el monto garantizado **crece linealmente de 0 a 5% del precio durante los 12 meses de obra** (I→RP), y luego se **mantiene constante en el 5% del precio durante los 24 meses de garantía** (RP→RD):
- Tramo I→RP (12 meses): monto medio = 5%/2 × 15.868.941 = $396.724 → costo = 396.724×1,5% = **$5.951**.
- Tramo RP→RD (24 meses): monto medio = 5% × 15.868.941 = $793.447 → costo = 793.447×1,5%×2 años = **$23.803**.
- **Costo total Buena Ejecución = 5.951+23.803 = $29.754.**

**c) Anticipo** — se garantiza el 100% del anticipo (10% del precio sin IVA), devuelto progresivamente conforme se descuenta de los certificados. Dos formas de estimar el monto medio, según el detalle de devolución dado (la planilla oficial trae ambas variantes):

*c.1) Devolución escalonada real (4 tramos de 3 meses, según el cronograma de certificación):*
Anticipo = 10%×11.764.706 = $1.176.471. Saldo pendiente de garantizar por tramo: 10% / 7,5% / 5% / 2,5% del precio (uno por trimestre) → monto medio mensual = promedio de los 4 tramos = **$735.294**. Costo = 735.294×1,5% (12 meses) = **$11.029**.

*c.2) Simplificación lineal (devolución proporcional uniforme, monto medio = 50% del anticipo):*
Monto medio = 50%×1.176.471 = $588.235. Costo = 588.235×1,5% = **$8.824**.

*(Ambas variantes están en la planilla oficial; la (c.1), con el cronograma real de devolución, es la más precisa y la que corresponde reportar como respuesta principal.)*

**Costo total de garantías = Fiel Cumplimiento + Buena Ejecución + Anticipo = 11.902+29.754+11.029 = $52.685** (usando la variante c.1).

---

## IV. Régimen Salarial (sin solución oficial — teórico, criterio de la Guía)

**a) Sistema de remuneración Ley 14.411:** cubre a los trabajadores de la industria de la construcción. Rasgos principales: (1) categorización por oficio y tarea (peón, medio oficial, oficial, capataz, etc.) con salarios mínimos por categoría fijados en Consejos de Salarios (Grupo 37); (2) el "monto imponible" de aportes se calcula como jornales + un adicional ficto en sustitución de beneficios que en otras industrias se pagan aparte (aguinaldo, licencia, salario vacacional, feriados) — en la construcción se paga **todo dentro del jornal**, elevando el "monto imponible" a un ~80% del costo de mano de obra abonado (ver Guía secc. 5 y 6); (3) aporte unificado patronal (Ley 14.411) que sustituye a los aportes tradicionales de BPS + rubros propios del sector (fondo social de la construcción, seguro de paro especial, etc.), hoy ~75,8% sobre el monto imponible (incluye 4% Caja de Profesionales Universitarios cuando corresponde); (4) la Caja de Industria y Comercio no aplica — es la BPS Construcción quien administra los aportes.

**b) Convenio Colectivo de la Construcción (Grupo 37):** intervienen tripartitamente (i) representantes de las cámaras empresariales (CCU/Liga de la Construcción), (ii) el SUNCA (sindicato de trabajadores), y (iii) el Poder Ejecutivo (MTSS) como mediador/homologador. Principales temas tratados: escala salarial por categoría/oficio, ajustes/correctivos periódicos por inflación, condiciones de trabajo y seguridad e higiene, régimen de licencias adicionales propio del sector, presentismo, viáticos y transporte, categorización y pases de categoría, y disposiciones sobre despido/aviso previo específicas de la actividad (alta rotación de obra en obra).

## V. Materiales (sin solución oficial — teórico, criterio de la Guía)

Para que los materiales de una obra estén correctamente:
- **a) Identificados:** definir con precisión marca/tipo/calidad/norma técnica exigida (planos y especificaciones técnicas), de modo que la cotización sea comparable entre proveedores y no haya ambigüedad sobre qué se está comprando.
- **b) Cuantificados:** obtener el metraje/cómputo métrico de cada material a partir de planos y planillas, **incluyendo desperdicios** (roturas, recortes, mermas de manipuleo y colocación) — nunca el metraje "neto" de proyecto sin más.
- **c) Valorados:** cotizar a precio de mercado vigente (varios proveedores), incluyendo todos los costos hasta que el material esté disponible en obra: flete, seguro de transporte, impuestos (IVA, aranceles si es importado), acopio/almacenaje, y mermas de estadía si aplica.

---

## Resumen de resultados

| Parte | Resultado |
|---|---|
| I.a Volumen hormigón | **25,20 m³** |
| I.b Encofrado | **126,00 m²** — Tenor **5,00 m²/m³** |
| I.c Acero | **2.177,28 kg** — Cuantía **86,40 kg/m³** |
| II.a Flujo acum. máx. descubierto (sin interés) | **-3.000 (mil $)** |
| II.b Línea a usar | **Línea 2** (la Línea 1 no cubre el pico) |
| II.c Intereses totales | **-120 (mil $)** |
| II.d Monto máx. de línea a usar (con interés) | **-3.030 (mil $)** |
| III.a Fiel Cumplimiento | **$11.902** |
| III.b Buena Ejecución | **$29.754** |
| III.c Anticipo | **$11.029** (o $8.824 en la variante simplificada) |
| III Total garantías | **$52.685** |
