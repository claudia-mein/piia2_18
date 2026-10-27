# Comparación de modelos y estrategias de generación

## Qué construir

Queremos desarrollar un procedimiento que nos permita comparar los resultados obtenidos con los diferentes modelos de lenguaje y estrategias de generación utilizados en el proyecto.

Para ello, reuniremos los resultados de las evaluaciones de los informes generados con Llama, Qwen, GPT y Mistral, teniendo en cuenta aspectos como la estructura de los documentos, la coherencia clínica, la consistencia de la información, los errores detectados y las métricas automáticas utilizadas.

La comparación se realizará tanto entre diferentes modelos como entre las distintas estrategias de generación de un mismo modelo, incluyendo prompting, few-shot prompting y generación en dos fases.

Organizaremos los resultados mediante tablas y resúmenes que permitan identificar las diferencias entre los experimentos, los tipos de errores más frecuentes y las mejoras o empeoramientos observados al modificar los prompts o las estrategias de generación.

Esta funcionalidad utilizará los resultados obtenidos mediante el procedimiento de evaluación definido anteriormente, con el objetivo de extraer conclusiones sobre las capacidades y limitaciones de los modelos estudiados.

## Por qué

Los diferentes modelos de lenguaje pueden generar informes clínicos con características y errores distintos, incluso cuando reciben instrucciones similares. Además, los cambios en los prompts o el uso de ejemplos pueden mejorar determinados aspectos de los informes, pero también provocar nuevos errores o empeorar otros.

Por este motivo, no es suficiente evaluar los informes de forma individual. Necesitamos comparar los resultados de los distintos experimentos para comprobar qué modelos y estrategias ofrecen mejores resultados y en qué aspectos presentan mayores dificultades.

Con esta funcionalidad buscamos identificar las diferencias entre los modelos estudiados, analizar cómo influyen las estrategias de generación y determinar qué combinaciones ofrecen un mejor equilibrio entre realismo, estructura y coherencia clínica.

También queremos que las conclusiones se basen en los resultados de las evaluaciones y no únicamente en impresiones subjetivas, de manera que podamos justificar las decisiones tomadas durante el proyecto y orientar futuras mejoras.

## Restricciones y supuestos

- **Modelos comparados:** se estudiarán los modelos de lenguaje seleccionados para el proyecto, como Llama, Qwen, GPT y Mistral. Solo se incluirán en las comparaciones los modelos con experimentos realizados y resultados disponibles.

- **Criterios de evaluación comunes:** todos los modelos y estrategias se compararán utilizando los mismos criterios de evaluación, definidos en la spec `evaluacion-informes.md`.

- **Condiciones experimentales:** para que las comparaciones sean lo más justas posible, se utilizarán instrucciones equivalentes y un número similar de informes por experimento. Se documentarán las diferencias en los parámetros de generación, los ejemplos utilizados y las condiciones de ejecución.

- **Comparación de estrategias:** cuando se compare el efecto de diferentes estrategias en un mismo modelo, se intentarán mantener constantes los demás parámetros para poder identificar qué cambios se deben a la estrategia utilizada.

- **Resultados de evaluación:** las comparaciones se basarán en los informes y las evaluaciones disponibles. No se asignarán puntuaciones a modelos o estrategias que todavía no hayan sido evaluados.

- **Métricas automáticas:** los resultados de BLEU, ROUGE y BERTScore se interpretarán como medidas de similitud textual y semántica, no como indicadores directos de corrección clínica.

- **Evaluación profesional:** las valoraciones del profesional sanitario se tendrán en cuenta cuando estén disponibles y se presentarán diferenciadas de las evaluaciones realizadas por el equipo.

- **Interpretación de resultados:** las conclusiones se limitarán a los experimentos realizados y al número de informes analizados. No se asumirá que un modelo es superior en todos los casos por obtener mejores resultados en una muestra pequeña.

- **Registro de comparaciones:** cada comparación deberá permitir identificar los modelos, las estrategias, las versiones de los prompts, el número de informes y los criterios de evaluación utilizados.

- 
