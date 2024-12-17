# diabetes_ML

La finalidad de la creaciòn de este repositorio es poder analizar una data de un nùmero random de pacientes que puedan tener riesgo de padecer diabetes.

El conjunto de datos incluye varias características esenciales para predecir el riesgo de diabetes, centrándose en una combinación de métricas demográficas, de estilo de vida y de salud. El modelo XGBoost utiliza estas características para predecir los niveles de riesgo, lo que permite intervenciones de atención médica personalizadas. Características como la edad, el peso, la glucosa en sangre y la actividad física son variables numéricas que contribuyen directamente al cálculo del riesgo de diabetes, mientras que las variables categóricas como la calidad de la dieta y la adherencia a la medicación proporcionan un contexto importante sobre el estilo de vida y los hábitos del usuario. En conjunto, estas características ayudan a crear un perfil integral de cada usuario, lo que permite realizar predicciones precisas y recomendaciones de salud personalizadas.

Diccionario de datos

A continuación se muestran las columnas incluidas en el conjunto de datos, junto con descripciones de cada una:

ID de usuario: Identificador único asignado a cada usuario para garantizar la privacidad y el seguimiento de los datos.

Datos: Representa la fecha específica de cada registro, indicando la naturaleza de serie temporal del conjunto de datos.

Peso (kg): peso corporal del usuario en kilogramos. El peso es un factor importante para determinar los riesgos relacionados con la obesidad.

Altura (cm): altura del usuario, medida en centímetros. Esto, combinado con el peso, ayuda a calcular el IMC, un predictor clave del riesgo de diabetes.

Glucemia (mg/dl): nivel de glucosa en sangre del usuario en miligramos por decilitro. Este es uno de los indicadores más importantes para diagnosticar la diabetes, con valores que suelen oscilar entre 70 y 300 mg/dl.

Actividad física (minutos/día): duración diaria de la actividad física, medida en minutos. La actividad física desempeña un papel fundamental en el control de los niveles de glucosa en sangre y la reducción del riesgo de diabetes.

Calidad de la dieta: variable categórica que describe la calidad de la dieta del usuario, clasificada como "saludable" o "insalubre". La dieta desempeña un papel importante en la prevención y el control de la diabetes.

Adherencia a la medicación: indica el grado de adherencia del usuario a la medicación prescrita, categorizada como "buena" o "mala". Una adherencia adecuada es crucial para controlar eficazmente los niveles de glucosa en sangre.

Nivel de estrés: el nivel de estrés informado por el usuario, categorizado como "bajo", "medio" o "alto". El estrés crónico puede afectar significativamente los niveles de glucosa en sangre y contribuir al riesgo de diabetes.

Duración del sueño (horas): la cantidad de horas que el usuario duerme cada día. Dormir lo suficiente es fundamental para mantener la salud general y estabilizar los niveles de azúcar en sangre.

Estado de hidratación: indica si el usuario está adecuadamente hidratado, con valores de "sí" o "no". Una hidratación adecuada favorece el funcionamiento óptimo del organismo, lo que incluye el mantenimiento del equilibrio de la glucosa en sangre.

IMC: Índice de masa corporal, calculado a partir del peso y la altura del usuario. El IMC es un indicador importante de si una persona tiene bajo peso, peso normal, sobrepeso u obesidad, lo que está directamente relacionado con el riesgo de diabetes.

Puntuación de riesgo: la puntuación de riesgo calculada para cada usuario, generada en función de varias métricas de salud. Esta puntuación ayuda a clasificar a los usuarios en diferentes niveles de riesgo:

-Riesgo bajo (< 30): Se considera que los usuarios tienen una baja probabilidad de desarrollar diabetes.

-Riesgo moderado (30-60): A los usuarios se les brindan consejos preventivos para reducir su riesgo.

-Riesgo alto (>60): Los usuarios corren un alto riesgo y reciben recomendaciones urgentes para controlar su condición.
