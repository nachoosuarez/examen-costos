# Examen Costos — Diciembre 2024 (18/12/2024) — Resolución

Fuente: `Examen Costos dic-2024.pdf` (letra completa + Anexo I) y `Examen Costos 12-2024 - Preg.
I,II,,IV,V.pdf` (planilla de solución oficial de las partes I, II, IV y V con los valores ya calculados, usada
para verificar el desarrollo). La Parte III fue eliminada antes del examen (no existe). La Parte VI no tiene
solución oficial; se resolvió con criterio propio.

Puntuación: I-25, II-10, IV-20, V-20, VI-15 (total 90). Aprobación: 50 puntos.

---

## I – Metraje (losa L201) — ✅ verificado contra solución oficial

**Datos:** recubrimientos despreciables; ganchos 10Φ; varillas comerciales de 12 m; empalme 50Φ; tabla
de densidad/desperdicio por diámetro.

**Lectura del plano (Anexo I):** L201 es una losa de corredor/pasillo, larga y angosta, contenida en sus
4 lados por vigas: V.208 (15×50, arriba), V.211 (15×50, abajo), V.251 (15×55, izquierda) y V.252 (18×30,
derecha, límite con L202). El criterio de la guía (losa = superficie **entre vigas**) se aplica restando el
ancho de cada viga limítrofe a las cotas de eje a eje del plano:

| Dirección | Cota eje-a-eje | − anchos de vigas limítrofes | Vano libre |
|---|---|---|---|
| Ancho (b) | 170 cm | − 15 (V.251) − 18 (V.252) | **137 cm = 1,37 m** |
| Largo (L) | 1.530 cm | − 15 (V.208) − 15 (V.211) | **1.500 cm = 15,00 m** |
| Espesor (e) | | (dato del plano) | **0,12 m** |

- **Volumen hormigón** = L×b×e = 15,00×1,37×0,12 = **2,466 m³**.
- **Encofrado**: la losa está contenida por vigas en los 4 lados (no hay laterales expuestos) → solo se
  encofra la cara inferior = L×b = 15,00×1,37 = **20,55 m²**.

**Armaduras** — malla Ø10 en ambas direcciones (una sola capa, a diferencia de Marzo-2025):
- **Este-Oeste** (barras cortas que cruzan el ancho de la losa, repetidas a lo largo del largo de 15 m):
  paso 0,15 m → cantidad = redondeo hacia arriba(15/0,15)+1 = **101 barras**, cada una con 2 ganchos
  (10Φ=0,10m c/u) y sin empalme (bar corta) → **355,52 m totales → 242,46 kg con desperdicio**.
- **Norte-Sur** (barras largas que corren a lo largo del largo de 15 m, repetidas a lo ancho de 1,37 m):
  paso 0,20 m → cantidad = redondeo hacia arriba(1,37/0,20)+1 = **8 barras**, cada una con 2 ganchos y
  **1 empalme** (50Φ=0,50m, porque la barra supera los 12 m comerciales) → **129,92 m totales →
  88,61 kg con desperdicio**.

Fórmula usada para el total de metros (consistente con la guía, sección 1): `L_tot = Cantidad×L_tramo +
Cantidad×Ganchos×10Φ + Cantidad×Empalmes×50Φ`.

**Total acero (kg con desp) = 242,46 + 88,61 = 331,07 kg.**

### Resultados finales

| Magnitud | Valor |
|---|---|
| Volumen hormigón | **2,466 m³** |
| Encofrado | **20,55 m²** |
| Acero total | **331,07 kg** |
| **Tenor** (encof/vol) | **8,33 m²/m³** |
| **Cuantía** (acero/vol) | **134,25 kg/m³** |

