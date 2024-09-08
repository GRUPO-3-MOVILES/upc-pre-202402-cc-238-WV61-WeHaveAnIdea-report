# Capítulo 3: Arquitectura

## 3.1. Product design.

### 3.1.1. Style Guidelines.

En esta sección, presentamos el plan detallado de diseño, estilos y estéticas que hemos desarrollado para nuestro proyecto. Este plan se enfoca en asegurar una experiencia de usuario optimizada, proporcionando una interfaz que no solo sea amigable, sino también intuitiva y agradable de utilizar. Nuestra principal meta es garantizar que cada visitante encuentre la navegación sencilla y visualmente atractiva, independientemente de su nivel de experiencia técnica. Para lograr este objetivo, hemos seleccionado cuidadosamente elementos visuales que destacan por su claridad y atractivo estético. Esto implica el uso de una paleta de colores coherente, tipografías legibles y adecuadas para el contenido, así como iconografía y gráficos que complementan el diseño sin saturarlo. Adicionalmente, hemos establecido un conjunto de restricciones específicas para evitar la inclusión de elementos gráficos que puedan resultar discordantes, sobrecargados, o que no contribuyan positivamente a la experiencia del usuario.

Es fundamental comprender que el diseño coherente y estandarizado no solo mejora la estética de una página web, sino que también incrementa la funcionalidad y usabilidad. Estas guías de estilo son esenciales para mantener la uniformidad en la presentación visual y asegurar que cada página o actividad móvil del proyecto ofrezca una experiencia homogénea y profesional. Según Zeldman (2024), una guía de estilo no solo define la apariencia y el comportamiento de los elementos en una interfaz, sino que también establece un marco de trabajo que facilita la colaboración entre los equipos de diseño y desarrollo, asegurando consistencia y eficiencia en la ejecución del proyecto.

#### 3.1.1.1. General Style Guidelines.

En esta sección se presentarán las General Style Guidelines, un conjunto integral de directrices diseñadas para asegurar la coherencia y la calidad visual en todo el proyecto. Se detallará la paleta de colores seleccionada, incluyendo las capas y combinaciones específicas para diferentes contextos de la interfaz, así como las tipografías que se utilizarán para garantizar legibilidad y estética en todos los medios. También se proporcionará información sobre el uso correcto de los logotipos, la iconografía elegida, el modelo de imágenes que se aplicará, y el tipo de lenguaje recomendado para mantener una comunicación clara y efectiva. Estas guías son esenciales para crear una experiencia de usuario unificada y profesional, facilitando así la cohesión en cada aspecto visual y textual del proyecto.

**Colores:**

El color es un componente esencial y destacado en los modelos de diseño de interfaces de usuario, desempeñando un papel crucial en la creación de una experiencia visual impactante. Según Westland y Maggio (2021), la selección cuidadosa de colores para el logotipo y el material de marketing de una empresa puede contribuir significativamente a la construcción de una identidad visual distintiva y fácilmente reconocible. Esta identidad no solo facilita que los consumidores identifiquen y recuerden la marca, sino que también permite que la empresa evoque emociones en su segmento de mercado de manera profunda y subjetiva. Además, en un entorno de mercado altamente competitivo, los colores se convierten en una herramienta vital para que una marca se destaque y se diferencie de sus competidores. Un esquema de colores único o inusual no solo captura la atención de los consumidores, sino que también hace que la marca sea más memorable y presente en la mente del consumidor (Wang et al., 2018).


**Tipografía:**

La tipografía corporativa constituye un elemento fundamental en el diseño integral de una marca. De acuerdo con Dopico (2021), la selección tipográfica genera una respuesta psicológica en el público, lo que puede influir en la percepción de la marca, haciéndola más atractiva, accesible y acogedora. La elección adecuada de una fuente no solo impacta estéticamente, sino que también modifica la experiencia emocional del usuario, contribuyendo a que interactúe de manera diferente con nuestra startup. Es crucial optar por tipografías que no solo refuercen la identidad corporativa, sino que también reflejen fielmente la personalidad y los valores de la empresa, con el objetivo de establecer una conexión emocional más sólida con el público objetivo. Esta estrategia busca fortalecer el vínculo entre la marca y sus usuarios, potenciando su lealtad y afinidad hacia la misma.

Dentro del vasto mundo tipográfico, existen dos grandes categorías que predominan en el diseño: serif y sans-serif.

- **Serif:** Estas tipografías se caracterizan por la presencia de pequeñas líneas o adornos en los extremos de las letras, conocidos como serifas. Estos elementos decorativos suelen proporcionar un aspecto más formal, tradicional y elegante, lo que las hace especialmente adecuadas para medios impresos o textos extensos, como libros o artículos académicos, donde mejoran la legibilidad al guiar la mirada de un carácter a otro. Esta cualidad es particularmente útil en textos largos, ya que facilita el flujo de lectura (Jay & Lupton, 2024). Ejemplos populares de fuentes serif incluyen Times New Roman, que ha sido ampliamente utilizada en medios impresos y documentos formales, y Georgia, una fuente que también equilibra legibilidad y elegancia en medios tanto digitales como impresos.

