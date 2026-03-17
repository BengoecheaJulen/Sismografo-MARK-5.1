# SEISMIC · MARK 5 — Systemic Risk Intelligence

**Real-time early warning system for S&P 500 extreme volatility events.**

Live dashboard: [**SEISMIC MARK 5**](https://bengoecheajulen.github.io/Sismografo-MARK-5.1/)

Data updated daily at 22:30 CET (Mon–Fri) · GitHub-timestamped · Immutable record

---

## What is SEISMIC?

SEISMIC is a systemic risk detection system that identifies the buildup of conditions preceding market crashes, fat tails, and extreme volatility regimes in the S&P 500. It does **not** predict daily price direction — it detects when the probability of an extreme event is significantly elevated.

The model is based on a proprietary physics-derived framework that processes independent market factors daily. Its signals are **structurally decorrelated** from all standard financial models.

---

## Performance Metrics (Out-of-Sample, 2022–2025)

| Metric | Value |
|--------|-------|
| Correlation with GARCH | **0.27** (genuinely independent signal) |
| GARCH models among themselves | 0.93–0.95 (nearly identical) |
| RMSE (prediction error) | **0.088** (12.1% better than predecessor) |
| Pearson correlation with realized vol | **0.35** (out-of-sample) |
| Median lead time before crisis | **40 days** |
| Maximum lead time | **90 days** (EU Debt Crisis 2011) |
| Crisis coverage (ELEVATED+) | **89%** of historical crises detected |
| False positives vs predecessor | **−54%** reduction |
| Combined with GARCH in extreme events (σ > 0.30) | **+28.3%** RMSE improvement |
| Combined with GARCH in crisis (σ > 0.20) | **+13.0%** RMSE improvement |
| Lindblad vs classical benchmark | **+77.7%** improvement |
| Historical crises validated | GFC 2008, EU Debt 2011, COVID 2020, Inflation 2022, Tariffs 2025 |

*All metrics computed on data the model has never seen during development.*

---

## Why This Matters

Standard risk models (GARCH, EWMA, GJR-GARCH) correlate **0.93–0.95 with each other**. Adding another GARCH variant to your risk system adds almost zero new information.

SEISMIC correlates **0.27 with GARCH** — providing genuinely independent risk intelligence. When both your existing models and SEISMIC agree on elevated risk, the probability of a real crisis is significantly higher than either signal alone.

In extreme market events (σ > 0.30), combining SEISMIC with GARCH reduces prediction error by **28.3%** compared to GARCH alone. No single indicator provides this level of improvement on standard models in tail events.

---

## Alert Regime Classification — 7 States

| Color | State | Meaning |
|-------|-------|---------|
| 🟣 Purple (pulsing) | **TAIL FORMING** | 5+ consecutive critical days. Active fat tail formation. Historical: 97% crisis probability within 30 days. |
| 🔴 Red | **EXTREME TAIL** | Very high predicted volatility confirmed by market. Rare (0.1% of days). |
| 🟠 Dark orange | **CRITICAL** | High risk confirmed. 69% crisis probability within 30 days. |
| 🟠 Orange | **HIGH RISK** | Elevated risk with rising market stress. 44% crisis probability. |
| 🟡 Yellow | **ELEVATED** | Model sees risk, market starting to confirm. 24% crisis probability. |
| 🔵 Blue (bright, pulsing) | **WATCHLIST CONFIRMED** | Early warning with high escalation ratio. Probable real alert. |
| 🔵 Blue (faded, dashed) | **WATCHLIST** | Model detects something, market calm. Possible false positive. |
| 🟢 Green | **STABLE** | Normal regime. |
| ⚫ Grey | **CALM** | Very low risk. |
| ⚪ White dot | **NEXUS ALERT** | Leading indicator elevated. Typically appears 8 days before main signal rises. |

---

## How to Read the Dashboard

- **State color** is the primary signal. Orange or worse → elevated risk.
- **White dot (NEXUS ALERT)** next to a green/yellow state → the model's leading indicator is rising before the main signal. Watch closely.
- **Blue bright vs faded** → discriminates real watchlist alerts from probable false positives using internal escalation dynamics.
- **PULSE percentage** → predicted annualized volatility. Above 25% = elevated. Above 35% = serious.
- All values shown as **percentiles** (P30, P70, P90...) for intuitive interpretation.

---

## Data

- S&P 500 daily data since January 2000 (6,500+ trading days)
- 6 independent market factors
- Every daily reading is GitHub-committed with timestamp — creating an **immutable, verifiable track record**

---

## Contact

**Julen Bengoechea** — Quantitative Research

📧 [bengoecheajulen@gmail.com](mailto:bengoecheajulen@gmail.com) · 🔗 [LinkedIn](https://www.linkedin.com/in/julen-bengoechea-805382295) · 📊 [GitHub](https://github.com/BengoecheaJulen)

---

## Legal

SEISMIC is a research intelligence system. Signals do not constitute financial advice or investment recommendations. Past performance does not guarantee future results. For institutional research purposes only.

---

---

# SEISMIC · MARK 5 — Inteligencia de Riesgo Sistémico

**Sistema de alerta temprana en tiempo real para eventos de volatilidad extrema del S&P 500.**

Dashboard en vivo: [**SEISMIC MARK 5**](https://bengoecheajulen.github.io/Sismografo-MARK-5.1/)

Datos actualizados diariamente a las 22:30 CET (Lun–Vie) · Timestamp en GitHub · Registro inmutable

---

## ¿Qué es SEISMIC?

SEISMIC es un sistema de detección de riesgo sistémico que identifica la acumulación de condiciones que preceden a crashes, colas pesadas y regímenes de volatilidad extrema en el S&P 500. **No** predice la dirección diaria del precio — detecta cuándo la probabilidad de un evento extremo está significativamente elevada.

El modelo está basado en un framework propietario derivado de la física que procesa factores de mercado independientes diariamente. Sus señales están **estructuralmente descorrelacionadas** de todos los modelos financieros estándar.

---

## Métricas de Rendimiento (Fuera de Muestra, 2022–2025)

| Métrica | Valor |
|---------|-------|
| Correlación con GARCH | **0.27** (señal genuinamente independiente) |
| Modelos GARCH entre sí | 0.93–0.95 (prácticamente idénticos) |
| RMSE (error de predicción) | **0.088** (12.1% mejor que predecesor) |
| Correlación Pearson con vol realizada | **0.35** (fuera de muestra) |
| Lead time mediano antes de crisis | **40 días** |
| Lead time máximo | **90 días** (Crisis deuda europea 2011) |
| Cobertura de crisis (ELEVATED+) | **89%** de las crisis históricas detectadas |
| Falsos positivos vs predecesor | **−54%** de reducción |
| Combinado con GARCH en eventos extremos (σ > 0.30) | **+28.3%** mejora en RMSE |
| Combinado con GARCH en crisis (σ > 0.20) | **+13.0%** mejora en RMSE |
| Motor propietario vs benchmark clásico | **+77.7%** de mejora |
| Crisis históricas validadas | GFC 2008, Deuda EU 2011, COVID 2020, Inflación 2022, Aranceles 2025 |

*Todas las métricas calculadas sobre datos que el modelo nunca ha visto durante su desarrollo.*

---

## Por Qué Esto Importa

Los modelos de riesgo estándar (GARCH, EWMA, GJR-GARCH) correlacionan **0.93–0.95 entre sí**. Añadir otra variante GARCH a tu sistema de riesgo no aporta información nueva.

SEISMIC correlaciona **0.27 con GARCH** — proporcionando inteligencia de riesgo genuinamente independiente. Cuando tus modelos existentes y SEISMIC coinciden en riesgo elevado, la probabilidad de una crisis real es significativamente mayor que la de cualquier señal por separado.

En eventos de mercado extremos (σ > 0.30), combinar SEISMIC con GARCH reduce el error de predicción un **28.3%** comparado con GARCH solo. Ningún indicador individual proporciona este nivel de mejora sobre modelos estándar en eventos de cola.

---

## Clasificación de Alertas — 7 Estados

| Color | Estado | Significado |
|-------|--------|-------------|
| 🟣 Púrpura (pulsante) | **TAIL FORMING** | 5+ días críticos consecutivos. Formación activa de cola pesada. Históricamente: 97% probabilidad de crisis en 30 días. |
| 🔴 Rojo | **EXTREME TAIL** | Volatilidad predicha muy alta confirmada por mercado. Raro (0.1% de los días). |
| 🟠 Naranja oscuro | **CRITICAL** | Riesgo alto confirmado. 69% probabilidad de crisis en 30 días. |
| 🟠 Naranja | **HIGH RISK** | Riesgo elevado con estrés de mercado creciente. 44% probabilidad. |
| 🟡 Amarillo | **ELEVATED** | Modelo ve riesgo, mercado empieza a confirmar. 24% probabilidad. |
| 🔵 Azul (brillante, pulsante) | **WATCHLIST CONFIRMED** | Alerta temprana con ratio de escalada alto. Probable alerta real. |
| 🔵 Azul (apagado, punteado) | **WATCHLIST** | Modelo detecta algo, mercado en calma. Posible falso positivo. |
| 🟢 Verde | **STABLE** | Régimen normal. |
| ⚫ Gris | **CALM** | Riesgo muy bajo. |
| ⚪ Punto blanco | **NEXUS ALERT** | Indicador adelantado elevado. Aparece típicamente 8 días antes de que la señal principal suba. |

---

## Cómo Leer el Dashboard

- El **color del estado** es la señal primaria. Naranja o peor → riesgo elevado.
- **Punto blanco (NEXUS ALERT)** junto a un estado verde/amarillo → el indicador adelantado del modelo está subiendo antes que la señal principal. Vigilar de cerca.
- **Azul brillante vs apagado** → discrimina alertas watchlist reales de probables falsos positivos usando dinámica interna de escalada.
- **Porcentaje PULSE** → volatilidad anualizada predicha. Por encima de 25% = elevado. Por encima de 35% = serio.
- Todos los valores como **percentiles** (P30, P70, P90...) para interpretación intuitiva.

---

## Datos

- Datos diarios del S&P 500 desde enero de 2000 (más de 6.500 días de trading)
- 6 factores de mercado independientes
- Cada lectura diaria se registra en GitHub con timestamp — creando un **historial verificable e inmutable**

---

## Contacto

**Julen Bengoechea** — Investigación Cuantitativa

📧 [bengoecheajulen@gmail.com](mailto:bengoecheajulen@gmail.com) · 🔗 [LinkedIn](https://www.linkedin.com/in/julen-bengoechea-805382295) · 📊 [GitHub](https://github.com/BengoecheaJulen)

---

## Aviso Legal

SEISMIC es un sistema de inteligencia de investigación. Las señales no constituyen asesoramiento financiero ni recomendaciones de inversión. Rendimiento pasado no garantiza resultados futuros. Solo para fines de investigación institucional.
