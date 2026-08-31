# ProyectoFinal_Rendimiento_Escolar
Aplicación que analiza la relación entre horas de estudio y calificación final en estudiantes. Carga datos desde Google Sheets, permite limpiar anomalías, genera un modelo de regresión lineal y predice calificaciones según el tiempo de estudio. Incluye navegación entre 4 etapas: Ver Datos, Limpiar, Modelar y Predice.

Rendimiento Estudiantil: Predictor de Calificaciones
Es una aplicación de ciencia de datos desarrollada en MIT App Inventor que permite analizar la relación entre los hábitos de estudio y el rendimiento académico de los estudiantes, específicamente su calificación en el examen final. La aplicación sigue un flujo de trabajo de cuatro etapas y está diseñada para ser utilizada por docentes, investigadores o estudiantes interesados en comprender cómo factores como las horas de estudio influyen en el desempeño académico.

- Funcionalidades Principales:
+
           Ver Datos (View Data)
  
* Carga de forma automática un conjunto de datos desde Google Sheets con información de estudiantes.
* Visualización gráfica en un gráfico de dispersión que muestra la relación entre:

      Eje X: Horas de estudio por semana (study_time_hours)

      Eje Y: Calificación del examen final (final_exam_score)

* Resumen estadístico con el número total de registros cargados.
+
           Limpieza de Datos (Data Cleaning)

* Detección de anomalías mediante un algoritmo que identifica valores atípicos en los datos.
* Resaltado visual de los puntos anómalos en el gráfico para su identificación rápida.
* Eliminación interactiva de registros problemáticos haciendo clic directamente sobre ellos.
* Preparación de un conjunto de datos "limpio" para el modelado.
+
          Modelo Matemático (Math Model)

* Cálculo de regresión lineal entre las horas de estudio (variable independiente X) y la calificación final (variable dependiente Y).
* Visualización de la línea de mejor ajuste (trendline) superpuesta al gráfico de datos.
* Presentación de resultados clave:

      Pendiente (m): Indica cuánto aumenta la calificación por cada hora adicional de estudio.

      Intersección (b): Calificación estimada cuando las horas de estudio son cero.

      Coeficiente de correlación (R): Mide la fuerza de la relación entre las variables.
+
          Predicciones (Predictions)
          
* Interfaz simple donde el usuario puede observar el cálculo automático de la calificación estimada utilizando la ecuación del modelo:

      calificación_estimada = (m × horas_estudio) + b

* Resultado instantáneo que muestra la predicción en pantalla. Ademas de utilzar una herramienta de inteligencia artificial.

- Navegación
+
Menú funcional que permite al usuario moverse fácilmente entre las cuatro pantallas de la aplicación. Diseño intuitivo con botones de navegación en cada pantalla.

- Conjunto de Datos Utilizado
+
La aplicación utiliza un conjunto de datos de rendimiento estudiantil que incluye las siguientes variables:
  Columna	Descripción:
       
        Tiempo de estudio
        Horas de sueño por noche
        Ultima calificacion del examen final (variable objetivo)

Fuente de datos: Google Sheets (enlace público disponible en la documentación del proyecto).

Tecnologías Utilizadas
- MIT App Inventor (Entorno de desarrollo visual)
- Google Sheets API (Almacenamiento y lectura de datos)
- Componentes de ciencia de datos de App Inventor:
- Spreadsheet (Conexión con Google Sheets)
- Chart2D (Gráficos de dispersión)
- Trendline (Regresión lineal)
- AnomalyDetection (Limpieza de datos).
