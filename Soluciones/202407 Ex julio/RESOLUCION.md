# Examen Costos — Julio 2024 (01/08/2024)

Verificado contra solución oficial (planilla de cálculo incluida en el propio PDF `Examen Costos 07-2024 - Preg. I,II,III,IV,V y VI.pdf`, páginas 1-3). Todos los resultados de este archivo son los oficiales.

---

## I – Metraje (20 pts)

**Enunciado:** determinar volumen de hormigón, tenor de encofrado y cuantía de hierro de la losa L204 (Anexo 1), **incluyendo los bordes que hacen de escalón entre losas**. Ganchos=10Φ, empalme 50cm (Φ6/Φ8) o 70cm (Φ12), varillas comerciales de 12m.

**Losa L204 — nota sobre el plano:** el Anexo usa la misma notación de planilla en "cruz" (Φ / paso en cuadrícula junto a las cotas de armado) que ya había aparecido en Dic-2024 y Ene-2026 sin poder decodificarse con certeza. En este examen, sin embargo, el PDF de la letra trae la **planilla de cálculo ya resuelta** (Preg. I,II,...), así que se usa directamente esa desagregación oficial (columnas Diámetro | Tramo | Paso | Cantidad | Ganchos | Longitud | kg) en vez de re-derivar cada cota del plano — el objetivo de este archivo es que quede clara la **metodología de armado de la planilla tipo** (ver Guía sección 1), no inventar una lectura del plano que no se puede confirmar al 100%. *(Tercer caso con esta notación en "cruz" — sigue pendiente de decodificar de forma cerrada; ver nota al final de la Guía.)*

**Volumen y encofrado:**

| Id | L (m) | b (m) | h (m) | V (m³) | Encof (m²) |
|---|---|---|---|---|---|
| Losa | 2,75 | 1,81 | 0,15 | **0,747** | 4,98 |
| Bordes (escalón) | 6,67 | 0,15 | 0,35 | **0,350** | 3,67 |
| **Total** | | | | **1,097** | **8,646** |

**Armadura (planilla, con desperdicio ya incluido en "kg con desp"):**

| Id | Tipo | Ø (mm) | Tramo (m) | Paso (m) | Cant. | Ganchos | L (m) | L tot (m) | kg (c/desp) |
|---|---|---|---|---|---|---|---|---|---|
| Losa | Ancho | 12 | 2,75 | 0,20 | 15 | 2 | 2,33 | 34,95 | 34,22 |
| Losa | Largo | 12 | 1,81 | 0,20 | 11 | 0 | 4,65 | 51,15 | 50,08 |
| Losa | Este/Oeste | 10 | 1,81 | 0,20 | 22 | 2 | 2,35 | 51,70 | 35,26 |
| Losa | Norte | 8 | 2,75 | 0,20 | 15 | 2 | 1,77 | 26,55 | 10,87 |
| Losa | Sur | 8 | 2,75 | 0,20 | 15 | 2 | 2,31 | 34,65 | 14,19 |

**Resultados finales:**
- Total volumen de hormigón: **1,097 m³**
- Total encofrado: **8,65 m²**
- Total acero (con desperdicio): **144,61 kg**
- **Tenor de encofrado = 8,65 / 1,097 = 7,88 m²/m³**
- **Cuantía de acero = 144,61 / 1,097 = 131,85 kg/m³**

Valores dentro del rango esperado para una losa suspendida con bordes de escalón (tenor y cuantía más altos que una losa simple, coherente con el hierro extra de los bordes y el doble armado Este/Oeste).

---

## II – Movimiento de suelos (15 pts)

**Enunciado:** platea de hormigón 35m×14m sobre terreno arcilloso con 2% de pendiente en el sentido de la dimensión mayor (35m). Estructura: hormigón 15cm + balasto 25cm. Terreno natural en su punto más bajo a 60cm bajo la cara superior de la losa; capa vegetal 20cm. Camión de 10 m³. No se consideran taludes.

**Datos:**

| Material | Esponjamiento (Ce) | Compactación (Cc) | Aporte (Ca) |
|---|---|---|---|
| Tierra (capa vegetal) | 1,3 | 0,7 | 1,1 |
| Balasto | 1,5 | 0,9 | 0,8 |
| Arcilla | 1,4 | 0,6 | 1,1 |

**Área de la platea:** 35×14 = 490 m².

**Paso a paso (oficial):**