**¿Son esperables?** Cuando el encofrado es solo la cara inferior (losa contenida en los 4 bordes), el
tenor es matemáticamente ≈1/espesor (Encofrado=L×b=Área; Volumen=Área×e ⟹ Tenor=Área/(Área×e)
=1/e = 1/0,12 = 8,33 — **coincide exactamente**). Es un tenor **alto en comparación con losas de 15-20
cm** de espesor porque **esta losa es más delgada (12 cm)**, típica de una losa de corredor/pasillo con
poca carga — a menor espesor, mayor tenor, es geométricamente esperable, no un error. La cuantía
(134,25 kg/m³) también es relativamente alta para una losa de una sola capa: se explica porque es una
**losa angosta y corta**, donde los ganchos y empalmes (que no aportan superficie de hormigón)
representan una fracción mayor del peso total del acero que en una losa grande — el "efecto de borde"
pesa proporcionalmente más en piezas pequeñas.

---

## II – Consumos Unitarios (por m³ de losa) — ✅ verificado contra solución oficial

**Datos de rendimiento:** Pasta hormigón: 5,00 hs/m³ Of. Carpintero + 3,00 hs/m³ Ayudante. Encofrado:
0,90 hs/m² cada uno (Carpintero y Ayudante). Hierro: 0,04 hs/kg cada uno (Herrero y Ayudante). Tabla
de pino 2,40×0,15m (0,36 m²), desperdicio 10%, 3 reúsos. Hormigón premezclado: desperdicio 5%.

**Paso a paso (método de la guía, tipo 2), usando tenor=8,33 m²/m³ y cuantía=134,25 kg/m³ de la Parte I:**

| Insumo | Fórmula | Consumo unitario |
|---|---|---|
| Of. Carpintero | 1×5,00 + 8,33×0,90 | **12,50 hs/m³** |
| Ayudante | 1×3,00 + 8,33×0,90 + 134,25×0,04 | **15,87 hs/m³** |
| Of. Herrero | 134,25×0,04 | **5,37 hs/m³** |
| Hormigón premezclado | 1×(1+5%) | **1,05 m³/m³** |
| Hierro | = cuantía | **134,25 kg/m³** |
| Tabla de pino | (8,33×1,10)/(0,36×3) | **8,49 unidades/m³** |

Mano de obra total = 15,87+12,50+5,37 = **33,74 HH/m³**.

**Consumo total para toda la losa (×2,466 m³):** Ayudante 39,14 hs · Of. Carpintero 30,83 hs · Of. Herrero
13,24 hs · Hormigón premezclado 2,59 m³ · Hierro 331,07 kg (=total acero de la Parte I ✓) · Tabla de
pino 20,93 unidades.

---

## III – (No existe, eliminada previo al examen)

---

## IV – Garantías (edificio de viviendas privado) — ✅ verificado contra solución oficial

**Datos:** Costo sin IVA = $200.000.000; Mano de Obra Imponible = $40.000.000; Beneficio 15% sobre
venta; IVA 22%; costo del seguro de fianza (BSE) 2% anual del monto a garantizar en los tres casos.
Plazo de ejecución (I→RP) = 15 meses; plazo de garantía (RP→RD) = 18 meses.

**Paso previo — armar el precio base:**
1. Venta sin IVA (P) = Costo/(1−15%) = 200.000.000/0,85 = **$235.294.118**.
2. IVA = 22%×P = **$51.764.706** → Venta con IVA = **$287.058.824**.
3. Leyes Sociales sobre M.O. Imponible: **75,8%** (obra de arquitectura/vivienda) × 40.000.000 =
   **$30.320.000** → Venta total con IVA y LLSS = 287.058.824+30.320.000 = **$317.378.824**.

### a) Fiel Cumplimiento de Contrato

Base: Precio con IVA y LLSS ($317.378.824). Monto a garantizar = 10% = **$31.737.882**. Perfil:
**constante** desde la firma (Inicio) hasta la Recepción Provisoria (15 meses; la RP coincide con el fin de
obra, no hay tramo adicional).

Costo = Monto × tasa anual × (meses/12) = 31.737.882 × 2% × (15/12) = **$793.447**.

### b) Buena Ejecución (Fondo de Reparo)

Base: Precio con IVA y LLSS. Monto máximo = 5% de cada certificado = 5%×317.378.824=$15.868.941.
Perfil: **rampa creciente de 0 a 5% entre I y RP** (certificación uniforme ⟹ crecimiento lineal, monto
medio = 2,5%), luego **constante al 5% entre RP y RD** (18 meses, el fondo se retiene hasta la
recepción definitiva).