- **Sans-serif:** Estas tipografías se distinguen por la ausencia de los adornos o serifas, lo que les otorga un diseño más limpio, moderno y minimalista. Debido a su simplicidad, las fuentes sans-serif han ganado popularidad, especialmente en el ámbito digital, donde la claridad y la simplicidad en la presentación del texto son fundamentales para la experiencia del usuario (Jay & Lupton, 2024). Ejemplos de tipografías sans-serif incluyen Arial, una fuente versátil ampliamente utilizada en múltiples plataformas, Helvetica, famosa por su elegancia minimalista, y Roboto, desarrollada específicamente para mejorar la legibilidad en interfaces digitales.

En el contexto de aplicaciones móviles, donde las interfaces están diseñadas para ser funcionales y visualmente atractivas en pantallas pequeñas, las tipografías "sans-serif" son, en general, la mejor opción. Esta preferencia se debe tanto a consideraciones técnicas como de diseño. Entre las principales razones, se pueden encontrar las siguientes:

- **Legibilidad en pantallas pequeñas:** Las pantallas móviles son considerablemente más pequeñas que las de los dispositivos de escritorio, lo que limita el espacio disponible para mostrar texto. Las tipografías sans-serif, al tener líneas simples y limpias sin adornos adicionales, son más fáciles de leer en resoluciones reducidas, lo que optimiza la experiencia del usuario al reducir la fatiga visual (Minakata & Beier, 2022).

- **Claridad en diferentes resoluciones:** Según lo indicado por Gonzalez-Rodrigueza et al. (2024), en el ecosistema móvil, donde los dispositivos pueden tener diferentes densidades de píxeles, las fuentes sans-serif mantienen su nitidez y legibilidad, independientemente de la calidad de la pantalla. Esto asegura una experiencia de lectura consistente tanto en dispositivos de gama baja como en aquellos con pantallas de alta resolución, como los smartphones premium.

- **Estilo moderno y minimalista:** Siguiendo lo indicado por Minakata y Beier (2022), la estética visual de las aplicaciones móviles tiende a seguir principios de diseño minimalista, donde se prioriza la funcionalidad y la simplicidad. Las tipografías sans-serif refuerzan este enfoque, transmitiendo una sensación de orden y modernidad que mejora la navegación y la usabilidad.

- **Rendimiento en interfaces dinámicas:** En aplicaciones móviles, donde el contenido puede ser dinámico y cambiar rápidamente, ya sea mediante animaciones o desplazamientos, las fuentes sans-serif ofrecen una experiencia de lectura más fluida y cómoda. Al carecer de detalles adicionales que puedan generar distracciones, el texto se presenta de manera más accesible y comprensible en todo momento (Vecino et al., 2022).

En base a los puntos expuestos previamente, hemos llegado a la conclusión de que las tipografías sans-serif serán las más adecuadas para la aplicación que se desarrollará bajo el nombre Roademics. Considerando las tendencias actuales en diseño contemporáneo, hemos decidido seleccionar diferentes tipografías según el contexto específico de uso dentro de la aplicación, asegurándonos de que todas mantengan el enfoque sans-serif que resulta esencial para una implementación óptima. A partir de este análisis, hemos identificado y planteado los siguientes escenarios clave:

**- Tipo de Letra Primaria:**

Para la aplicación Roademics, hemos decidido adoptar Raleway como nuestra tipografía primaria. Raleway es una fuente sans-serif que se distingue por su sofisticación y claridad, atributos que consideramos esenciales para proporcionar una experiencia de usuario excepcional. Esta tipografía, con su diseño moderno y estilizado, ofrece una combinación ideal de elegancia y funcionalidad. La estructura geométrica de Raleway no solo mejora la legibilidad, sino que también añade un toque contemporáneo a la interfaz de la aplicación.

El carácter refinado de Raleway la convierte en una elección sobresaliente para los elementos principales de nuestra interfaz, como encabezados, botones y menús. Su diseño uniforme y sus proporciones bien equilibradas aseguran que el texto se presente de manera clara y legible en diversas resoluciones de pantalla y tamaños. Además, la fluidez y la precisión tipográfica de Raleway contribuyen a una estética profesional y pulida, que refuerza la identidad visual de Roademics.

###### Figura 19.
*Presentación de modelos de grosor para el tipo de letra Raleway.*

<img src="/assets/img/capitulo-3/style-guidelines/typography/raleway.png">

**- Tipo de Letra para Soporte de Internacionalidad:**

