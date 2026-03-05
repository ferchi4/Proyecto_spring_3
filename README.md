# Análisis de Preferencias Musicales: Comparación entre Springfield y Shelbyville

Este proyecto analiza el comportamiento de escucha musical de los usuarios en dos ciudades, Springfield y Shelbyville, utilizando datos reales de una plataforma de música online. El objetivo es probar si existen diferencias significativas en la actividad de escucha según el día de la semana y la ciudad.

## Objetivo
Probar la hipótesis de que la actividad de los usuarios difiere según el día de la semana y dependiendo de la ciudad de residencia.

## 🛠️ Tecnologías Utilizadas
- **Python:** Análisis de datos y manipulación con pandas.
- **Jupyter Notebook:** Entorno interactivo para el desarrollo del análisis.
- **Pandas:** Biblioteca principal para procesamiento y análisis de datos.
- **CSV Dataset:** Archivo `music_project_en.csv` con registros de reproducciones musicales.

## Pasos Clave

### 1. **Descripción de los Datos**
   - Exploración inicial del dataset con 65,079 registros y 7 columnas
   - Identificación de tipos de datos (todos object)
   - Detección de problemas: valores ausentes, duplicados y formato inconsistente

### 2. **Preprocesamiento de Datos**
   - **Estandarización de encabezados:** Conversión a minúsculas, eliminación de espacios y aplicación de snake_case
   - **Manejo de valores ausentes:** Reemplazo de valores NaN en columnas 'track', 'artist' y 'genre' con 'unknown'
   - **Eliminación de duplicados explícitos:** Remoción de 7,526 filas duplicadas
   - **Corrección de duplicados implícitos:** Unificación de variantes del género 'hiphop' ('hip', 'hop', 'hip-hop') mediante función personalizada

### 3. **Análisis de Hipótesis**
   - **Comparación general:** Cálculo de reproducciones totales por ciudad (Springfield: 42,741 | Shelbyville: 18,512)
   - **Análisis por día:** Evaluación de patrones de escucha en lunes, miércoles y viernes
   - **Función personalizada:** Creación de `number_tracks(day, city)` para filtrar y contar reproducciones por criterios específicos

### 4. **Resultados por Ciudad y Día**

| Ciudad      | Lunes   | Miércoles | Viernes |
|-------------|---------|-----------|---------|
| Springfield | 15,740  | 11,056    | 15,945  |
| Shelbyville | 5,614   | 7,003     | 5,895   |

## Conclusiones

El análisis confirma que:

- **La actividad de escucha musical varía significativamente** entre Springfield y Shelbyville
- **Springfield muestra mayor actividad** en todos los días analizados, especialmente los lunes y viernes
- **Shelbyville presenta un pico de actividad** los miércoles, a diferencia de Springfield
- **La hipótesis inicial es ACEPTADA:** existen diferencias estadísticamente relevantes en los hábitos de escucha entre ambas ciudades según el día de la semana

## Aplicaciones de Negocio

Estos hallazgos permiten:
- Personalizar recomendaciones musicales según la ciudad y el día
- Optimizar estrategias de marketing y promociones en momentos de mayor actividad
- Planificar lanzamientos de contenido en días de mayor engagement por ciudad

## Cómo Ejecutar
Clona este repositorio:
(https://github.com/ferchi4/Proyecto_spring_3)