1. **Capa vegetal** (se retira toda, 20cm en toda el área): Vol. en sitio = 490×0,20 = **98,0 m³**. Es material que **sale** de la obra → se lleva a volumen suelto con el coeficiente de **Esponjamiento**: 98,0×1,3 = **127,4 m³ sueltos** = Movilizar.
2. **Balasto** (capa de aporte, 25cm compactados en toda el área): Vol. en sitio (compactado, la capa terminada) = 490×0,25 = **122,5 m³**. Es material que **entra** y se compacta → el volumen suelto a transportar en camión es mayor que el compactado: 122,5 / 0,9 = **136,1 m³ sueltos** = Movilizar. *(Nota: acá el coeficiente que reproduce el resultado oficial es el de la columna "Compactación" (0,9), no el de "Aporte" (0,8) — ver aclaración de terminología al pie.)*
3. **Arcilla — terraplén (relleno) vs. desmonte (excavación):** la pendiente del terreno (2% en 35m = 0,70m de desnivel) y la cota de fondo de estructura (60cm bajo la cara superior de la losa = bajo la capa de hormigón+balasto, o sea a −0,40m tomando la cara sup. de losa en 0) hacen que en la parte alta del terreno haya que **desmontar** arcilla y en la parte baja haya que **rellenar (terraplenar)** con arcilla para nivelar antes de poner el balasto:
   - Terraplén de arcilla necesario (en sitio, compactado): **56,0 m³** → suelto a transportar = 56,0 / 0,6 = **93,3 m³**.
   - Desmonte de arcilla (en sitio, banco): **31,5 m³** → suelto que produce al excavar = 31,5×1,4 = **44,1 m³**.
   - Como la arcilla excavada del desmonte se puede reutilizar como relleno del terraplén, el **movimiento neto a transportar** (import de arcilla, ya que el terraplén necesita más de lo que aporta el desmonte) es: 93,3 − 44,1 = **49,2 m³ sueltos**.

**Viajes de camión (10 m³, redondeado hacia arriba):**

| Material | Vol. suelto a movilizar (m³) | Viajes |
|---|---|---|
| Capa vegetal (retiro) | 127,4 | **13** |
| Balasto (aporte) | 136,1 | **14** |
| Arcilla (neto, import) | 49,2 | **5** |

**Aclaración de terminología (importante, ver Guía sección 13):** en este examen la tabla de coeficientes trae **3 columnas** (Esponjamiento, Compactación, Aporte) pero el coeficiente que efectivamente convierte "volumen compactado requerido" en "volumen suelto a transportar" para el balasto y el terraplén de arcilla es el de la columna **"Compactación"**, no el de "Aporte" (que en este examen no se usó en el cálculo). Esto **no coincide** con la convención de Jul-2025, donde el coeficiente usado para ese mismo pasaje se llamaba "Ca" (Aporte). **Conclusión: el nombre de la columna varía según el examen — lo que importa es identificar, por prueba con los volúmenes que da el enunciado, cuál coeficiente cumple `Vol. suelto = Vol. compactado / coeficiente` (coeficiente <1, típicamente 0,6-0,9), sin fiarse del nombre de la etiqueta.**

---

## III – Garantías (15 pts)

**Enunciado:** costo total de garantías de Fiel Cumplimiento de Contrato y Buena Ejecución (fondo de reparo), para una obra de saneamiento de la IM de Montevideo. Costo total (sin LLSS de M.O. ley 14.411): $200.000.000. Costo de M.O. sujeta a ley 14.411: $30.000.000. Beneficio 15% s/precio de venta. IVA 22%. Prima de la garantía (Seguro de Fianza BSE): 2% anual del monto a garantizar. Plazo de ejecución 14 meses (I→RP), plazo de garantía 18 meses (RP→RD). Certificación uniforme.

**1) Armado del precio de venta con IVA y LLSS:**

| Concepto | % | Monto ($) |
|---|---|---|
| Costo sin IVA | | 200.000.000 |
| Venta sin IVA (P) — Beneficio 15% s/venta | 15% | 200.000.000/(1−0,15) = **235.294.118** |
| IVA | 22% | 235.294.118×0,22 = 51.764.706 |
| Venta total con IVA | | 287.058.824 |
| Mano de Obra ley 14.411 (dato) | | 30.000.000 |
| Mano de Obra Imponible | 80% | 30.000.000×0,80 = 24.000.000 |
| Leyes Sociales (Obra Pública) | 71,8% | 24.000.000×0,718 = 17.232.000 |
| **Venta total, IVA y LLSS incluidos** | | **304.290.824** |

**2) a) Fiel Cumplimiento de Contrato** (monto constante, de I a RP):
- Monto a garantizar = 10% × 304.290.824 = **30.429.082**
- Período = 14 meses
- **Costo = 30.429.082 × 2%/año × (14/12) = $ 710.012**

**3) b) Buena Ejecución / Fondo de Reparo** (rampa 0→5% durante ejecución, luego constante al 5% durante el plazo de garantía):
- Monto máximo a garantizar = 5% × 304.290.824 = 15.214.541
- Tramo I→RP (14 meses): certificación uniforme ⇒ el monto retenido crece linealmente de 0 al máximo ⇒ **monto medio = 2,5% × 304.290.824 = 7.607.271**. Costo parcial = 7.607.271×2%×(14/12) = **177.503**
- Tramo RP→RD (18 meses): se mantiene el monto completo (5%) retenido ⇒ **monto medio = 15.214.541**. Costo parcial = 15.214.541×2%×(18/12) = **456.436**
- **Costo Buena Ejecución = 177.503 + 456.436 = $ 633.939**