- Tramo I→RP: monto medio = 2,5%×317.378.824 = $7.934.471 → costo = 7.934.471×2%×(15/12) =
  **$198.362**.
- Tramo RP→RD: monto medio = 5%×317.378.824 = $15.868.941 → costo = 15.868.941×2%×(18/12) =
  **$476.068**.
- **Costo total Buena Ejecución = 198.362+476.068 = $674.430.**

### c) Anticipo (100% del anticipo)

Base: Precio **sin** IVA ni LLSS ($235.294.118, dato del enunciado). Monto del anticipo = 20% =
$47.058.824. Perfil: **rampa decreciente de 20% a 0 entre I y RP** (se devuelve en cada certificado
durante los 15 meses de ejecución, certificación uniforme ⟹ decrecimiento lineal), monto medio=10%.

Costo = (10%×235.294.118) × 2% × (15/12) = 23.529.412 × 2,5% = **$588.235**.

### Costo total de garantías

**793.447 + 674.430 + 588.235 = $2.056.112**, equivalente a 2.056.112/317.378.824 = **0,65% del
precio de venta** — dentro del rango razonable de 0,5%-1,5% mencionado en la guía (sección 7).

---

## V – Punto de Equilibrio — ✅ verificado contra solución oficial

### a) Definición

Ver definición general en la Guía de Ejercicios Tipo, sección 11: nivel de producción/venta donde
Ingresos Totales = Costos Totales (CF+CV), resultado nulo.

**Datos:** CF mensual = $300.000 (CF anual = $3.600.000); CV unitario = $30/unidad; producción
máxima 1 turno = 3.000.000 unidades/año.

### b) Precio unitario para que el equilibrio se alcance al 50% de la capacidad

Producción de equilibrio = 50%×3.000.000 = **1.500.000 unidades/año**.

En el equilibrio: `Venta = Costo Total` → `Pu × 1.500.000 = CF + CV×1.500.000`
- CV total = 1.500.000×30 = $45.000.000.
- Costo total = 3.600.000 + 45.000.000 = **$48.600.000**.
- **Pu = 48.600.000 / 1.500.000 = $32,40/unidad.**

### c) Margen máximo posible sin aumentar capacidad (1 turno, se vende el 100% de lo producido)

Con Pu=$32,40 fijo (el establecido en b) y producción/venta a full capacidad (3.000.000 u/año):
- Venta total = 3.000.000×32,40 = **$97.200.000**.
- Costo Variable Total = 3.000.000×30 = $90.000.000. Costo Fijo Total = $3.600.000 (no cambia).
- **Beneficio Total = 97.200.000 − 90.000.000 − 3.600.000 = $3.600.000/año**, equivalente a
  **3,70% sobre venta** (3.600.000/97.200.000).

### d) Mismo análisis agregando un segundo turno (capacidad duplicada, CF +$50.000/mes)

Nueva capacidad = 6.000.000 u/año. Nuevo CF anual = 3.600.000 + (50.000×12) = **$4.200.000**. Se
mantiene el mismo precio unitario ($32,40, ya fijado en b) y se vende el 100% de lo producido:
- Venta total = 6.000.000×32,40 = **$194.400.000**.
- Costo Variable Total = 6.000.000×30 = $180.000.000. Costo Fijo Total = $4.200.000.
- **Beneficio Total = 194.400.000 − 180.000.000 − 4.200.000 = $10.200.000/año**, equivalente a
  **5,25% sobre venta**.

**Conclusión:** agregar el segundo turno casi **triplica el beneficio anual** ($3,6M → $10,2M) y además
**mejora el margen sobre venta** (3,70%→5,25%), porque el costo fijo adicional ($600.000/año) es
proporcionalmente mucho menor que el volumen de venta adicional que genera — típico efecto de
**apalancamiento operativo**: una vez superado el punto de equilibrio, cada unidad extra vendida aporta
directamente su margen de contribución (Pu−Cvu=32,40−30=$2,40/u) casi íntegro al beneficio.

