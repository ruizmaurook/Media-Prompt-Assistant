# Media Prompt Assistant
  
  'Media Prompt Assistant' es un proyecto de desarrollo de chatbots especializados en generar prompts avanzados para los modelos Suno AI y Adobe Firefly Image 4. Los mismos funcionan a partir de una API Key de Gemini proporcionada por el usuario en un archivo .env para comunicarse con el modelo.
  El objetivo de los mismos consiste en arrojar prompts avanzados a partir de prompts sencillos tomando como referencia la base de datos (dataset) cargada previamente. Existen 2 versiones: una para utilizar la API Key free de Gemini, y otra optimizada en tokens (versión 'TKO') para utilizar la API Key de pago. Ambas versiones están disponibles tanto para el chatbot de Suno AI como el de Adobe Firefly Image 4.

# Introducción

* **Nombre del proyecto:** Media Prompt Assistant

* **Problema a abordar:** Un cliente quiere lanzar un canal de YouTube con contenido musical en formato “radio en vivo”. Para esto necesita música original y una imagen de portada, que también servirá como primer frame de un video generado con IA. El género elegido para uno de los videos es Synthwave, con influencias de subgéneros como Darkwave y Chillwave, entre otros. Todas las canciones deben ser instrumentales, ya que la finalidad es acompañar momentos de concentración, estudio o trabajo.

**Propuesta de solución** 

Se utilizarán los chatbots para generar los prompts avanzados de los modelos. Esto permite agilizar los procesos de producción y abaratar los costos de la misma ya que podemos ingresar prompts sencillos que luego serán analizados y mejorados por el modelo. Cada prompt se escribirá primero en español y luego se traducirá al inglés, de manera que el modelo interprete mejor las instrucciones. Para este proceso podemos usar un modelo vía web en lugar de API, ya que lo que necesitamos ingresar en el chatbot puede resolverse directamente gracias a su entrenamiento previo.


**Prompt para utilizar el chatbot destinado a Suno AI**

* Prompt original en español (hecho por usuario):

*“Desarrolla una canción instrumental de género Synthwave. Puedes mezclar con subgéneros como el Darkwave o Chillwave. Describe la instrumentación propia del género la cual le da la estética sonora. Utiliza el campo ‘Lyrics’ para la estructura de la canción y luego continúa con la descripción correspondiente para para los campos ‘Style’, ‘Exclude Style’, ‘Weirdness’ y ‘Style Influence’.” (99 tokens).*

  Aclaración: Cabe destacar que para redactar prompts con más detalles y descripciones, es necesario contar con saberes previos de producción musical y entender cómo interpreta Suno las instrucciones ya que el modelo se encuentra en constante actualización. Para fines prácticos del trabajo, se utilizarón prompts sencillos para mejor entendimiento de la funcionalidad de los chatbots.

* Prompt traducido al inglés (respuesta de la IA):

  *“Develop an instrumental song in the Synthwave genre. You can mix in subgenres such as Darkwave or Chillwave. Describe the instrumentation typical of the genre that gives it its sonic aesthetic. Use the field ‘Lyrics’ for the structure of the song and then continue with the corresponding description for the fields ‘Style’, ‘Exclude Style’, ‘Weirdness’, and ‘Style Influence’.” (79 tokens).*

* Prompt optimizado en cantidad de tokens (para los chatbots TKO) en inglés:

  *“Create an instrumental Synthwave track, mixing Darkwave or Chillwave elements. Describe the genre’s key instruments that shape its sound. Use the ‘Lyrics’ field for song structure, then add descriptions for ‘Style’, ‘Exclude Style’, ‘Weirdness’, and ‘Style Influence’.” (59 tokens).*

  
**Prompt para chatbot de Adobe Firefly Image 4**

* Prompt en español (hecho por usuario):

*“Desarrolla un prompt para generar una imágen estilo Synthwave, utilizando la paleta de colores más usual (magenta, cian, violeta, azul y rojo). La imágen debe ser una ciudad futurista adaptada al estilo mencionado. Describe las características técnicas necesarias para respetar la estética que se quiere representar”. (79 tokens).*

* Prompt traducido al inglés (respuesta de la IA):

