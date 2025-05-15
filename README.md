# Café Productivo: Análisis del Comportamiento de Clientes en un Espacio de Trabajo y Estudio

## Objetivo General:

Analizar el comportamiento de los clientes en una cafetería enfocada en estudio y trabajo para optimizar decisiones
relacionadas con el menú horarios, disposición del espacio y promociones.

## Preguntas guía del análisis
1. ¿En qué horarios hay mayor afluencia de personas trabajando o estudiando?
2. ¿Qué productos se consumen más durante sesiones de estudio/trabajo?
3. ¿Cuál es el tiempo promedio de estancia de los distintos tipos de clientes?
4. ¿Las ventas cambian si hay eventos como lluvias, exámenes universitarios, etc.?
5. ¿Qué diferencias hay entre clientes individuales y grupos (reuniones)?
6. ¿Hay correlación entre consumo de cafeína y duración de la visita?
7. ¿Cuáles son los días más rentables y por qué?

## Análisis sugeridos:
1. Análisis exploratorio (EDA):
   - Distribución de visitas por hora y día.
   - Duración de visitas por hora y tipo de cliente.
   - Productos más vendidos por franja horaria.
   - Correlación entre tipo de consumo (café, té, postres) y duración.
2. Segmentación de clientes:
    - K-Means clustering por hábitos de consumo + duración.
    - Agrupar perfiles: "trabajador remoto", "estudiante intenso", "reunión rápida", etc.
3. Predicción y Modelos (Opcional):
    - Modelo de predicción de ventas por hora usando regresión (factores: clima, día, eventos).
    - Clasificación de clientes en tipos a partir de su consumo y duración.
4. Visualizaciones interactivas:
    - Heatmaps de afluencias por hora/día.
    - Gráfico de embudo de consumo típico según propósito.
    - Series temporales de ingresos y afluencia.

## Ideas adicionales para enriquecer:
- Crear una tabla de recomendaciones para rediseñar el menú según las horas más ocupadas.
- Estimar ingresos perdidos por baja rotación de mesas.
- Evaluar si los enchufes/zonas silenciosas influyen en el tiempo de estancia.
- Analizar cómo afecta el cambio de música o iluminación (si se registra).