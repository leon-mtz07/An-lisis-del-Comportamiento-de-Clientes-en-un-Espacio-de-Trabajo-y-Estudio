# Café Productivo: Análisis del Comportamiento de Clientes en un Espacio de Trabajo y Estudio

## Objetivo General:

Analizar el comportamiento de los clientes en una cafetería enfocada en estudio y trabajo para optimizar desiciones
relacionadas con el menú horarios, disposición del espacio y promociones.

### Tecnologías usadas en el análisis:

- Python 3.12
- Pandas
- Datetime
- Seaborn
- Sklearn
- KMeans

## Preguntas guía del análisis

1. ¿En qué horarios hay mayor afluencia de personas trabajando o estudiando?
2. ¿Qué productos se consumen más durante sesiones de estudio/trabajo?
3. ¿Cuál es el tiempo promedio de estancia de los distintos tipos de clientes?
4. ¿Las ventas cambian si hay eventos como lluvias, exámenes universitarios, etc.?
5. ¿Qué diferencias hay entre clientes individuales y grupos (reuniones)?
6. ¿Hay correlación entre consumo de cafeína y duración de la visita?
7. ¿Cuáles son los días más rentables y por qué?

## Análisis

### 1. ¿En qué horarios hay mayor afluencia de personas trabajando o estudiando?
En el análisis se vio que hay mayor cantidad de gente que viene a nuestro café de manera individual que de manera
grupal o en pareja. Esto debido a que por ejemplo en un solo día en total dentro de una hora, el conjunto de personal
que viene de manera grupal y en pareja sumados no alcanza a las personas que viene de manera individual, por lo que
de antemano ya sabemos quien es nuestro público objetivo, los que vienen de manera individual.

A continuación se presentan los horarios de ocupación a partir de su tipo de visita y su propósito:

- Tipo de visita en 'grupo' y con un propósito de 'trabajar':

<div style="text-align: center;">
<img src="img/grupo_trabajo.png" alt="horarios de ocupación de gente en grupo y propósito de trabajar">
</div>
 
-  Tipo de visita en 'grupo' y con un propósito de 'estudiar':

<div style="text-align: center;">
<img src="img/grupo_estudiar.png" alt="horarios de ocupación de gente en grupo y propósito de estudiar">
</div>

- Tipo de visita en 'grupo' en general:

<div style="text-align: center;">
<img src="img/grupo.png" alt="horario de ocupación por grupo">
</div>

- Tipo de visita en 'pareja' y con propósito de 'trabajar':

<div style="text-align: center">
<img src="img/pareja_trabajo.png" alt="horario de ocupacion de pareja y trabajando">
</div>

- Tipo de visita en 'pareja' y con propósito de 'estudiar':

<div style="text-align: center">
<img src="img/pareja_estudiar.png" alt="horario de ocupación">
</div>

- Tipo de visita en 'pareja':

<div style="text-align: center">
<img src="img/pareja.png" alt="">
</div>

- Tipo de visita 'individual' y con propósito de 'trabajar':

<div style="text-align: center">
<img src="img/individual_trabajo.png" alt="">
</div>

- Tipo de visita 'individual' y con propósito de 'estudiar':

<div style="text-align: center">
<img src="img/individual_estudiar.png" alt="">
</div>

- Visita con un propósito de 'estudiar':

<div style="text-align: center">
<img src="img/estudiar.png" alt="">
</div>

- Visita con un propósito de 'trabajar':

<div style="text-align: center">
<img src="img/trabajar.png" alt="">
</div>

De manera general podemos ver a simple vista que uno de los días más ocupados es el martes, y que conforme se va
viendo las imágenes, se va viendo que se van ocupando poco a poco, por lo que podemos análizar que los grupos no nos
frecuentan tanto, luego le sigue las parejas, y en seguida los individuales, por lo que aquí se vuelve a apreciar
que nuestro público objetivo son las personas que vienen de manera individual, y que a su vez, las personas vienen
más a estudiar que ha trabajar

### 2. ¿Qué productos se consumen más durante sesiones de estudio/trabajo?

En los dos análisis se ve que no tienen mucha diferencia, pero si le prestamos más atención se podrán sacar varias
conclusiones de esas tablas:

- Productos que más se consumen cuando la gente va a estudiar:

| Producto       | Precio | Cantidad | %_cantidad | %_ingresos |
|----------------|--------|----------|------------|------------|
| Ensalada       | 5.0    | 233      | 11.61      | 17.00      |
| Sándwich       | 4.5    | 206      | 10.26      | 13.53      |
| Smoothie       | 4.0    | 216      | 10.76      | 12.61      |
| Tarta de queso | 3.5    | 232      | 11.56      | 11.85      |
| Café con leche | 3.0    | 267      | 13.30      | 11.69      |
| Capuchino      | 3.2    | 225      | 11.21      | 10.51      |
| Té verde       | 2.8    | 196      | 9.77       | 8.01       |
| Café americano | 2.5    | 215      | 10.71      | 7.84       |
| Croissant      | 2.2    | 217      | 10.81      | 6.97       |

- Productos que más se consumen cuando la gente va a trabajar:

| Producto       | Precio | Cantidad | %_cantidad | %_ingresos |
|----------------|--------|----------|------------|------------|
| Ensalada       | 5.0    | 239      | 10.64      | 15.71      |
| Sándwich       | 4.5    | 236      | 10.50      | 13.96      |
| Smoothie       | 4.0    | 240      | 10.68      | 12.62      |
| Tarta de queso | 3.5    | 254      | 11.30      | 11.69      |
| Café con leche | 3.0    | 269      | 11.97      | 10.61      |
| Capuchino      | 3.2    | 240      | 10.68      | 10.10      |
| Té verde       | 2.8    | 272      | 12.11      | 10.01      |
| Café americano | 2.5    | 239      | 10.64      | 7.85       |
| Croissant      | 2.2    | 258      | 11.48      | 7.46       |