**Costo Total de Garantías = 710.012 + 633.939 = $ 1.343.951** (0,47% de la venta total con IVA y LLSS — dentro del rango típico 0,5%-1,5% visto en otros exámenes, apenas por debajo por tratarse solo de 2 garantías con prima baja del 2%).

---

## IV – Subcontrato (10 pts)

**Enunciado:** indicar y describir las categorizaciones de Tipo de Subcontrato (válidas también para el contrato principal Cliente/Propietario–Contratista).

**Tipos (de la Clase de Subcontratos, con las mismas categorías usadas también para el contrato principal):**
1. **Precio Total**: el subcontratista se compromete a construir el objeto a un precio total determinado, sujeto solo a los ajustes explicitados en el contrato (ajuste paramétrico, aumentos/reducciones de alcance).
2. **Precios Unitarios**: el subcontratista se compromete a construir a los precios unitarios establecidos, ajustándose las cantidades a pagar a lo efectivamente ejecutado.
3. **"Llave en Mano"**: el subcontratista se encarga de todos o la mayoría de los trámites necesarios para realizar la obra (proyecto, ejecución, etc.) a cambio de un precio cerrado global y un plazo determinado.
4. **"Colaboración"**: el contratista mantiene algunas responsabilidades (suministros, aprobación del proyecto/partes, elección de marcas/proveedores); ambas partes deben cumplir en tiempo y forma, ya que errores/omisiones de cualquiera de las dos repercuten en el objetivo del contrato.
5. **"Par y Paso"**: se trasladan al subcontrato todas las condiciones del contrato principal (multas, garantías, proporciones, límites), pudiendo acordarse variantes puntuales (ej. plazos de pago) sin cambiar el espíritu general.
6. **"Combinación"**: las categorías anteriores suelen combinarse y no son excluyentes (ej. precio total con algunos rubros a precios unitarios, como excavación en roca o reparación de pavimentos). Si se combinan, es clave que el **texto del contrato sea coherente** con la combinación elegida, para no desvirtuarla.

---

## V – Riesgos (15 pts)

**Enunciado:** indicar y describir las etapas del Análisis y Gestión de Riesgos de un Proyecto.

1. **Identificación preliminar**: identificar todos los riesgos posibles; es muy valiosa la experiencia previa y un listado general (checklist) de riesgos típicos.
2. **Valoración y Cuantificación**: valorar y cuantificar cada riesgo en todos sus aspectos (no solo el económico — también reputacional, accidentes personales, etc.) y la responsabilidad que se asume por él.
3. **Tratamiento y Mitigación**: determinar todas las medidas razonables y posibles para (a) reducir/eliminar la probabilidad de ocurrencia, (b) reducir/eliminar los perjuicios si ocurre, (c) reducir/eliminar la responsabilidad propia sobre el riesgo.
4. **Valoración Final o Residual**: análisis conjunto de todos los riesgos con su valoración/probabilidad y posible simultaneidad, determinando el **Riesgo Máximo** y completando el Plan de Acción de Riesgos con todas las mitigaciones definidas.
5. **Gestión del Riesgo**: una vez cerrado el análisis, gestión continua del Plan de Acción de Riesgos para asegurar su cumplimiento y ajustarlo ante desvíos o modificaciones durante la obra.

---

## VI – Evaluación de una Inversión (15 pts)

**a) TIR (Tasa Interna de Retorno):** es la tasa de interés/descuento **i** para la cual el Valor Neto Actualizado (VNA) de los flujos de una inversión (ingresos−egresos de cada período) es exactamente cero. Utilidad: permite comparar la rentabilidad intrínseca del proyecto (independiente de una tasa de mercado externa) contra el costo de oportunidad del capital u otras alternativas de inversión — si la TIR de un proyecto supera la tasa mínima requerida (o la de otro proyecto alternativo), conviene esa inversión.

**b) Ecuación:**

VNA = Σ (Iₜ − Eₜ)/(1+i)ᵗ para t=0…10 (o el horizonte del proyecto) = I₀/(1+i)⁰ + I₁/(1+i)¹ + … − E₀/(1+i)⁰ − E₁/(1+i)¹ − …

**TIR** es el valor de **i** tal que: Σ (Iₜ−Eₜ)/(1+i)ᵗ = **0**

---

## Resumen ejecutivo del examen

| Parte | Resultado clave |
|---|---|
| I – Metraje | Vol=1,097 m³; Encof=8,65 m²; Tenor=7,88 m²/m³; Acero=144,61 kg; Cuantía=131,85 kg/m³ |
| II – Movimiento de suelos | 13 viajes (capa vegetal) + 14 viajes (balasto) + 5 viajes (arcilla neta) |
| III – Garantías | Fiel Cumplimiento $710.012 + Buena Ejecución $633.939 = **$1.343.951** |
| IV – Subcontratos | 6 tipos: Precio Total, Precios Unitarios, Llave en Mano, Colaboración, Par y Paso, Combinación |
| V – Riesgos | 5 etapas: Identificación, Valoración/Cuantificación, Tratamiento/Mitigación, Valoración Final, Gestión |
| VI – Inversión | TIR = i tal que VNA=0 |