*“Develop a prompt to generate a Synthwave-style image, using the most common color palette (magenta, cyan, violet, blue, and red). The image should depict a futuristic city adapted to this style. Describe the technical features required to maintain the intended aesthetic.” (53 tokens).*

* Prompt optimizado en cantidad de tokens (para los chatbots TKO) en inglés:

*“Synthwave futuristic city, neon lights, grid streets, retro skyline, glowing magenta cyan violet blue red, high contrast, cinematic.” (27 tokens).*
  

* Viabilidad del proyecto: El proyecto es posible de realizar ya que al contar con el acceso a los modelos, es posible testear y optimizar a los mismos para que respondan la manera más eficiente. Dichos modelos ya eran utilizados previamente para trabajar, por lo que esta herramienta busca optimizar los tiempos y mejorar los resultados.


# Objetivo

  El proyecto tiene como finalidad optimizar los tiempos en el desarrollo de prompts avanzados para los modelos utilizados. Esto significa que a partir de un prompt sencillo el modelo nos arroja un prompt avanzado de acuerdo a las indicaciones que se les han otorgado en los distintos datasets. Esto permite reducir los tiempos de producción significativamente y obtener mejores resultados.


# Metodología

A partir de los prompts de salida avanzados en los chatbots generados en base a los prompts sencillos que se presentan el apartado de *"Propuesta de solución"*, se introducen los prompts para generar los contenidos multimedia requeridos en el proyecto. Para los resultados obtenidos se utilizarón los chatbots en su versión de Gemini API free.

---

### Prompt avanzado arrojado por el chatbot de Suno AI (copia textual)

Of course. Based on the deep analysis of the provided documentation, I will develop a complete prompt optimized for Suno v4.5+ to generate a high-quality instrumental Synthwave track.

Here is the complete prompt, designed to leverage Suno's architectural strengths, particularly the Chirp model for instrumentation and the advanced parameters for precise control.


**Full Suno Prompt**

**`Lyrics`:**

> [Intro]
[Atmospheric] [Rain SFX]
> (A lone, distant arpeggio emerges from a wash of lush, dark synth pads. The sound of rain on a futuristic cityscape. A low, resonant hum builds tension.)
(0:00 - 0:20)

> [Verse 1]
[Driving Rhythm]
(A classic gated reverb snare hits, establishing a steady 4/4 beat. A pulsating, rhythmic Moog-style bassline enters, providing the core groove. The main arpeggio becomes clearer and more defined, driving the track forward.)
(0:21 - 1:00)

> [Chorus]
[Euphoric] [Cinematic]
(The main synth lead melody enters—a soaring, melancholic, and powerful hook. Lush synth pads swell underneath, creating a wide, epic wall of sound. The harmony shifts to a more hopeful progression, evoking a panoramic view of a neon-lit metropolis.)
(1:01 - 1:40)

> [Verse 2]
[Introspective]
(The main lead melody fades out, leaving the driving bassline and drum beat. A new, more intricate counter-melody from a crystalline-sounding synth appears, weaving in and out of the main arpeggio.)
(1:41 - 2:20)

> [Bridge]
[Dreamy] [Instrumental Break]
(The drums and bass drop out completely. Only the ethereal, reverb-heavy synth pads remain, holding a sustained chord. A gentle, filtered synth melody plays a simple, nostalgic phrase. A moment of calm and reflection before the climax.)
(2:21 - 2:50)

> [Synth Lead Solo]
[Epic] [Intense]
(The drums and bass crash back in with explosive energy. A virtuosic and emotional synth lead solo takes center stage, full of pitch bends and expressive vibrato. The solo builds in intensity over a powerful chord progression.)
(2:51 - 3:30)

> [Outro]
[Fade Out] [Atmospheric]
(The solo ends, echoing into the distance. The beat and bassline slowly fade away, leaving only the main arpeggio, which gradually gets filtered and slows down. The initial rain sound effect returns, bringing the track full circle as it fades to silence.)
(3:31 - 4:00)

**`Style`:**
> Instrumental 80s Synthwave, Darksynth, Cinematic, Retro-futuristic, Nostalgic, Driving, Melancholic. 120 BPM. Main instrumentation consists of a powerful Moog-style bassline, classic TR-808 style electronic drums with heavy gated reverb on the snare, lush analog synth pads, and a soaring, emotional lead synthesizer melody. Features prominent arpeggiated synth sequences. Production is polished with heavy hall reverb, stereo ping-pong delay, sidechain compression for a pumping effect, and a wide stereo image to create a deep, immersive soundscape. Analog warmth, subtle tape hiss.


