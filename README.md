# Algoritmos Genéticos en Aprendizaje de Máquina

Este repositorio presenta la aplicación de algoritmos genéticos (AG) en tres problemas fundamentales del aprendizaje de máquina:

* Selección de características (Feature Selection)
* Optimización de hiperparámetros (Hyperparameter Optimization)
* Neuroevolución (Neuroevolution)

El objetivo es demostrar cómo un mismo enfoque evolutivo puede utilizarse para optimizar distintos componentes de un modelo.

## Descripción general

Los algoritmos genéticos son técnicas de optimización inspiradas en la evolución natural. Funcionan a partir de una población de soluciones (cromosomas), que evolucionan mediante selección, cruzamiento y mutación.

En este proyecto, se aplican estos operadores para resolver tres problemas diferentes en Machine Learning.

## Metodología

En los tres casos se sigue el mismo ciclo:

1. Representación del cromosoma
2. Inicialización de la población
3. Evaluación mediante función de aptitud (fitness)
4. Selección de individuos
5. Cruzamiento
6. Mutación
7. Terminación (número de generaciones)

La diferencia entre los problemas radica en qué representa el cromosoma.

## Feature Selection

Se busca encontrar el mejor subconjunto de características que maximiza el rendimiento del modelo.

* Representación: vector binario
* Ejemplo: [1,0,1,1]
* Interpretación: usar o no cada característica

Resultado: se identificaron combinaciones de variables que mantienen alta precisión reduciendo la dimensionalidad.

## Hyperparameter Optimization

Se optimizan los hiperparámetros de un modelo de clasificación.

* Representación: valores numéricos
* Ejemplo: [94, 4]
* Parámetros: número de árboles, profundidad

Resultado: se encontraron múltiples configuraciones con alto rendimiento.

## Neuroevolution

Se entrena una red neuronal simple utilizando algoritmos genéticos.

* Representación: pesos y bias
* Ejemplo: [w1, w2, b]
* No se usa backpropagation

Resultado: se alcanzó una precisión del 100% en el problema AND.

## Resultados

| Problema          | Mejor solución    | Accuracy |
| ----------------- | ----------------- | -------- |
| Feature Selection | [0,0,1,1]         | 0.95     |
| Hyperparameter    | [94,4]            | 1.00     |
| Neuroevolution    | Pesos optimizados | 1.00     |

## Ejecutar en Google Colab

Los notebooks pueden ejecutarse directamente en Google Colab.

## Conclusión

Los algoritmos genéticos demostraron ser una herramienta versátil para seleccionar características, ajustar hiperparámetros y entrenar redes neuronales utilizando un mismo enfoque evolutivo.
