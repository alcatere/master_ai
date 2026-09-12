# Reporte — Ejercicio 1: Perceptrón Multicapa en Iris

### 1. ¿Bajar más el error al añadir dos capas, o se estancó / empeoró? ¿Igual en NumPy y en Keras?
No bajó más; en ambos casos se estancó y empeoró:
- **NumPy:** La red simple (4x3x3) aprendió bien y redujo el error hasta ~0.06. En cambio, la red profunda (4x3x3x3x3) bajó únicamente en las primeras 10 épocas y se quedó totalmente plana en ~0.67 sin progresar.
- **Keras:** Ocurrió exactamente lo mismo. El modelo de 2 capas alcanzó un loss de 0.2099, mientras que la red con dos capas extra se estancó alrededor de la época 150 en 0.2223.

En ambas implementaciones hacer la red más profunda perjudicó el entrenamiento.

---

### 2. ¿Las curvas de la notebook 01 y de Keras se parecen con la misma topología? Si no, ¿qué diferencias de implementación podrían explicarlo (orden de los datos, inicialización, vectorización, etc.)?
No se parecen tanto. La curva de NumPy cae más rápido y llega a un valor final menor (~0.06 vs ~0.21). Esto se explica por varias diferencias:
1. **Actualización de pesos:** En NumPy es SGD puro (actualización muestra por muestra, en orden secuencial fijo 0 a 149). Keras entrena por mini-batches (batch size 32 por defecto) y aplica *shuffle* en cada época.
2. **Inicialización:** En NumPy usamos una distribución uniforme manual en $[-0.5, 0.5]$ para pesos y sesgos.
3. **Escala de la métrica:** En NumPy sumamos el error cuadrático de las 3 salidas por muestra y promediamos entre $N$. En Keras, el MSE promedia además sobre la dimensión de salida (divide entre 3), cambiando la escala numérica de la pérdida.

---

### 3. Con sigmoides apiladas y MSE, ¿tiene sentido que una red más profunda no aprenda mejor en Iris? Relaciónalo con lo que viste en las gráficas.
Sí, tiene total sentido:
1. **Desvanecimiento del gradiente:** La derivada de la sigmoide tiene un valor máximo de 0.25. Al encadenar 4 capas con sigmoide, al retropropagar el error los deltas se multiplican sucesivamente por valores $\le 0.25$. El gradiente que llega a las primeras capas es prácticamente cero, congelando el aprendizaje. Esto se refleja directamente en las gráficas de la red profunda: tras una bajada inicial mínima, la curva se vuelve completamente horizontal.
2. **Naturaleza del problema:** Iris tiene solo 150 muestras y es casi linealmente separable. No requiere abstracciones jerárquicas profundas; añadir capas solo añade parámetros innecesarios y complica la optimización.
Este tipo de problema es ideal para algoritmos más simples, y la evidencia empírica lo confirma: la red simple aprende bien, mientras que la profunda se estanca.