# Media-Prompt-Assistant
  
  'Media Prompt Assistant' es un proyecto de desarrollo de chatbots especializados en generar prompts avanzados para los modelos Suno AI y Adobe Firefly Image 4. Los mismos funcionan a partir de una API Key de Gemini proporcionada por el usuario para comunicarse con el modelo. 
  El objetivo de los mismos consiste en arrojar prompts avanzados a partir de prompts sencillos tomando como referencia la base de datos (dataset) cargada previamente. Existen 2 versiones: una para utilizar la API Key free de Gemini, y otra optimizada en tokens (versión 'TKO') para utilizar la API Key de pago. Ambas versiones están disponibles tanto para el chatbot de Suno AI como el de Adobe Firefly Image 4.


# Introducción

* Nombre del proyecto: Media Prompt Assistant

* Problema a abordar: Un cliente quiere lanzar un canal de YouTube con contenido musical en formato “radio en vivo”. Para esto necesita música original y una imagen de portada, que también servirá como primer frame de un video generado con IA. El género elegido para uno de los videos es Synthwave, con influencias de subgéneros como Darkwave y Chillwave, entre otros. Todas las canciones deben ser instrumentales, ya que la finalidad es acompañar momentos de concentración, estudio o trabajo.

* Propuesta de solución: Se utilizarán los chatbots para generar los prompts avanzados de los modelos. Esto permite agilizar los procesos de producción y abaratar los costos de la misma ya que podemos ingresar prompts sencillos que luego serán analizados y mejorados por el modelo. 
  

* Viabilidad del proyecto: El proyecto es posible de realizar ya que al contar con el acceso a los modelos, es posible testear y optimizar a los mismos para que respondan la manera más eficiente. Dichos modelos ya eran utilizados previamente para trabajar, por lo que esta herramienta busca optimizar los tiempos y mejorar los resultados.


# Objetivo

  El proyecto tiene como finalidad optimizar los tiempos en el desarrollo de prompts avanzados para los modelos utilizados. Esto significa que a partir de un prompt sencillo el modelo nos arroja un prompt avanzado de acuerdo a las indicaciones que se les han otorgado en los distintos datasets. Esto permite reducir los tiempos de producción significativamente y obtener mejores resultados.


# Metodología

  A partir del conocimiento del proyecto con el cual debemos trabajar, se utilizarán los prompts adecuados para generar los prompts avanzados de cada modelo. De esta manera podremos generar la música necesaria a partir de la utilización de los prompts arrojados en el chatbot utilizando el modelo Suno AI y de la misma manera podemos generar la imágen correspondiente ingresando el prompt que nos arroja el modelo en Adobe Firefly Image 4.

  
# Técnicas de Fast Prompting

  La técnica aplicada para el uso de los chatbots será 'Zero Prompt Shooting', la cual es posible gracias al dataset cargado previamente, sin necesidad de explicarle al modelo cómo debe responder. Para lograr esto, se utilizó la técnica de 'Few Prompt Shooting' dentro del conjunto de datasets para ajustar el comportamiento del modelo, brindandole ejemplos de cómo el modelo interpreta los prompts y qué particularidades tiene cada uno al momento de utiizar cada modelo.


# Implementación

  En el repositorio se encuentran disponibles para descargar los chatbots dentro de los archivos .zip. Los mismos deben correrse con el software 'Jupyter Notebook' ya que el código fue adaptado para funcionar allí.


  
