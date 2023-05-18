# Flujo de trabajo basado en NLP para la extracción de tópicos y clasificación de correos electrónicos generados por usuarios. Caso de estudio aplicado a una fintech
## Descripción
El propósito de este proyecto es explorar técnicas de NLP para procesar y analizar el contenido de correos electronicos. Las funcionalidades principales del proyecto incluyen:

Limpieza

Normalización

Reducción de vocabulario

Tokenización

Lematización

Analizis de frecuencias

Modelado de tópicos

Modelado de clasificación

La carpeta Data contiene 3 subcarpetas: 1. Bronce, 2. Plata, 3. Oro:

  1. Bronce: Contiene un dataframe 'raw_data' con 3 columnas. Nos interesa la columna 'contenido', la cual contiene los cuerpos de los        correos sin procesar.

  2. Plata: Contiene 2 dataframes: 'datos_preprocesados' que contiene la informacion de 'raw_data' y adicional una lista de tokens y          descripción de estos tokens. El dataframe 'list_tokens' contiene solamente la lista de tokens de cada texto.

  3. Oro: Contiene 2 dataframes: 'df_etiquetado' que contiene el corpus y el topico principal de cada texto y 'topicos' que contiene la        información de 'datos_preprocesados' adicional columnas del tópico principal y su respectivo peso

La carpeta Jobs contiene 4 notebooks enumerados del 1 hasta el 4. A continuación se detalla el uso de cada uno:

  Notebook 1. Se carga el df 'raw_data' de Bronce. Se realiza Limpieza, Normalización, Reducción de vocabulario, Tokenización,                         Lematización, y Analizis de frecuencias. Se exportan los df contenidos en la subcarpeta Plata de Data.
  
  Notebook 2. Se carga el df 'list_tokens' de Plata. Se realiza el modelo de detección de tópicos con LDA y NMF y se exportan los df                   pertenecientes a la subcarpeta Oro de Data.
  
  Notebook 3. Se carga el df 'df_etiquetado' de Oro. Se entrenan los modelos de clasificación supervisados y se escoge el mejor modelo.
  
  Notebook 4. Se carga el df 'df_etiquetado' de Oro como dataframe PySpark y se entrena el modelo ganador del notebook anterior en la                   libreria Mlib de PySpark.
