# Stochastic-processes
University assesments related to Stochastic processes, random walks, Markov chains and many more simulations.

# Simulación y Análisis del Paseo Aleatorio Simple (PAS)

Este repositorio contiene la implementación y el análisis visual de un **Paseo Aleatorio Simple (PAS)** en tiempo discreto, desarrollado en Python utilizando `NumPy` y `Matplotlib`. El objetivo principal es modelizar trayectorias estocásticas y comprobar empíricamente las propiedades matemáticas fundamentales del proceso.

## Características del Proyecto

* **Vectorización Eficiente:** La función núcleo `simular_PAS` ha sido diseñada evitando el uso de bucles `for` explícitos. Utiliza matrices multidimensionales y operaciones por ejes de NumPy (`np.random.choice`, `np.cumsum`) para generar miles de trayectorias de forma rápida y eficiente computacionalmente.
* **Flexibilidad Paramétrica:** Permite ajustar la probabilidad de éxito (p), el número de pasos (n) y el número de simulaciones independientes (reps), modelando tanto paseos simétricos como aquellos con tendencia (drift).

## Visualizaciones Incluidas

El cuaderno reproduce las siguientes situaciones teóricas:

1. **Exploración de Tendencias (Visualización 1):** Comparativa de trayectorias individuales bajo diferentes probabilidades (p=0.5, 0.6, 0.4), mostrando cómo el parámetro afecta el "drift" del paseo.
2. **Cotas Teóricas y Desigualdad de Chebyshev (Visualización 2):** Se grafican múltiples trayectorias superponiendo la **media teórica** y las **bandas de dispersión** de 1 y 2 desviaciones típicas. Esto permite verificar visualmente que la mayoría de los caminos se mantienen dentro de los límites probabilísticos esperados.
3. **Ley de los Grandes Números (Visualización 3):** Análisis de convergencia comparando la media teórica con la media empírica. Se demuestra cómo, al promediar un número creciente de trayectorias (de 5 a 1000), el resultado converge hacia la función de medias teórica.

## Tecnologías Utilizadas
* Python 3
* NumPy (Generación de matrices aleatorias y cálculo matricial)
* Matplotlib (Visualización de series temporales y áreas de confianza)
