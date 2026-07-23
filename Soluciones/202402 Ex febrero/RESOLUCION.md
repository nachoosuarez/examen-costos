# Examen Costos — Febrero 2024 (30/01/2024)

Verificado contra solución oficial (planilla de cálculo incluida en `Examen Costos 02-2024 - Preg. I,II,III,VI,V.pdf` — cubre I, II, III, IV(Garantías) y V; la Parte VI (Régimen Salarial, teórica) no viene con solución oficial en el repo, se responde con el criterio de la Guía).

---

## I – Metraje (20 pts)

**Enunciado:** volumen de hormigón, tenor de encofrado y cuantía de hierro de la losa L104 (Anexo 1). Ganchos=10Φ, varilla comercial 12m.

**Losa L104 — plano:** losa de 8,00×5,00m entre ejes de vigas (V104/V108 en las direcciones cortas, V154/V155 en las largas), con el mismo tipo de notación en "cruz" en el centro del paño (Φ10 arriba, Φ12 a la izquierda, y los números "16 15" y "26" debajo) que ya apareció sin decodificar del todo en Ene-2026/Dic-2024/Jul-2024. **En este examen se logró decodificar parcialmente**, comparando contra la planilla oficial: el número **"26" = paso de 0,26m de la armadura Φ10** ("Largo") y el número **"15" = paso de 0,15m de la armadura Φ12** ("Ancho") — ambos coinciden exactamente con el paso oficial de cada familia. El número "16" queda sin explicación clara (no coincide con ningún paso, cantidad ni longitud de la planilla oficial). Las armaduras Φ6 (bordes norte/sur) y Φ8 (este/oeste, con barra doblada) sí tienen rótulo explícito y directo en el plano ("Φ6/30" y "Φ8/25"), sin ambigüedad.

**Volumen y encofrado** (losa suspendida en sus 4 lados → Tenor=1/espesor, atajo ya visto en Dic-2024):

| Id | L (m) | b (m) | h (m) | V (m³) | Encof (m²) |
|---|---|---|---|---|---|
| Losa | 7,80 | 4,80 | 0,16 | **5,990** | **37,44** |

*(Encof=L×b=7,80×4,80=37,44 (losa contenida en los 4 lados por vigas, solo encofrado inferior) → Tenor=37,44/5,990=6,25=1/0,16 ✓ identidad verificada.)*

**Armadura (verificada, fórmula cant=redondeo hacia arriba(tramo/paso)+1; "Norte, sur" agrupa 2 bordes de 17 barras c/u = 34):**

| Tipo | Ø (mm) | Tramo (m) | Paso (m) | Cant. | L unit. (m) | L tot (m) | kg (c/desp) |
|---|---|---|---|---|---|---|---|
| Ancho | 12 | 7,8 | 0,15 | 53 | 5,24 | 277,72 | 271,89 |
| Largo | 10 | 4,8 | 0,26 | 20 | 8,20 | 164,00 | 111,85 |
| Este | 8 | 7,8 | 0,25 | 33 | 1,56 | 51,48 | 21,08 |
| Oeste | 8 | 7,8 | 0,25 | 33 | 2,66 | 87,78 | 35,95 |
| Norte, sur | 6 | 4,8 | 0,30 | 34 | 1,12 | 38,08 | 8,80 |

**Resultados finales:**
- Total Vol. hormigón: **5,990 m³**
- Total encofrado: **37,44 m²**
- Total acero (con desperdicio): **449,56 kg**
- **Tenor = 6,25 m²/m³** (=1/0,16, confirma la identidad de losa apoyada en 4 vigas)
- **Cuantía = 75,05 kg/m³**

---

## II – Consumos (10 pts)

**Rendimientos:** Of.Carpintero 5,00 hs/m³ pasta + 0,90 hs/m² encofrado; Ayudante 3,00 hs/m³ pasta + 0,90 hs/m² encofrado; Of.Herrero/Ayudante 0,04 hs/kg hierro. Tabla de pino 2,40×0,15m (0,36 m²), desperdicio 10%, 3 reúsos.

