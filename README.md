# DL-QPI

Título del proyecto: Traducción de campo brillante a fase plausible en eritrocitos con CycleGAN: evaluación de viabilidad en el dataset P. vivax

## Objetivo general
Evaluar la viabilidad de generar representaciones de fase plausibles de eritrocitos a partir de imágenes de campo brillante mediante un modelo CycleGAN no pareado, determinando su capacidad para conservar las características morfológicas de las células de entrada y reproducir las propiedades estadísticas y los perfiles de fase observados en imágenes reales obtenidas mediante microscopía holográfica digital (DHM).

## Objetivos específicos
Construir un conjunto de datos armonizado de imágenes de eritrocitos en los dominios de campo brillante y fase DHM, mediante el ajuste de escala espacial, la conversión de las imágenes de fase a una representación numérica normalizada, la reducción de artefactos y la extracción de parches, estableciendo un pipeline reproducible para el entrenamiento y la evaluación del modelo.
Implementar y comparar un modelo CycleGAN convencional y una variante que incorpore una función de pérdida orientada a preservar las características morfológicas y los perfiles de fase de los eritrocitos, utilizando una línea base sin aprendizaje y un procedimiento de segmentación para extraer los perfiles celulares y calcular el delta de fase máximo-mínimo.
Evaluar la calidad y plausibilidad de las imágenes de fase generadas mediante métricas de similitud entre distribuciones, conservación morfológica y comparación de los perfiles y deltas de fase promedio frente a las imágenes DHM reales, estableciendo criterios de evaluación y documentando las limitaciones del enfoque.

## Equipo y roles

Acordado en la reunión del 2026-10-28.

| Integrante | GitHub | Rol |
|---|---|---|
| Jacobo Giraldo | [@Jacogz](https://github.com/Jacogz) | Arquitectura de la solución |
| Juan Lotero | [@juanlotero2552](https://github.com/juanlotero2552) | Procesamiento y preparación de datos |
| Sahian Salome | [@sahiansalome14](https://github.com/sahiansalome14) | Diseño de la heurística e implementación del modelo |
