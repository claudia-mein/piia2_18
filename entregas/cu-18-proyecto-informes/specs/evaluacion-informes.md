# Evaluación de informes clínicos sintéticos

## Qué construir

Queremos desarrollar un procedimiento de evaluación que nos permita analizar la calidad de los informes clínicos sintéticos generados por los distintos modelos de lenguaje.

Para ello, definiremos unos criterios comunes con los que revisar aspectos como la estructura y el formato del informe, la coherencia entre los síntomas, las pruebas diagnósticas, el diagnóstico y el tratamiento, la consistencia de las fechas y las dosis, y la variedad de los casos generados.

La evaluación incluirá la identificación y clasificación de errores concretos, como contradicciones clínicas, incoherencias temporales, información inventada o tratamientos que no se corresponden con el diagnóstico. También estudiaremos el uso de métricas automáticas, como BLEU, ROUGE y BERTScore, para analizar la similitud textual y semántica con los informes de referencia, sin considerar estas métricas como una medida directa de corrección médica.

Además, contaremos con la valoración de un profesional sanitario, que revisará una selección de informes para identificar posibles errores clínicos y valorar su coherencia médica.

Los resultados de las evaluaciones se registrarán de forma organizada, asociando cada valoración al informe, modelo y estrategia de generación correspondientes. Esto nos permitirá analizar los errores más frecuentes y utilizar la información obtenida para comparar y mejorar las estrategias de generación.