| Insumo | Fórmula | Cons. Unitario /m³ | Consumo Total (×5,990 m³) |
|---|---|---|---|
| Ayudante (hs) | 3,00 + 6,25×0,90 + 75,05×0,04 | **11,63** | 69,65 |
| Oficial Carpintero (hs) | 5,00 + 6,25×0,90 | **10,63** | 63,65 |
| Oficial Herrero (hs) | 75,05×0,04 | **3,00** | 17,98 |
| Hormigón premezclado (m³) | 1×1,05 | **1,05** | 6,29 |
| Hierro (kg) | = Cuantía | **75,05** | 449,56 |
| Tabla de pino (unid) | (6,25×1,10)/(0,36×3) | **6,37** | 38,13 |

**HH/m³ (horas-hombre totales por m³, todos los oficios):** 11,63+10,63+3,00 = **25,25 hs/m³**.

---

## III – Costo Financiero (20 pts)

**a) Valor Neto Actualizado (VNA):** es la suma de los valores presentes de todos los flujos (ingresos y egresos) de una inversión u obligación, descontados a una tasa de interés/descuento dada, a un momento de referencia (habitualmente el instante inicial). `VNA = Σ Flujoₜ/(1+i)ᵗ`.

**b) Caso — deuda de $1.000.000 (miles $), 3 alternativas de pago, tasa trimestral 25%:**

| | trim1 | trim2 | trim3 | trim4 | trim5 | **VNA (miles $)** |
|---|---|---|---|---|---|---|
| Deuda (referencia) | | | | | | **1.000** |
| Alternativa 1 | 400 | 300 | 300 | 200 | 200 | **813** |
| Alternativa 2 | 350 | 350 | 350 | 300 | 300 | **904** |
| Alternativa 3 | 0 | 0 | 0 | 0 | 2.000 | **655** |

*(Ejemplo de cálculo, Alt.1: 400/1,25 + 300/1,25² + 300/1,25³ + 200/1,25⁴ + 200/1,25⁵ = 320+192+153,6+81,92+65,54 = 813.)*

**b1) Orden de conveniencia para la empresa constructora (de mayor a menor VNA, quien cobra prefiere el VNA más alto):**
1. **Alternativa 2** (VNA=904) — la más conveniente.
2. Alternativa 1 (VNA=813).
3. **Alternativa 3** (VNA=655) — la menos conveniente (a pesar de sumar el mayor monto nominal, $2.000, todo llega al final del quinto trimestre y con alta tasa de descuento trimestral eso pesa mucho).

**b2) ¿Alguna alternativa indemniza más que el costo del dinero?** Ninguna: las 3 alternativas tienen VNA (813, 904, 655) **por debajo** de los $1.000 de la deuda original. Como ninguna alcanza siquiera a igualar el valor presente de la deuda, **ninguna reconoce una indemnización mayor al costo del dinero** — todas implican una pérdida financiera para la empresa constructora frente a haber cobrado el monto completo de inmediato.

---

## IV – Garantías (15 pts)

**Enunciado:** costo total de garantías de Fiel Cumplimiento, Buena Ejecución y Anticipo (100% del anticipo). Costo sin IVA $100.000.000. Mano de Obra Imponible (dato directo) $30.000.000. Beneficio 12% s/venta. IVA 22%. Prima Seguro de Fianza BSE: 2,5% anual. Plazo ejecución (I→RP) 14 meses, garantía (RP→RD) 18 meses.

**1) Armado del precio:**

| Concepto | % | Monto ($) |
|---|---|---|
| Costo sin IVA | | 100.000.000 |
| Venta sin IVA (P) | 12% s/venta | 100.000.000/(1−0,12) = **113.636.364** |
| IVA | 22% | 25.000.000 |
| Venta total con IVA | | 138.636.364 |
| Mano de Obra Imponible (dato) | | 30.000.000 |
| Leyes Sociales (Obra Pública) | 71,8% | 21.540.000 |
| **Venta total, IVA y LLSS incluidos** | | **160.176.364** |

**2) a) Fiel Cumplimiento** (constante, I→RP=14 meses): Monto=10%×160.176.364=16.017.636. **Costo = 16.017.636×2,5%×(14/12) = $ 467.181**

**3) b) Buena Ejecución** (rampa 0→5% en I→RP, constante al 5% en RP→RD=18 meses): monto medio I→RP=2,5%×160.176.364=4.004.409 → costo parcial=**116.795**; monto medio RP→RD=5%(máximo, se mantiene)=8.008.818 → costo parcial=8.008.818×2,5%×(18/12)=**300.331**. **Costo Buena Ejecución = 116.795+300.331 = $ 417.126**