**`Exclude Styles`:**
> No vocals, no singing, no rap, no spoken word, no human voice, acoustic instruments, acoustic guitar, piano, orchestra, choir, happy pop, folk, country.



**Recommendations for Advanced Options**

*   **Vocal Gender:**
    *   **Recommendation:** Not applicable as this is an instrumental track. Leave it on the default setting. The `Exclude Styles` field will ensure no vocals are generated.

*   **Weirdness Control:**
    *   **Recommendation:** Set between **30% and 45%**.
    *   **Reasoning:** This range provides a balance between adherence to genre conventions and creative freedom. A value of `30%` will produce a very classic, predictable Synthwave track, ideal for capturing the authentic 80s sound. Increasing it to `45%` allows Suno's Chirp model to introduce subtle, interesting variations in the synth textures or rhythmic patterns without straying from the core aesthetic. This avoids overly experimental or chaotic results while still allowing for a touch of unique AI creativity.

*   **Style Influence:**
    *   **Recommendation:** Set between **75% and 90%**.
    *   **Reasoning:** A high Style Influence is crucial here. The `Style` field is meticulously detailed with specific instrumentation (Moog-style bass, TR-808 drums), production techniques (gated reverb, sidechain compression), and mood descriptors. Setting the influence to `80%` or higher forces the Chirp model to prioritize these explicit instructions over its generalized training. This ensures the final track will have the precise sonic palette requested, from the drum sounds to the atmospheric effects, resulting in a professional and authentic Synthwave sound.
 
Luego de ingresar los prompts en los campos correspondientes, el modelo genera dos canciones por cada creación, por lo que podemos seleccionar una o ambas, dependiendo del proyecto. En este caso seleccione la que consideré que tuvo mejor resultado para el proyecto.

---

### Prompt avanzado arrojado por el chatbot de Adobe Firefly Image 4 (copia textual)

The prompt is designed in two parts: the main creative prompt, which describes the scene in rich detail, and a technical analysis that breaks down the specific parameters to achieve the desired professional result.

**Prompt Optimizado para Adobe Firefly Image 4**

**Prompt Principal:**
> Cinematic, ultra-detailed panoramic shot of a sprawling Synthwave metropolis at perpetual twilight. The scene is viewed from a low angle, looking up at towering, chrome-and-glass skyscrapers that pierce a dark violet sky. Endless multi-level highways weave between the buildings, with the light trails of a sleek, 80s-inspired futuristic sports car creating streaks of crimson red and electric blue. The entire cityscape is bathed in a vibrant, electric glow, dominated by a palette of intense magenta and cool cyan neon signs with retro typography. A giant, stylized sun with a digital grid pattern sinks below the horizon, casting long, dramatic shadows. The wet asphalt of the streets gleams with vivid reflections, and a light atmospheric haze catches the volumetric light, creating a dreamy, nostalgic, and energetic atmosphere. Photorealistic rendering with a subtle film grain.

---

### Análisis y Características Técnicas (Guía de Implementación)

This section explains *why* the prompt is structured this way and how to use Firefly's controls to achieve the perfect Synthwave aesthetic.

1.  **Composición y Encuadre:**
    *   **Instrucción:** `panoramic shot`, `low angle`, `sprawling`.
    *   **Parámetro Firefly:** Set **Aspect Ratio** to **16:9 (`--ar 16:9`)**.
    *   **Justificación:** The 16:9 aspect ratio is essential for creating a cinematic, wide-screen feel that captures the vastness of the city. The low angle makes the skyscrapers feel monumental and imposing, a classic technique in cyberpunk and retro-futuristic art to inspire awe.

2.  **Tipo de Contenido y Estilo:**
    *   **Instrucción:** `Cinematic`, `ultra-detailed`, `Photorealistic rendering`, `subtle film grain`.
    *   **Parámetro Firefly:** Set **Content Type** to **Photo**. Under **Styles**, use keywords like `Synthwave`, `Retrofuturism`, `Vibrant`, `Neon`, and `Cinematic`.
    *   **Justificación:** Although the scene is fantastical, setting the Content Type to "Photo" instructs Firefly to aim for high-fidelity textures, realistic reflections, and sophisticated lighting, which grounds the image. The style keywords reinforce the specific artistic direction, ensuring the model doesn't just create a generic futuristic city. The "subtle film grain" adds a vintage, analog touch authentic to the 80s inspiration.

