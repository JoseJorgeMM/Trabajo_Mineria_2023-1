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

1. Bronce: Contiene un dataframe 'raw_data' con 3 columnas. Nos interesa la columna 'contenido', la cual contiene los cuerpos de los correos sin procesar.

2. Plata: Contiene 2 dataframes: 'datos_preprocesados' que contiene la informacion de 'raw_data' y adicional una lista de tokens y descripción de estos tokens. El dataframe 'list_tokens' contiene solamente la lista de tokens de cada texto.

3. Oro: Contiene 2 dataframes: 'df_etiquetado' que contiene el corpus y el topico principal de cada texto y 'topicos' que contiene la información de 'datos_preprocesados' adicional columnas del tópico principal y su respectivo peso