**4) c) Anticipo** (100% del anticipo, base Precio SIN IVA ni LLSS=113.636.364; rampa decreciente de 20%→0 durante I→RP=14 meses, se devuelve en cada certificado): Monto máximo=20%×113.636.364=22.727.273; **monto medio=10%×113.636.364=11.363.636** (mitad del máximo, por ser rampa lineal a 0). **Costo = 11.363.636×2,5%×(14/12) = $ 331.439**

**Costo Total de Garantías = 467.181 + 417.126 + 331.439 = $ 1.215.746** (0,76% de la venta total con IVA y LLSS).

---

## V – Punto de Equilibrio (15 pts)

**a) Definición:** el Punto de Equilibrio de un sistema de producción es el nivel de producción/venta en el cual los **Ingresos Totales igualan a los Costos Totales** (fijos+variables) — resultado (beneficio) nulo. Por debajo de ese nivel la empresa pierde dinero; por encima, gana.

**Datos:** Cvu=$20/u; CF=$200.000/mes=$2.400.000/año; Producción máxima=2.000.000 u/año.

**b) Precio para que el equilibrio se dé al 50% de la capacidad:**
`Q_equilibrio = 50%×2.000.000 = 1.000.000 u/año`
`Pu×Q = CF + Cvu×Q → Pu = (CF+Cvu×Q)/Q = (2.400.000+20×1.000.000)/1.000.000`
**Pu = $ 22,40/unidad**

**c) Beneficio máximo posible sin ampliar capacidad** (vendiendo el 100% de la producción máxima, 2.000.000 u, al mismo Pu=$22,40):
- Venta total = 22,40×2.000.000 = $44.800.000
- Costo Variable Total = 20×2.000.000 = $40.000.000
- Costo Fijo Total = $2.400.000
- **Beneficio Total = 44.800.000−40.000.000−2.400.000 = $ 2.400.000/año**
- **Margen sobre venta = 2.400.000/44.800.000 = 5,36%**

---

## VI – Régimen Salarial (10 pts) *(teórico, sin solución oficial en el repo)*

**a) Principales características del sistema de remuneración del personal amparado por la Ley 14.411:** el personal con tareas directas de obra tributa el **Aporte Unificado de la Construcción** (sustituye a los aportes de Industria y Comercio). La remuneración se rige por **categorías y laudos** fijados en el Convenio Colectivo (jornal por hora según categoría, de "Peón" a "Oficial Especializado"), y se complementa con componentes obligatorios: presentismo (semanal y mensual), feriados no laborables pagos, tickets de alimentación, ropa de trabajo/herramientas/transporte, media hora de descanso paga. El Monto Imponible para leyes sociales integra la mayoría de estos ítems (ver Guía sección 5). Los aportes patronales financian además los **Fondos Sociales de la Construcción** (FOSVOC, FSC, FOCAP, FOCER).

**b) Partes del Convenio Colectivo de la Construcción (Grupo 37) y aspectos que trata:** convenio **tripartito** entre las **Empresas** (cámaras empresariales del sector), los **Trabajadores** (representados por el sindicato SUNCA) y el **MTSS/Poder Ejecutivo** (que convoca la negociación y homologa el acuerdo). Se renueva periódicamente (rondas de negociación colectiva, históricamente cada 2-3 años). Principales aspectos que trata: categorías laborales y sus laudos (jornal por hora), mecanismo de ajuste salarial (ligado a metas de inflación del BCU), régimen de licencias, condiciones generales de trabajo y seguridad, y los Fondos Sociales de la Construcción.

---

## Resumen ejecutivo del examen

| Parte | Resultado clave |
|---|---|
| I – Metraje | Vol=5,990 m³; Encof=37,44 m²; Tenor=6,25 m²/m³ (=1/e); Acero=449,56 kg; Cuantía=75,05 kg/m³ |
| II – Consumos | Ayudante 11,63 hs/m³; HH/m³ total=25,25 |
| III – Costo Financiero | Alt.2 (VNA=904) la más conveniente; ninguna alternativa supera el costo del dinero |
| IV – Garantías | FC $467.181 + BE $417.126 + Anticipo $331.439 = **$1.215.746** |
| V – Punto de Equilibrio | Precio equilibrio a 50% capacidad = **$22,40/u**; beneficio máx. = $2.400.000/año (5,36% s/venta) |
| VI – Régimen Salarial | Aporte Unificado Ley 14.411; Convenio Colectivo tripartito (Empresas-SUNCA-MTSS) |
