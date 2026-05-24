# Prediction Playground

Repositorio con los notebooks que uso en mis vídeos sobre **Machine Learning, estadística y probabilidad aplicados al deporte**.

Aquí no hay magia: cada notebook explica paso a paso cómo construir un modelo predictivo real, desde la obtención de datos hasta la visualización de resultados. Los temas van de Fórmula 1 a fútbol, pasando por apuestas y probabilidad.

---

## Índice

| # | Notebook | Tema | Técnica |
|---|----------|------|---------|
| 01 | [GP Canadá 2026 — ¿Quién chocará contra el Muro de los Campeones?](01-muro-campeones-logistica.ipynb) | F1 | Regresión Logística |
| 02 | [¿Cómo calculan las casas de apuestas las cuotas?](02-cuotas-casas-de-apuestas.ipynb) | Fútbol / Apuestas | Modelo de Poisson |

---

### 01 · GP Canadá 2026 — Muro de los Campeones

Usa datos reales de telemetría de FastF1 para entrenar una **regresión logística** con los resultados históricos del circuito de Montreal (2018–2024). El modelo aprende qué pilotos tienen más riesgo de incidente en función de su inconsistencia en tiempos de vuelta y su velocidad punta, y predice las probabilidades para la parrilla de 2026.

**Librerías:** `fastf1`, `scikit-learn`, `pandas`, `matplotlib`

---

### 02 · ¿Cómo calculan las casas de apuestas las cuotas?

Replica, de forma transparente, el proceso que usan las casas de apuestas para fijar cuotas. Usando el **modelo de Poisson** y estadísticas reales de la UEFA Conference League 2026 (Crystal Palace vs Rayo Vallecano), calcula la probabilidad de cada marcador posible, obtiene las probabilidades de victoria y reconstruye las cuotas incluyendo el margen de la casa.

**Librerías:** `numpy`, `scipy`, `pandas`, `matplotlib`, `seaborn`

---

## Cómo usar estos notebooks

Cada notebook es autocontenido. En la primera celda encontrarás las instrucciones de instalación de dependencias. Puedes ejecutarlos en local con Jupyter o en [Google Colab](https://colab.research.google.com/) sin instalar nada.

```bash
pip install fastf1 scikit-learn pandas numpy matplotlib seaborn scipy
jupyter notebook
```
