<div align="center">
<img src="https://www.cuc.edu.co/wp-content/uploads/2024/03/logo_cuc.png" alt="Logo CUC" width="300"/>
</div>

# CUC - UNIVERSIDAD DE LA COSTA
## Departamento de Ciencias de la Computación y Electrónica
## Materia: Data Mining

## *Unidad 2:*
###             ACTIVIDAD I: APRENDIZAJE SUPERVISADO vs. NO SUPERVISADO


### Presentado por:

- *Jesus Gabriel Gudiño Lara*

- *Ana Rosa Ramirez Lopez*

---
# Dataset Sintético de Deserción Estudiantil

Este repositorio contiene un conjunto de datos sintético generado para la Actividad I de la asignatura de Minería de Datos de la Universidad de la Costa. El objetivo es simular un escenario real para predecir la deserción estudiantil en programas de pregrado.

## Descripción del Dataset

El conjunto de datos (dataset_desercion_estudiantil.csv) contiene *500 registros* y las siguientes 10 columnas:

### Variables

| Nombre de la Variable            | Tipo de Dato  | Rango/Valores Posibles                       | Descripción                                        |
| -------------------------------- | ------------- | -------------------------------------------- | -------------------------------------------------- |
| edad                           | Numérico (int)  | 17 - 24                                      | Edad del estudiante en años.                       |
| genero                         | Categórico    | 'Masculino', 'Femenino'                      | Género del estudiante.                             |
| lugar_origen                   | Categórico    | 'Urbano', 'Rural'                            | Zona de procedencia del estudiante.                |
| promedio_bachillerato          | Numérico (float)| 7.0 - 10.0                                   | Calificación promedio obtenida en la secundaria.   |
| puntaje_admision               | Numérico (int)  | 800 - 1300                                   | Puntaje obtenido en el examen de ingreso.          |
| calificaciones_primer_semestre | Numérico (float)| 5.0 - 10.0                                   | Promedio de calificaciones en su primer semestre.  |
| nivel_socioeconomico           | Categórico    | 'Bajo', 'Medio', 'Alto'                      | Nivel socioeconómico de la familia del estudiante. |
| tiene_beca                     | Categórico    | 'Sí', 'No'                                   | Indica si el estudiante cuenta con alguna beca.    |
| tiene_credito                  | Categórico    | 'Sí', 'No'                                   | Indica si el estudiante usa algún crédito educativo.|
| desercion                      | Categórico    | 'Sí', 'No'                                   | *Variable objetivo:* Indica si el estudiante desertó. |

---

### Introducción de Nulos y Atípicos

Para simular un conjunto de datos más realista, se introdujeron imperfecciones de forma controlada:

1.  *Valores Nulos:*
    * Se introdujo un *5%* de valores nulos (NaN) en la columna promedio_bachillerato para simular expedientes incompletos.
    * Se introdujo un *8%* de valores nulos en nivel_socioeconomico para simular encuestas no respondidas.

2.  *Valores Atípicos (Outliers):*
    * Se insertaron *3 registros* con valores extremadamente bajos (entre 0.0 y 2.5) en calificaciones_primer_semestre para representar casos de muy bajo rendimiento.
    * Se insertaron *2 registros* con valores anormalmente altos (superiores a 1500) en puntaje_admision para simular posibles errores de captura de datos.