3.  **Iluminación y Atmósfera:**
    *   **Instrucción:** `perpetual twilight`, `vibrant, electric glow`, `volumetric light`, `gleams with vivid reflections`, `light atmospheric haze`.
    *   **Parámetro Firefly:** Under **Effects**, apply `Glow` or `Bloom` to enhance the neon. In the **Photo Settings**, adjust **Shutter Speed** to a lower value to imply motion blur in the light trails, and increase **Aperture** for a subtle depth of field.
    *   **Justificación:** The lighting is the soul of Synthwave. "Volumetric light" and "haze" are key terms for creating light beams that have a visible presence in the air. Describing the reflections on "wet asphalt" is a classic trope that doubles the impact of the neon lights and adds texture to the scene.

4.  **Paleta de Colores:**
    *   **Instrucción:** `dark violet sky`, `crimson red`, `electric blue`, `intense magenta`, `cool cyan`.
    *   **Parámetro Firefly:** In the prompt itself, specify the colors clearly. You can also use the **Color and Tone** controls to emphasize `Vibrant Color` and set a `Cool Tone` to ensure the blues and violets dominate the shadows.
    *   **Justificación:** The prompt explicitly integrates the requested color palette into the description of the scene's elements (sky, light trails, neon signs). This is more effective than simply listing them, as it gives the AI context for where each color should be applied, ensuring a cohesive and visually striking result.

By combining this detailed descriptive prompt with the strategic use of Firefly Image 4's technical parameters, you will generate a high-quality, aesthetically precise image that fully captures the essence of the Synthwave genre.

---

Para generar la imagen, tomamos el prompt principal y luego podemos guiarnos con la explicación para terminar de configurar la preferencias del modelo tales como referencia, estilos, efectos, color y tono, iluminación y ángilo de cámara. Se adjunta la imagen generada en el repositorio de archivos del proyecto.

# Técnicas de Fast Prompting

  La técnica aplicada para el uso de los chatbots será 'Zero Prompt Shooting', la cual es posible gracias al dataset cargado previamente, sin necesidad de explicarle al modelo cómo debe responder. Para lograr esto, se utilizó la técnica de 'Few Prompt Shooting' dentro del conjunto de datasets para ajustar el comportamiento del modelo, brindandole ejemplos de cómo el modelo interpreta los prompts y qué particularidades tiene cada uno al momento de utiizar cada modelo.


# Implementación

  En el repositorio se encuentran disponibles para descargar los archivos .ipynb perteneciente a los chatbots junto con los *datasets* dentro de los archivos .zip. Los mismos deben correrse con el software 'Jupyter Notebook' ya que el código se encuentra optimizado para el mismo.

# Resultados

Si bien el uso de los chatbots contribuye a generar entradas más complejas a partir de prompts sencillos, es preciso aclarar que a pesar de que los resultados que arroja nos permiten generar los archivos multimedia, es posible que necesitemos iterar el prompt para que la salida del modelo se adapte mejor a nuestras necesidades. Si el resultado satisface parcialmente nuestras necesidades, podemos intervenir en manera manual en el prompt ajustandolo a nuestras necesidades.

# Conclusiones

Para continuar con la optimización y desarrollo de las herramientas, es necesario revisar los datasets correspondientes a cada chatbot para asegurarnos de que los prompts que genera sean factibles de utilizar y no 'alucine' parámetros. En el caso del chatbot para Adobe Firefly Image 4 se puede ver que algunas de las características que arroja para optimizar nuestro prompt no están disponibles en el modelo aunque nos sirve como guía para seleccionar los parámetros que sí se encuentran en el modelo.

# Referencias

https://suno.com/
https://help.suno.com/en
https://www.sunometatagcreator.com/metatags-guide
https://firefly.adobe.com/
https://helpx.adobe.com/ar/firefly/user-guide.html
https://www.adobe.com/cc-shared/assets/pdf/business/teams/sdk/firefly-image-model-4-guide.pdf



  