Para garantizar una representación adecuada en contextos internacionales, hemos seleccionado Noto Sans como nuestra tipografía especializada. Esta fuente sans-serif ha sido cuidadosamente diseñada para ofrecer un soporte extenso a una amplia variedad de idiomas y sistemas de escritura. Gracias a su diseño versátil, Noto Sans asegura que el texto se muestre de manera clara, legible y consistente, sin importar la configuración lingüística o regional en la que se utilice.

Según lo aclarado por Huang (2019), la implementación de Noto Sans contribuye a la accesibilidad y la inclusividad, aspectos fundamentales para ofrecer una experiencia de usuario universal. Al utilizar esta tipografía, no solo garantizamos una presentación uniforme del contenido en distintos contextos internacionales, sino que también reafirmamos nuestro compromiso con la adaptabilidad y la consideración de las necesidades globales de nuestros usuarios.

###### Figura 20.
*Presentación de modelos de grosor para el tipo de letra Noto Sans en General.*

<img src="/assets/img/capitulo-3/style-guidelines/typography/noto-sans.png">

El propósito principal de Noto Sans en nuestra aplicación Roademics es facilitar una experiencia globalizada, abordando las necesidades de una audiencia diversa. Esta tipografía ha sido elegida para su uso en todos los aspectos de la aplicación que requieren un enfoque inclusivo, asegurando que todos los usuarios, sin importar su idioma o sistema de escritura, puedan interactuar con la aplicación de manera efectiva.

###### Figura 21.
*Presentación de modelos de grosor para el tipo de letra Noto Sans en Japonés.*

<img src="/assets/img/capitulo-3/style-guidelines/typography/noto-sans-japanese-script.png">

###### Figura 22.
*Presentación de modelos de grosor para el tipo de letra Noto Sans en Chino Tradicional.*

<img src="/assets/img/capitulo-3/style-guidelines/typography/noto-sans-traditional-chinese-script.png">

###### Figura 23.
*Presentación de modelos de grosor para el tipo de letra Noto Sans en Tailandés.*

<img src="/assets/img/capitulo-3/style-guidelines/typography/noto-sans-thai-script.png">

###### Figura 24.
*Presentación de modelos de grosor para el tipo de letra Noto Sans en Coreano.*

<img src="/assets/img/capitulo-3/style-guidelines/typography/noto-sans-korean-script.png">

###### Figura 25.
*Presentación de modelos de grosor para el tipo de letra Noto Sans en Árabe.*

<img src="/assets/img/capitulo-3/style-guidelines/typography/noto-sans-arabic-script.png">

**- Tipo de Letra Complementaria:**

En situaciones en las que debemos depender del conjunto de fuentes disponible en los dispositivos de los usuarios, como es el caso de las campañas de correo electrónico o SMS, utilizaremos Arial. Esta fuente sans-serif se distingue por su amplia compatibilidad con una variedad de sistemas operativos y plataformas, lo que garantiza que el contenido se presente de manera uniforme y consistente en distintos entornos digitales.

Arial es apreciada por su claridad y simplicidad, atributos que la convierten en una opción confiable para comunicaciones por correo electrónico, mensajes SMS, y otros medios similares. Su diseño neutral y funcional asegura que el texto se mantenga legible y profesional en diferentes tamaños y resoluciones de pantalla, proporcionando una experiencia de usuario sin inconvenientes. Al optar por Arial, garantizamos que nuestras formas de comunicación digital mantengan una presentación clara y coherente, reforzando la efectividad de nuestra comunicación y la profesionalidad de nuestra marca.

###### Figura 26.
*Presentación de modelos de grosor para el tipo de letra Arial.*

<img src="/assets/img/capitulo-3/style-guidelines/typography/arial.png">

### 3.1.2. Information Architecture.

#### 3.1.2.1. Organization Systems.

#### 3.1.2.2. Labelling Systems.

#### 3.1.2.3. SEO Tags and Meta Tags.

#### 3.1.2.4. Searching Systems.

#### 3.1.2.5. Navigation Systems.

### 3.1.3. Landing Page UI Design.

#### 3.1.3.1. Landing Page Wireframe.

#### 3.1.3.2. Landing Page Mock-up.

### 3.1.4. Mobile Applications UX/UI Design.

#### 3.1.4.1. Mobile Applications Wireframes.

#### 3.1.4.2. Mobile Applications Wireflow Diagrams.

#### 3.1.4.3. Mobile Applications Mock-ups.

#### 3.1.4.4. Mobile Applications User Flow Diagrams.

#### 3.1.4.5. Mobile Applications Prototyping.

## 3.2. Architecture Overview.

### 3.2.1. Domain-Driven Software Architecture.

#### 3.2.1.1. Software Architecture Context Level Diagram.

#### 3.2.1.2. Software Architecture Container Level Diagram.

#### 3.2.1.3. Software Architecture Components Diagram.

### 3.2.2. Software Object-Oriented Design.

#### 3.2.2.1. Class Diagrams.

#### 3.2.2.2. Class Dictionary.

#### 3.2.2.3. Database Design.

#### 3.2.2.4. Database Diagram.