---

## VI – Varios

### a) Finalidad de las fórmulas paramétricas y expresión genérica

(Ver desarrollo completo en la Guía de Ejercicios Tipo, sección 8, y en `Soluciones/202503 Ex Marzo/`.)
Trasladan al precio contractual las variaciones de costo de los insumos principales entre la oferta y el
momento de pago, evitando que contratista o contratante asuman un riesgo de costo que no controlan.
Expresión genérica **sin ajuste de costos financieros** (es decir, sin un término específico de interés/
costo del dinero, solo materiales y mano de obra):

`Pn = P0 × [a·(Jn/J0) + b·(M1n/M10) + c·(M2n/M20) + ... + z·(Zn/Z0)]`, con `a+b+c+...+z = 1`.

### b) Coeficientes de movimiento de tierra: esponjamiento, compactación y aporte

Los tres se definen respecto al mismo volumen de referencia: el **volumen en banco** (material en su
estado natural, sin remover, "in situ").

- **Coeficiente de Esponjamiento (Ce)** = Volumen suelto / Volumen en banco. Es **>1**: al remover el
  material, este pierde compacidad natural y ocupa más volumen (más aire entre partículas).
- **Coeficiente de Compactación (Cc)** = Volumen compactado / Volumen en banco. Es **<1**: al
  compactar mecánicamente (rodillo, pisón), el material queda más denso que en su estado natural.
- **Coeficiente de Aporte (Ca)** = Volumen compactado / Volumen suelto. Es el que se usa para pasar
  de "cuánto material compactado necesito" a "cuánto material suelto tengo que transportar" (ver
  Guía, sección 13).

**Relación matemática:** como los tres se refieren al mismo volumen en banco, `Ca = Cc/Ce`
(equivalente a `Cc = Ca × Ce`), porque: Cc = V_compactado/V_banco = (V_compactado/V_suelto) ×
(V_suelto/V_banco) = Ca × Ce.

### c) Clasificación de los costos por Naturaleza en el presupuesto de una obra

Según el criterio usado consistentemente en el material del curso (ver tabla "Resumen de Insumos" de
la Clase 20 y las tablas de costo directo de Marzo-2025/Dic-2025), los costos de una obra se agrupan
por naturaleza en:

**Costos Directos** (imputables directamente a cada tarea/rubro ejecutado):
1. **Mano de Obra** — jornales del personal afectado directamente a la ejecución.
2. **Materiales** — insumos que quedan incorporados a la obra (cemento, hierro, agregados, etc.).
3. **Equipos** — costo horario de la maquinaria propia o alquilada usada en la ejecución.
4. **Suministros y Subcontratos** — provisiones e instalaciones a cargo de terceros (ascensores,
   instalaciones especializadas, estructuras metálicas, etc.).
5. **Varios** — insumos menores no clasificables individualmente en las categorías anteriores.

**Costos Indirectos** — gastos que no se pueden asignar a una tarea específica pero son necesarios para
ejecutar la obra en su conjunto (dirección de obra, administración, obrador, seguros/garantías, gastos
generales de la empresa prorrateados, etc.). Se suman al costo directo total y, junto con el **Beneficio**
(margen sobre venta), determinan el precio de venta final.

---

## Resumen de resultados

| Parte | Resultado clave |
|---|---|
| I | Vol. 2,466 m³ · Encof. 20,55 m² · Acero 331,07 kg · Tenor 8,33 m²/m³ · Cuantía 134,25 kg/m³ |
| II | Mano de obra 33,74 HH/m³ · Hormigón premezclado 1,05 m³/m³ · Hierro 134,25 kg/m³ · Tabla de pino 8,49 u/m³ |
| IV | Costo total de garantías = **$2.056.112** (0,65% del precio de venta) |
| V | Precio equilibrio 50% cap. = $32,40/u · Beneficio 1 turno = $3,6M (3,70%) · Beneficio 2 turnos = $10,2M (5,25%) |
| VI | Fórmula paramétrica sin costo financiero, Ca=Cc/Ce, clasificación de costos por naturaleza (5 directos + indirectos) |
