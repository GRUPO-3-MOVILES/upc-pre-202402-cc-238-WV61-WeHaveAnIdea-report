# Capítulo 4: Backend Product Implementation & Validation

## 4.1. Software Configuration Management.

En la gestión de la configuración del backend para la aplicación móvil Roademics, nos centramos en el control eficiente del código fuente, asegurando un manejo riguroso de versiones mediante sistemas como Git, y manteniendo una estructura modular y organizada durante todo el ciclo de desarrollo. Implementamos pipelines de CI/CD (Integración Continua y Despliegue Continuo) que automatizan pruebas, integraciones y despliegues en los entornos de desarrollo, pruebas y producción. Asimismo, nos aseguramos que todos los bounded context estén correctamente versionados y alineados con la infraestructura en, permitiendo una fácil integración con las APIs externas como Firebase Authentication, Stripe y Twilio.

Estas decisiones son críticas para asegurar la eficiencia, coherencia y flexibilidad en la estructura del backend, lo que nos permite responder de manera ágil a las necesidades de los usuarios finales. De este modo, garantizamos una plataforma robusta y escalable, optimizada para manejar grandes volúmenes de solicitudes y datos de forma segura. Adicionalmente, la correcta gestión del backend asegura que tanto los reclutadores y empresas, como los estudiantes y profesionales, puedan interactuar de forma fluida con la plataforma, explorando y gestionando los roadmaps profesionales. Todo ello se complementa con la infraestructura descrita en los capítulos posteriores de esta documentación.

### 4.1.1. Software Development Environment Configuration.

En esta sección, el equipo de desarrollo detallará las herramientas de software esenciales para el backend de la aplicación móvil, especificando el nombre de cada producto, su propósito dentro del proyecto, y el método de acceso o instalación. Para las herramientas basadas en SaaS (Software como servicio), se proporcionará la URL de acceso a sus páginas web, mientras que para aquellas que requieren ejecución en servidores locales, se indicará la ruta de descarga. 

Las herramientas seleccionadas cubren actividades críticas para el backend, como la gestión de bases de datos, control de versiones, servidores de aplicaciones, despliegues, integración continua y entrega continua (CI/CD), monitoreo de servicios, gestión de API, y la documentación técnica de los servicios del backend.

**Project Management**: Esta sección aborda la planificación y supervisión del proyecto durante todo su ciclo de vida, incluyendo la coordinación del equipo, la gestión de sus tareas y colaboraciones, así como la asignación de responsabilidades previamente establecidas. Para estructurar esta gestión, hemos dividido el enfoque en métodos distintos de comunicación y administración del equipo.

- Reuniones de Trabajo: Para la coordinación de las tareas del equipo de backend, utilizamos "Discord" como plataforma principal de comunicación. Esta elección se fundamenta en la familiaridad del equipo con la herramienta, lo que permite una comunicación ágil y efectiva para la discusión de temas técnicos relacionados con la infraestructura del backend. Aunque "Discord" no posee ciertas características avanzadas de otras plataformas, su interfaz intuitiva y la posibilidad de reuniones sin restricciones de tiempo nos facilitan la planificación detallada de la arquitectura y la resolución de problemas complejos del backend. Además, los canales temáticos permiten organizar conversaciones específicas sobre desarrollo, despliegue, base de datos y gestión de servicios externos, mejorando el seguimiento de los temas relevantes al backend.

Página oficial de Discord: https://discord.com/

- Control de Versiones: Para la gestión del control de versiones del backend, utilizamos las herramientas integradas de "Github". Esta plataforma permite al equipo colaborar de manera eficiente a través de commits y pull requests específicos para el código del backend. Los commits documentan detalladamente los cambios realizados en la lógica del servidor y los servicios externos, proporcionando un historial claro para revisar y rastrear las modificaciones en la infraestructura del backend. Los pull requests facilitan la revisión y discusión de los cambios antes de integrarlos en la rama principal, asegurando que las nuevas funcionalidades del backend se implementen de forma controlada y sin comprometer la estabilidad del sistema. Este enfoque ayuda a mantener la integridad del backend y permite identificar y revertir errores críticos si es necesario.

Página oficial de Github: https://github.com/

---

**Requirements Management**: Para asegurar una organización efectiva del trabajo en nuestro equipo, en esta sección hemos implementado una metodología que utiliza herramientas diseñadas para la asignación y seguimiento de tareas, así como para la gestión de los requisitos del proyecto. En particular, hemos empleado una serie de programas que presenten listas organizadas junto a tableros con los objetivos y metas que necesitamos completar, ademas de todos los puntos que falten completar.

- Organización de tareas: Hemos adoptado ClickUp como nuestra herramienta principal para la gestión de tareas del backend. La plataforma ofrece una interfaz amigable que facilita la división de las actividades relacionadas con la infraestructura y el desarrollo del backend entre los miembros del equipo. Al crear tableros personalizados y asignar tareas específicas del backend, podemos establecer plazos, asignar responsables y monitorear el progreso de cada tarea técnica de manera eficiente. Esta configuración nos permite evaluar el avance en la implementación de la API, servicios externos y despliegues, así como analizar el desempeño general del equipo de backend. ClickUp también permite revisar las contribuciones individuales y el trabajo realizado en la parte del servidor, promoviendo la transparencia y la colaboración efectiva dentro del equipo técnico.

Página oficial de ClickUp: https://clickup.com/ 

---

**Product Architecture Design**: Esta sección se centra en el desarrollo y diseño de la arquitectura del backend a lo largo de todo su ciclo de vida. Las herramientas seleccionadas deben ofrecer aplicaciones que permitan la creación de diagramas detallados y complejos de cada capa de la arquitectura del backend. Esto incluye la identificación de los componentes clave, como bases de datos, APIs y servicios externos, así como los frameworks, entornos de desarrollo (IDEs) y lenguajes de programación que se utilizarán. La capacidad de representar de manera clara y precisa la estructura del backend es esencial para asegurar que todos los aspectos técnicos sean comprensibles, bien documentados y alineados con los requisitos del sistema.

- Diagramas C4: Para diseñar los diagramas C4 del backend de nuestro proyecto, nuestro equipo ha optado por utilizar "Visual Paradigm". Esta herramienta ha sido seleccionada por sus características específicas que facilitan el modelado claro y efectivo de las vistas de arquitectura del backend según el enfoque C4. "Visual Paradigm" se destaca por su simplicidad en la creación de diagramas estructurados y su capacidad para ofrecer una representación visual comprensible tanto para desarrolladores como para partes interesadas no técnicas. La elección de esta herramienta se basa en su capacidad para generar diagramas detallados y precisos del backend sin necesidad de codificación de bajo nivel, lo que la convierte en una opción accesible y eficaz para documentar la arquitectura del backend de nuestro proyecto.

Página oficial de Visual Paradigm: https://www.visual-paradigm.com/

- Diagramas UML: Para el diseño de los diagramas UML relacionados con la arquitectura del backend de nuestro proyecto, hemos optado por "LucidChart". Esta plataforma es especialmente adecuada para la creación de diagramas UML del backend debido a su interfaz intuitiva y su amplia gama de herramientas específicas para el modelado de sistemas. "LucidChart" permite crear diagramas detallados y bien estructurados que representan con precisión la arquitectura del backend, incluyendo la estructura de bases de datos, relaciones entre microservicios y flujos de datos. La facilidad de uso y las opciones avanzadas para organizar y estructurar los diagramas hacen que "LucidChart" sea la herramienta ideal para garantizar una representación clara y completa de la arquitectura del backend. Su capacidad para integrar y organizar partes del diagrama facilita la colaboración y la comunicación entre los miembros del equipo técnico, especialmente entre los desarrolladores y arquitectos de software involucrados en el proyecto.

Página oficial de LucidChart: https://lucidchart.com/

- Diseño de Diagrama de Bases de Datos: Para el diseño de la base de datos no relacional de nuestro proyecto, hemos optado por "Moon Modeler". Esta herramienta es eficaz para el modelado y visualización de bases de datos no relacionales, como MongoDB. Ofrece una interfaz intuitiva que facilita la creación de diagramas detallados y bien estructurados, permitiendo diseñar esquemas claros y precisos para la estructura de datos del backend. "Moon Modeler" proporciona funcionalidades como la generación automática de documentación y la exportación de diseños en varios formatos, lo cual es esencial para una correcta representación y documentación de la base de datos. Aunque la herramienta está diseñada para el trabajo individual y no está orientada a la colaboración en tiempo real, permite la creación y revisión de modelos de datos, con la colaboración facilitada a través del intercambio de archivos exportados. Esta característica debe ser considerada al integrar el diseño de bases de datos en el flujo de trabajo del equipo de backend.

Página oficial de Moon Modeler: https://www.datensen.com/data-modeling/moon-modeler-for-databases.html 

**Product UX/UI Design**:

Esta sección abarca el desarrollo y diseño de las interfaces UX y UI para nuestro proyecto durante todo su ciclo de vida. Las herramientas seleccionadas deben ofrecer la flexibilidad para modificar la estética de las páginas y garantizar una experiencia óptima para nuestros usuarios finales, alineándose con las historias de usuario y las metodologías de desarrollo móvil. También es fundamental que estas herramientas permitan la estructuración y diagramación adecuada de todos los elementos necesarios.

**Mapas y User Personas**: Para la creación y seguimiento de mapas como el Empathy Map, Journey Map e Impact Map, hemos optado por la plataforma "UXPressia". Esta herramienta se distingue por su interfaz intuitiva y su conjunto de funcionalidades integradas que facilitan la elaboración detallada de estos mapas, esenciales para entender mejor a nuestros usuarios y sus necesidades. UXPressia permite colaborar de manera eficiente, ya que ofrece capacidades de trabajo en equipo en tiempo real, lo cual es crucial para mantener la coherencia y la calidad en el diseño.
Además, UXPressia proporciona herramientas para crear User Personas con modelos predefinidos y plantillas adaptables, que nos ayudan a representar de forma clara y visual los perfiles de nuestros usuarios objetivo. Aunque la plataforma puede tener algunas limitaciones en la creación de gráficos complejos, su enfoque en la simplicidad y la usabilidad compensa estas restricciones. Su capacidad para integrar y visualizar datos de manera efectiva asegura que nuestros mapas y personas sean precisos y útiles para el desarrollo del producto.

Página oficial de UXPressia: https://uxpressia.com/

**Escenarios**: Para modelar los escenarios AS-IS y TO-BE de nuestros segmentos de mercado, hemos seleccionado la herramienta "Miro". Miro es una plataforma altamente versátil que ofrece una amplia gama de plantillas y modelos para la creación de diagramas, tablas y mapas visuales. Su capacidad para facilitar la colaboración en tiempo real es una de sus principales ventajas, permitiendo que varios miembros del equipo trabajen juntos simultáneamente, lo cual mejora la calidad y la coherencia de los resultados finales. Miro también ofrece funcionalidades para crear mapas de procesos y diagramas de flujo detallados, que son esenciales para comprender las interacciones actuales y planificar mejoras futuras. La interfaz de Miro es intuitiva y permite una navegación fluida, lo que hace que el proceso de modelado sea eficiente y menos propenso a errores.

Página oficial de Miro: https://miro.com/

**Wireframes, Mock-ups, Prototypes y Diseño Móvil**: Para la creación de wireframes, mock-ups y prototipos de la landing page de nuestra startup y la interfaz de la aplicación móvil, hemos optado por "Figma". Figma es una herramienta poderosa y especializada en el diseño de interfaces digitales, ofreciendo un conjunto completo de funcionalidades para la creación de prototipos interactivos y el diseño colaborativo. La plataforma permite a los diseñadores trabajar en tiempo real, lo que facilita la comunicación y el intercambio de ideas entre los miembros del equipo, y asegura que el proceso de diseño sea ágil y eficiente. Figma también incluye una extensa biblioteca de componentes y recursos que pueden ser reutilizados, lo que acelera la creación de diseños consistentes y de alta calidad. Además, la capacidad de Figma para integrar comentarios y revisiones directamente en el diseño facilita la iteración y la mejora continua del producto. Esta herramienta es ideal para el diseño móvil, ya que ofrece características específicas para adaptar interfaces a diferentes dispositivos y resoluciones.

Página oficial de Figma: https://figma.com/

---

**Web Services**: En esta sección estarán las herramientas de desarrollo del Web Services con el Backend. Es esencial adoptar frameworks y metodologías que garanticen una programación eficiente y la implementación de un backend robusto y de alto rendimiento. Utilizaremos frameworks que proporcionen bibliotecas preimplementadas para facilitar la creación, configuración y manejo de los servicios web. Estos frameworks permiten una integración fluida de los servicios, optimizando el rendimiento y asegurando que el backend pueda manejar de manera eficiente las solicitudes y respuestas entre los diferentes componentes del sistema.

- Modelo de Arquitectura: El estilo arquitectónico elegido para la aplicación será RESTful API, conocido por su eficacia en establecer una comunicación eficiente y directa entre clientes y servidores. Este enfoque es ampliamente reconocido por su capacidad para alinearse con las mejores prácticas de diseño y seguridad, lo que resulta fundamental para cualquier aplicación moderna. Al adoptar este estilo arquitectónico, se garantiza la creación de un backend no solo robusto, sino también altamente escalable, capaz de adaptarse a las crecientes demandas del sistema. Esto, a su vez, promueve un desarrollo coherente y seguro, estableciendo las bases necesarias para un rendimiento óptimo y una experiencia de usuario fiable.

Página de guía y seguimiento para el modelo REST: https://es.apis.support.brightcove.com/getting-started/learning-guide-using-rest-apis.html 

- Desarrollo de código: Para el desarrollo propio del código del backend, se optará por utilizar Java junto con el framework Spring Boot. Spring Boot facilita enormemente la creación de aplicaciones basadas en Spring, ya que ofrece un conjunto completo de funcionalidades preconfiguradas para construir servicios web eficientes y rápidos. Mientras tanto, Java es un lenguaje de programación altamente robusto y versátil, conocido por su eficiencia, seguridad y amplia comunidad de soporte. Esta combinación de tecnologías permite establecer un entorno de desarrollo sólido y flexible, adaptado a las necesidades actuales del proyecto. Al emplear Spring Boot con Java, se garantiza una infraestructura capaz de manejar las demandas de un backend de alto rendimiento, ofreciendo escalabilidad, mantenibilidad y una integración más fluida con otros componentes del sistema.

Página oficial de Spring Boot: https://spring.io/projects/spring-boot

Página de guía y seguimiento para Java: https://www.oracle.com/java/technologies/javase-jdk11-downloads.html

- Entorno de desarrollo integrado: El IDE seleccionado para este proceso será IntelliJ IDEA, que forma parte del conjunto de herramientas de JetBrains Toolbox. IntelliJ IDEA es ampliamente reconocido por sus potentes características específicas para el desarrollo en Java, brindando un entorno que facilita enormemente la codificación, depuración y gestión de proyectos. Gracias a sus funciones avanzadas, como la autocompletación inteligente, análisis de código en tiempo real y herramientas de refactorización, se logra un proceso de desarrollo más ágil y productivo, reduciendo significativamente los errores y mejorando la calidad del código.

Página oficial de IntelliJ IDEA: https://www.jetbrains.com/idea/

- Documentación de servicios web: Se empleará Swagger, basado en la OpenAPI Specification. Swagger se ha consolidado como un estándar en la industria para la documentación de APIs, ya que ofrece una estructura clara y coherente que facilita su comprensión y uso, tanto por desarrolladores internos como externos. Además, Swagger permite registrar y reflejar rápidamente los cambios realizados en la API durante el proceso de desarrollo, garantizando que la documentación se mantenga precisa y actualizada en todo momento. Esto no solo mejora la comunicación entre los equipos, sino que también asegura un desarrollo más eficiente y colaborativo.

Página oficial de Swagger: https://swagger.io/

---

**Database Development**: Esta sección aborda las herramientas y aplicaciones esenciales para la implementación efectiva de la base de datos que sustentará el ciclo de vida completo del proyecto. Se enfatiza la selección de recursos tecnológicos que no solo sean accesibles y fáciles de utilizar, sino que también ofrezcan un alto grado de fiabilidad y robustez. Esto es crucial para asegurar que la base de datos se implemente de manera eficiente, minimizando riesgos de bajo rendimiento o inconsistencias operativas que puedan comprometer la integridad de los datos y la fluidez de los procesos del proyecto. 

- Gestor de bases de datos: Se ha decidido utilizar MongoDB como el sistema de gestión de bases de datos no relacional. MongoDB está diseñado para manejar grandes cantidades de datos no estructurados y semi-estructurados, lo que es ideal para una plataforma social donde los usuarios pueden generar diversos tipos de contenidos, desde textos hasta imágenes y videos, hasta sus propios roadmaps y hojas de ruta. Además, al ser una base de datos orientada a documentos, MongoDB permite una mayor flexibilidad en el almacenamiento y modelado de datos, lo que facilita la evolución de las funcionalidades de la red social sin necesidad de modificaciones extensivas en la estructura de la base de datos. 

Página oficial de MongoDB: https://www.mongodb.com/es 

- Despliegue de la base de datos: Se ha decidido utilizar MongoDB Atlas como la plataforma de despliegue para la base de datos. MongoDB Atlas es un servicio en la nube completamente gestionado que ofrece todas las ventajas de MongoDB, pero con el beneficio adicional de simplificar su administración y escalabilidad. Atlas permite una implementación rápida y sin complicaciones, asegurando la disponibilidad global de los datos y facilitando su distribución geográfica.

Página oficial de MongoDB Atlas: https://www.mongodb.com/products/platform/atlas-database 

---

**Software Development**:

Esta sección se centra en las herramientas y aplicaciones necesarias para la programación de la landing page y la aplicación móvil de nuestro proyecto durante todo su ciclo de vida. Los instrumentos seleccionados incluyen IDEs, lenguajes de programación, bibliotecas y frameworks que deben alinearse con las metodologías y principios establecidos en el proyecto. Estos deben cumplir con las historias de usuario y los esquemas definidos para alcanzar los objetivos de nuestra startup y satisfacer las necesidades de nuestros segmentos objetivos.

En el proceso de desarrollo de la aplicación móvil, se emplearán herramientas específicas para garantizar una programación eficiente y una integración adecuada con los distintos componentes del proyecto. Para la implementación técnica, se utilizará Kotlin como lenguaje de programación. Kotlin, conocido por su interoperabilidad con Java y su sintaxis concisa, proporciona una base sólida y moderna para el desarrollo de aplicaciones móviles en el entorno de Android.

Landing Page: La landing page será desarrollada utilizando HTML5, CSS3 y JavaScript nativo. Cada uno de estos lenguajes se gestionará en secciones específicas dentro del repositorio del proyecto, lo que garantiza una estructura organizada y eficiente. HTML5 y CSS3 se encargarán de la estructura y el diseño de la página, mientras que JavaScript nativo permitirá añadir interactividad y funcionalidad dinámica. Esta combinación asegura que la página sea robusta, flexible y adecuada para un entorno de producción.

Además, para mantener una interfaz clara y coherente, la landing page seguirá las directrices del Material Design. Este enfoque, conocido por su consistencia en el diseño de interfaces de usuario, contribuirá a una experiencia visualmente atractiva y funcional. En cuanto a las herramientas de desarrollo, se utilizará Visual Studio Code como el IDE principal. Aunque es más sencillo en comparación con otros IDEs más avanzados, su amplia gama de funcionalidades y extensiones facilita el proceso de programación, haciéndolo una opción efectiva para este proyecto.

Página oficial de Visual Studio Code: https://code.visualstudio.com/

Guías y recursos adicionales:

HTML: https://www.w3schools.com/html/

CSS: https://www.w3schools.com/css/default.asp

Javascript: https://developer.mozilla.org/es/docs/Web/JavaScript

Material Design: https://m3.material.io/Design

**Aplicación Móvil**: La aplicación móvil será desarrollada utilizando Flutter con VSCode como el entorno de desarrollo integrado (IDE). Flutter, el kit de herramientas de UI de Google para crear aplicaciones nativas compiladas para dispositivos móviles, web y escritorio a partir de una única base de código, ofrece una forma eficiente y flexible de construir interfaces de usuario atractivas y de alto rendimiento. VSCode es un IDE ligero pero potente que proporciona una integración fluida con Flutter, facilitando el desarrollo, la depuración y el diseño de la aplicación móvil.

El diseño de la interfaz de usuario de la aplicación se basará en los principios del Material Design, garantizando una experiencia de usuario intuitiva y visualmente atractiva. Flutter proporciona un conjunto completo de widgets y herramientas para implementar estos principios, permitiendo la creación de interfaces de usuario consistentes y funcionales.

Página oficial de Flutter: https://flutter.dev

Guías y recursos adicionales:

Material Design: https://m3.material.io

VSCode: https://code.visualstudio.com

---

**Software Deployment**:

Esta sección aborda las herramientas y aplicaciones necesarias para llevar a cabo el despliegue e implementación efectiva de todas las páginas web desarrolladas a lo largo del ciclo de vida del proyecto. Los recursos seleccionados deben ser fáciles de usar y ofrecer alta confiabilidad para asegurar que las páginas se publiquen sin problemas de rendimiento o inconsistencias en su formato.
Para el despliegue de la Landing Page, se utilizará GitHub Pages, que proporciona un rendimiento eficiente y confiable al alojar los sitios web directamente desde los repositorios en la misma plataforma. Dado que la Landing Page es estática, no requerirá actualizaciones frecuentes ni cambios continuos, lo que hace que GitHub Pages sea una opción adecuada para su implementación.

Página oficial de GitHub Pages: https://pages.github.com/

- Despliegue del Backend: Se optará por utilizar servicios en la nube como AWS o Heroku, que proporcionan un entorno robusto y confiable para alojar aplicaciones. Estas plataformas ofrecen escalabilidad y monitorización en tiempo real, lo que asegura que el backend pueda manejar las demandas del sistema de manera eficiente. Además, su facilidad de configuración y despliegue automatizado contribuye a un proceso de implementación fluido y seguro.
  
---

**Software Document**: Esta sección detalla las herramientas y aplicaciones seleccionadas para la documentación exhaustiva del código y del software a lo largo del ciclo de vida del proyecto. Las herramientas deben ser intuitivas para todos los miembros del equipo y capaces de gestionar documentación extensa, con soporte para imágenes y una estructura de secciones clara y organizada.

- Documentación del proceso e informe de software: Se utilizará un repositorio en GitHub, estructurado en múltiples ramas según las necesidades del equipo. La redacción de la documentación se llevará a cabo principalmente en Markdown, lo que garantiza una visualización coherente en la web a través de diferentes dispositivos, además de facilitar la compresión y el cifrado de los datos. En situaciones donde Markdown no sea suficiente, como para la creación de tablas complejas, se empleará HTML para lograr una representación más precisa y detallada.

Página oficial de GitHub: https://github.com/

Guía de uso de Markdown: https://www.markdownguide.org/

Guía y seguimiento para HTML5: https://www.w3schools.com/html/

### 4.1.2. Source Code Management.

En esta sección, se definirá la estrategia para utilizar GitHub como plataforma de control de versiones y colaboración durante el ciclo de vida del desarrollo del backend. Se emplearán todas las herramientas proporcionadas por GitHub para garantizar una gestión eficaz del código fuente, incluyendo el seguimiento de versiones y la colaboración entre miembros del equipo. Se mantendrá un registro exhaustivo de las versiones del backend, permitiendo rastrear cambios, identificar nuevos desarrollos y corregir errores de manera precisa.

Se establecerán ramas específicas para diferentes etapas del desarrollo, tales como la integración continua, las pruebas y la producción. Además, se implementarán políticas de pull requests y revisiones de código para asegurar la calidad y coherencia del backend. Esta metodología permitirá un control riguroso del ciclo de vida del desarrollo, facilitando la colaboración y asegurando que todos los cambios se registren de forma clara y ordenada.

A continuación, se proporciona una lista con los enlaces a la organización de GitHub de WHAI y a los repositorios específicos relacionados con el desarrollo del backend dentro de esta organización:

Repositorios en GitHub:

- Repositorio principal de la organización de Roademics: https://github.com/GRUPO-3-MOVILES 

- Repositorio del reporte y documentación de Roademics: https://github.com/GRUPO-3-MOVILES/upc-pre-202402-cc-238-WV61-WeHaveAnIdea-report 

- Repositorio con todo el código correspondiente al BackEnd de Roademics: https://github.com/GRUPO-3-MOVILES/WeHaveIdea

**Integrantes de la organización**:
En esta sección, se presentarán todos los usuarios que forman parte de la organización de GitHub del proyecto WHAI, junto con sus nombres de usuario correspondientes. El objetivo es evitar confusiones sobre los autores de los commits en GitHub y facilitar la identificación de los colaboradores al revisar y analizar el reporte y el código desarrollado por nuestro equipo.


###### Tabla 23.

*Modelo de integrantes del equipo dentro de la página de organización de Github*

|**Nombre de Usuario**|**Imagen de Perfil**|**Nombre del Integrante del Equipo**|
| ----- | ------ | ----- |
| JuanPescoran | <img src="/assets/img/capitulo-4/profiles/Juan-github.PNG" alt="Pescorán Angulo, Juan Fabritzzio">| Pescorán Angulo, Juan Fabritzzio - U20221C936 |
| FlavioTrigueros | <img src="/assets/img/capitulo-4/profiles/Flavio-github.PNG" alt="Trigueros Chumacero, Flavio Eduardo"> | Trigueros Chumacero, Flavio Eduardo - U202210190 |
| AldhaValenzuelaH | <img src="/assets/img/capitulo-4/profiles/Aldhair-github.PNG" alt="Valenzuela Huillcaya, Aldhair Johan Juan"> | Valenzuela Huillcaya, Aldhair Johan Juan - U20201F572 |
| LucioY250 | <img src="/assets/img/capitulo-4/profiles/Lucio-github.PNG" alt="Yen Cerna, Lucio Heli"> | Yen Cerna, Lucio Heli - U202213143 |

**GitFlow Workflow**:

En nuestro proyecto, implementaremos el modelo GitFlow para el control de versiones, el cual está estructurado en torno a ramas principales y secundarias. Las ramas principales actúan como las bases fundamentales para el desarrollo y la implementación final del backend. La rama master representa la versión estable y en producción, mientras que develop se utiliza para integrar todas las características y correcciones que se encuentran en desarrollo.

Las ramas secundarias se utilizan para gestionar desarrollos específicos y modificaciones puntuales. Estas ramas se crean para el desarrollo de nuevas funcionalidades, para abordar errores críticos en producción y para preparar la versión para su liberación final. Cada una de estas ramas se fusiona con develop a través de pull requests, los cuales son revisados por el equipo para asegurar la calidad y coherencia del código. Este enfoque asegura que cada cambio se maneje de manera organizada y que los errores críticos se aborden de forma eficiente, manteniendo la estabilidad del proyecto en todo momento.

Esta metodología garantiza una organización efectiva del flujo de trabajo, facilita la colaboración entre los miembros del equipo y optimiza la gestión de versiones del backend, asegurando que todos los cambios se integren de manera controlada y que el historial del proyecto sea claro y manejable. A continuación, se detallan las convenciones para nombrar las ramas dentro de nuestra organización:

**Ramas Principales**:

- `master`: Esta rama contiene la versión final y estable del backend, lista para su despliegue en el entorno de producción. Las integraciones a esta rama deben pasar por una revisión exhaustiva por parte del equipo técnico para asegurar la calidad y estabilidad del código del backend.
  
- `develop`: Esta rama agrupa los elementos en desarrollo relacionados con el backend, que han sido aprobados por al menos un miembro del equipo diferente del autor de las modificaciones. Sirve como etapa de integración y prueba de nuevas funcionalidades del backend antes de ser fusionadas con `master`.

**Ramas de Funcionalidades (Feature Branches)**:

###### Tabla 24.

*Modelo de todas las ramas implementadas dentro de la organización del proyecto en Github.*

| Nombre | Descripción |
|--------|-------------|
| feat/iam | Gestiona los cambios relacionados con la implementación del sistema de gestión de identidades y accesos (IAM) en el backend. Esta implementación asegura la autenticación, autorización y control de permisos de usuarios, garantizando la seguridad del sistema y un acceso adecuado a los recursos según los roles asignados. |
| feat/roadmaps | Agrupa los cambios correspondientes a la gestión de los roadmaps en el backend, incluyendo la lógica para la creación, almacenamiento y procesamiento de los datos relacionados con los roadmaps de los usuarios. Esto abarca la implementación de endpoints para la manipulación de datos, así como la optimización de consultas y almacenamiento en la base de datos para asegurar un rendimiento eficiente. |

**Ramas Individuales**: Estas ramas se utilizan para desarrollos individuales realizados por los miembros del equipo en el backend. Los cambios se integran a las ramas principales mediante pull requests, que deben ser aprobados por el líder del equipo. Una vez que los cambios han sido completados y fusionados, estas ramas se eliminan para evitar la acumulación innecesaria de ramas y mantener un repositorio limpio y organizado.

---

Para asegurar una convención clara y coherente en el nombramiento de ramas, así como en los modelos de pull requests y commits realizados por los miembros del equipo de backend, hemos establecido el siguiente formato estándar:

**Formato de Commit:**

|feat(branch): verb + brief description in English|
|-------------------------------------------------|
En este formato, "branch" debe indicar la rama en la que se han realizado los cambios propuestos para una nueva funcionalidad del backend. La descripción debe estar escrita en inglés y comenzar con un verbo que refleje claramente la naturaleza del cambio implementado. A continuación, se presenta una tabla con verbos recomendados para los mensajes de commit:

###### Tabla 25
*Modelo de escritura de verbos para todos los commits realizados en el proyecto de Github*

| Verbo | Traducción | Uso en el proyecto de programación |
|-------|------------|------------------------------------|
|Add  |Añadir  | Utilizado para añadir nuevas funcionalidades, clases o módulos al backend. Ideal para commits en los que se implementan nuevas APIs, controladores, o servicios, incrementando la capacidad del sistema sin afectar las funcionalidades existentes.  |
|Create  |Crear  | Empleado para la creación de nuevos esquemas de bases de datos, endpoints o controladores en el backend. Este verbo se usa cuando se inicia el desarrollo de una nueva característica o arquitectura dentro del sistema, estableciendo la base técnica sobre la cual se expandirá la funcionalidad.  |
|Update  |Actualizar  | Usado para realizar modificaciones menores en las funcionalidades existentes del backend, como la actualización de dependencias, optimización de consultas o ajustes en la lógica del controlador. Se aplica en casos donde los cambios no alteran significativamente la estructura, pero mejoran el rendimiento o corrigen comportamientos. |
|Modify  |Modificar  | Aplicado cuando se realizan cambios significativos en la lógica del backend, como la reestructuración de servicios o la implementación de nuevas políticas de negocio en la capa de lógica. Esto incluye cambios que afectan la arquitectura general o que impactan directamente en la interacción entre componentes.  |
|Correct  | Corregir  | Utilizado para corregir errores menores en la implementación del backend, como ajustes en las validaciones de entradas, corrección de rutas de API, o fallos en configuraciones que afectan el correcto funcionamiento del sistema. Este verbo se reserva para pequeñas correcciones sin grandes implicaciones. |
|Fix  |Arreglar  | Usado para solucionar bugs críticos o problemas que afectan directamente la funcionalidad del backend. Esto puede incluir arreglar errores en la lógica de negocio, problemas de conexión con la base de datos, o fallos en la autenticación y autorización de usuarios. También es comúnmente utilizado para resolver errores en la integración continua o el despliegue automático.  |
|Delete  |Borrar  | Aplicado para la eliminación de clases, métodos o recursos que ya no son necesarios en el backend. Debe utilizarse cuando se elimina código obsoleto o módulos que han sido reemplazados por implementaciones más eficientes o actualizadas. |
|Drop  |Tirar  | Exclusivo para la eliminación de esquemas de bases de datos, tablas, o configuraciones en el backend. Debe ser utilizado con precaución, ya que este tipo de cambios puede tener implicaciones críticas en el almacenamiento de datos y la estructura general del sistema. Suele aplicarse cuando se reorganiza o limpia la base de datos en el proceso de migración o refactorización. |

Esta norma sigue los principios de Conventional Commits, una convención ligera para estructurar y nombrar los commits. Esta convención proporciona un conjunto claro de reglas para crear un historial de cambios detallado y coherente, lo que facilita la automatización de procesos como el versionado semántico y el seguimiento de características, correcciones y modificaciones críticas. Su implementación mejora la trazabilidad del desarrollo, simplifica las revisiones y asegura una mayor transparencia en el control de versiones. (GitHub & Netlify, 2024).

**Estructura del Mensaje de Commit:**

|type: description|
|-----------------|

**Versionado Semántico:**

Para las versiones de lanzamiento del proyecto, se aplicará el versionado semántico 2.0.0., siguiendo la estructura:

|Major.Minor.Patch|
|-----------------|

Donde:
- El dígito final (Patch) se utiliza para correcciones de errores que son compatibles con versiones anteriores.
- El segundo dígito (Minor) aumenta cuando se añaden nuevas funcionalidades que son compatibles con versiones anteriores.
- El primer dígito (Major) se incrementa para cambios importantes que podrían no ser compatibles con versiones anteriores.

### 4.1.3. Source Code Style Guide & Conventions.

En esta sección, nuestro equipo explicará y establecerá las referencias que adoptaremos para nombrar, estructurar, organizar y programar en los lenguajes de programación que se utilizarán en el desarrollo de nuestra solución de software, con un enfoque exclusivo en la implementación del Backend. Se detallarán las convenciones y mejores prácticas que se seguirán para asegurar un código coherente y eficiente en el uso de Java y SpringBoot, los principales lenguajes y herramientas del proyecto. Estas convenciones de codificación garantizarán la claridad, mantenibilidad y escalabilidad del código, facilitando la colaboración entre los diferentes miembros del equipo de desarrollo backend.

Asimismo, también investigaremos y presentaremos las directrices para la interacción con la base de datos MongoDB y su despliegue en MongoDB Atlas. Esto incluirá la gestión adecuada de las operaciones CRUD (Crear, Leer, Actualizar, Eliminar) y la optimización del rendimiento en las consultas y manejo de grandes volúmenes de datos:

- Guía de Estilo para SpringBoot: https://docs.spring.io/spring-boot/docs/current/reference/html/
- Panel de Guías variadas sobre SpringBoot: https://spring.io/guides
- Guía de Estilo para Java del AOSP para colaboradores: https://source.android.com/docs/setup/contribute/code-style?hl=es-419
- Manual Completo de Código en Java: https://www.manualweb.net/java/
- Modelo de Convenciones de codificación Java: https://codegym.cc/es/groups/posts/es.491.convenciones-de-codificacion-de-java-cuales-seguir-y-por-que
- Documentación oficial de MongoDB: https://www.mongodb.com/docs/manual/
- Documentación oficial de MongoDB Atlas: https://www.mongodb.com/docs/atlas/
- Guía oficial de conexiones, migraciones y herramientas de MongoDB: https://www.mongodb.com/docs/tools-and-connectors/ 

#### Convenciones que Usaremos:

**Java:**

- Convenciones de Nomenclatura: La claridad en la nomenclatura es fundamental para la mantenibilidad y legibilidad del código. En el desarrollo de un backend con Java y SpringBoot, las clases deben seguir la convención de CamelCase, comenzando cada palabra con mayúscula (UserController, OrderService, etc). Los métodos deben usar una convención de camelCase, comenzando con un verbo que indique la acción que realizan (getUserById(), processOrder(), etc). Las variables deben ser descriptivas y seguir un esquema en camelCase para reflejar claramente su propósito. Además, se recomienda organizar el código en paquetes coherentes, agrupando funcionalidades similares.
  
- Uso de Encapsulamiento: El encapsulamiento es uno de los pilares de la programación orientada a objetos en Java y debe ser aplicado rigurosamente en el backend. Cada clase debe tener sus atributos privados y se debe acceder a ellos a través de métodos públicos como `getters` y `setters`. Esto asegura que los datos no puedan ser modificados directamente desde fuera de la clase, evitando comportamientos inesperados. Además, contribuye a la modularidad del código, facilitando la refactorización sin romper otras partes del sistema.

- Control de Errores con Excepciones Personalizadas: En Java, el manejo adecuado de excepciones es crucial para asegurar la estabilidad del backend. Además de utilizar las excepciones estándar de Java, es recomendable definir excepciones personalizadas para representar errores específicos de la aplicación, como `UserNotFoundException` o `InvalidTransactionException`. Esto permite un control más granular sobre los errores y facilita la depuración. Asimismo, es importante asegurarse de no capturar excepciones de manera genérica con `catch(Exception e)` sin procesarlas adecuadamente. 

- Uso Eficiente de Recursos: En el desarrollo backend, el manejo adecuado de recursos como conexiones a bases de datos o archivos es crítico. Java ofrece una estructura de manejo automático de recursos, como el bloque `try-with-resources`, que debe ser utilizado para asegurar que los recursos se cierren correctamente después de su uso. Esto no solo mejora el rendimiento del sistema, sino que también previene fugas de memoria y otros problemas relacionados con la gestión inadecuada de recursos.

- Inmutabilidad de Objetos: Siempre que sea posible, los objetos en Java deben ser inmutables, lo que significa que su estado no puede cambiar después de su creación. Esto es particularmente útil en el backend para manejar datos que no deben ser modificados una vez inicializados, como claves de acceso o datos de configuración. Para crear objetos inmutables en Java, se pueden declarar todos los campos como final y no proveer métodos `setters`, asegurando que los objetos permanezcan constantes a lo largo de su ciclo de vida.

- Uso de Lombok para Reducir Código Repetitivo: Para evitar escribir código repetitivo, como `getters`, `setters` y constructores, el uso de bibliotecas como "Lombok" puede ser muy útil en Java. Con anotaciones como `@Data`, `@AllArgsConstructor` y `@NoArgsConstructor`, se reduce significativamente el tamaño del código, haciéndolo más limpio y fácil de mantener. Sin embargo, es importante usar "Lombok" de manera consciente, ya que puede ocultar parte de la lógica del código y es necesario asegurarse de que su uso no genere dependencias innecesarias.

- Aplicación del Principio de Responsabilidad Única: Cada clase y método en Java debe seguir el principio de responsabilidad única, lo que significa que cada uno debe tener una única razón para cambiar. Este principio asegura que el código esté organizado de manera modular, facilitando el mantenimiento y la extensión del sistema sin introducir complejidad adicional.

- Implementación de Interfaces para Desacoplamiento: Para lograr un backend flexible y desacoplado en Java, es una buena práctica definir interfaces que abstraigan las implementaciones de las clases concretas. De esta forma, si en el futuro es necesario cambiar la implementación de un servicio, solo será necesario modificar la clase que implementa la interfaz, sin alterar el resto del código. Este patrón es especialmente útil en la interacción con bases de datos y servicios externos, permitiendo la inyección de dependencias con facilidad.

- Uso de Generics para Tipado Fuerte: Los "Generics" en Java son una herramienta poderosa que permite crear clases y métodos que funcionen con cualquier tipo de dato, proporcionando mayor flexibilidad sin perder la seguridad del tipado fuerte. En un backend, los "generics" pueden utilizarse en clases de repositorio, listas, y otros contenedores de datos, garantizando que el código sea reutilizable y evite errores de tipo en tiempo de ejecución.

- Convenciones de Documentación con Javadoc: La documentación es esencial en el desarrollo de backend en Java, y la convención estándar es usar "Javadoc" para documentar las clases, métodos y atributos. Al proporcionar descripciones claras de lo que hace cada parte del código, se facilita la comprensión del sistema por parte de otros desarrolladores o futuros mantenedores del proyecto. Además, Javadoc permite generar automáticamente documentación en formato "HTML", lo que es muy útil para proyectos de gran envergadura.

**Spring Boot**:

- Configuración de Aplicación Externa: En un proyecto de Spring Boot, es fundamental externalizar la configuración de la aplicación en archivos como `application.properties` o `application.yml`. Esto permite que diferentes entornos (desarrollo, prueba, producción) tengan configuraciones específicas sin necesidad de modificar el código fuente. Utilizar variables de entorno para manejar información sensible, como credenciales de bases de datos, refuerza la seguridad y la flexibilidad del sistema. Además, la configuración de la conexión a la base de datos debe ser clara y debe incluir parámetros como el nombre de la base de datos, la dirección del servidor y las credenciales de acceso.

- Uso de Anotaciones de Spring: Aprovechar las poderosas anotaciones proporcionadas por Spring Boot es esencial para crear aplicaciones más limpias y mantenibles. Anotaciones como `@RestController`, `@Service`, `@Repository` y `@Component` deben ser utilizadas correctamente para definir la función de cada clase dentro de la aplicación. Esto no solo ayuda a la legibilidad del código, sino que también permite a Spring gestionar automáticamente la inyección de dependencias y la configuración de componentes, promoviendo una arquitectura más cohesiva y modular.

- Manejo de Errores con Controladores de Excepciones: La gestión adecuada de errores es crucial en aplicaciones de Spring Boot. Utilizar `@ControllerAdvice` para manejar excepciones de forma centralizada proporciona una forma limpia de capturar y gestionar errores a lo largo de toda la aplicación. Al definir un controlador de excepciones global, puedes personalizar las respuestas de error, asegurando que los clientes reciban mensajes claros y coherentes en caso de fallos. Esto mejora la experiencia del usuario y facilita el proceso de depuración.

- Configuración de Rutas de API REST: En el desarrollo de servicios REST con Spring Boot, es esencial estructurar las rutas de forma coherente y lógica. Usar convenciones de versión, como `/api/v1/`, permite gestionar los cambios en la API a lo largo del tiempo sin romper compatibilidad con versiones anteriores. Cada controlador debe tener su conjunto de rutas bien definidas y documentadas, utilizando las anotaciones `@GetMapping`, `@PostMapping`, `@PutMapping` y `@DeleteMapping` para mapear adecuadamente las solicitudes HTTP a los métodos correspondientes.

- Integración de Spring Data MongoDB: Al trabajar con MongoDB, es recomendable utilizar "Spring Data MongoDB", que simplifica la interacción con la base de datos. Definir repositorios extendiendo "MongoRepository" permite implementar operaciones CRUD de forma sencilla y declarativa, eliminando la necesidad de escribir consultas "boilerplate". Además, se deben aprovechar las características de Spring Data, como las consultas personalizadas y la paginación, para optimizar el acceso a datos y mejorar el rendimiento general de la aplicación.

- Pruebas Automatizadas con Spring Boot Test: La calidad del software es vital, y Spring Boot facilita la implementación de pruebas automatizadas. Utilizar el módulo "Spring Boot Test" permite realizar pruebas unitarias y de integración de manera efectiva. Es recomendable seguir el patrón de pruebas AAA (Arrange, Act, Assert) y utilizar herramientas como "JUnit" y "Mockito" para asegurar que cada componente de la aplicación funcione correctamente en diversas condiciones. Esto no solo aumenta la confianza en el código, sino que también facilita el mantenimiento y la evolución del sistema.

- Aspectos de Seguridad con Spring Security: La seguridad es un aspecto crítico en cualquier aplicación, y Spring Boot ofrece Spring Security para gestionar la autenticación y autorización. Implementar medidas de seguridad, como la autenticación basada en tokens (JWT), es esencial para proteger las rutas de la API y garantizar que solo los usuarios autorizados puedan acceder a recursos críticos. Asegúrate de configurar correctamente las reglas de seguridad y de aplicar la menor cantidad de privilegios necesarios para cada rol de usuario, minimizando así el riesgo de vulnerabilidades.

- Uso de Profiles para Configuraciones Específicas: Spring Boot permite definir diferentes perfiles para diferentes entornos de ejecución, como desarrollo, prueba y producción. Al utilizar la anotación `@Profile`, puedes activar o desactivar componentes específicos de la aplicación según el entorno. Esto facilita la personalización de la configuración, permitiendo que los equipos de desarrollo y operaciones gestionen mejor los entornos de producción sin comprometer la estabilidad del sistema.

- Documentación de la API con Swagger: La documentación clara de la API es fundamental para facilitar la colaboración entre desarrolladores y consumidores de la misma. Integrar "Swagger" en un proyecto de Spring Boot permite generar documentación interactiva y visual para la API de forma automática. Asegúrate de incluir descripciones detalladas de los endpoints, parámetros y respuestas esperadas para que los desarrolladores puedan comprender fácilmente cómo interactuar con la API.

- Configuración de la Persistencia de Datos: Para garantizar que los datos sean persistentes y se gestionen correctamente, es recomendable establecer un modelo claro de las entidades que se utilizarán en la aplicación. Al definir clases de entidad con la anotación `@Document` de "Spring Data MongoDB", asegúrate de que cada clase refleje la estructura de los documentos en la base de datos. Además, utilizar anotaciones como `@Id` para identificar la clave primaria y `@Field` para mapear los campos de manera explícita proporciona claridad y coherencia en la gestión de datos.

**MongoDB:**

- Diseño de Esquemas Flexibles: Uno de los principales beneficios de MongoDB es su naturaleza de esquema flexible, lo que permite que los documentos dentro de una colección tengan diferentes estructuras. Sin embargo, es importante definir un esquema básico para cada colección, estableciendo reglas claras sobre qué campos son obligatorios y cuáles son opcionales. Esto ayuda a mantener la integridad de los datos y facilita la validación a nivel de aplicación. 

- Uso de Identificadores Únicos: En MongoDB, cada documento tiene un identificador único `_id` que se genera automáticamente, generalmente como un "ObjectId". Es crucial aprovechar este campo como clave primaria para garantizar que cada documento sea identificable de manera única dentro de su colección. En situaciones en las que se requiere un identificador alternativo (como un número de teléfono o un correo electrónico), es recomendable crear índices únicos sobre esos campos para prevenir duplicados y asegurar la integridad de los datos.

- Modelado de Relaciones con Referencias o Embedding: Al modelar datos en MongoDB, es importante decidir cómo manejar las relaciones entre documentos. Existen dos enfoques principales: "referencias" y "embedding". Las referencias se utilizan para relacionar documentos de diferentes colecciones, mientras que el embedding permite almacenar documentos relacionados dentro de un documento padre. La elección entre estos métodos dependerá de la naturaleza de los datos y de cómo se accede a ellos. Generalmente, si los datos son utilizados juntos frecuentemente, el "embedding" puede ser más eficiente; por otro lado, si los datos son independientes y cambian con frecuencia, las "referencias" pueden ser preferibles.

- Indices para Optimizar Consultas: Para mejorar el rendimiento de las consultas en MongoDB, es vital crear índices adecuados en los campos que se utilizan con frecuencia en las búsquedas. Utilizar el comando `createIndex` para establecer índices sobre campos clave, así como índices compuestos para combinaciones de múltiples campos, puede reducir significativamente el tiempo de respuesta de las consultas. Sin embargo, es importante equilibrar la creación de índices con el costo de mantenimiento que estos suponen al realizar operaciones de escritura, ya que cada índice adicional puede afectar el rendimiento de las inserciones y actualizaciones.

- Consulta Eficiente con Proyecciones: Al recuperar documentos de una colección en MongoDB, es recomendable utilizar proyecciones para limitar los campos devueltos en una consulta. Esto no solo mejora la eficiencia al reducir la cantidad de datos transferidos, sino que también minimiza el uso de recursos del servidor. 

- Manejo Adecuado de Transacciones: Aunque MongoDB es conocido por su naturaleza de base de datos de documentos, las transacciones se han vuelto cada vez más importantes, especialmente en aplicaciones que requieren la consistencia de múltiples operaciones de escritura. Desde la versión 4.0, MongoDB admite transacciones ACID que abarcan múltiples documentos y colecciones. Es esencial utilizar estas transacciones adecuadamente para asegurar que un grupo de operaciones se ejecute completamente o no se ejecute en absoluto, manteniendo así la integridad de los datos.

- Implementación de Seguridad y Autenticación: La seguridad es un aspecto crítico en cualquier base de datos. En MongoDB, es importante habilitar la autenticación y la autorización, asegurando que solo los usuarios y aplicaciones autorizados puedan acceder a los datos. Configurar roles y permisos específicos a nivel de base de datos permite un control más granular sobre quién puede leer o escribir datos, lo que ayuda a mitigar el riesgo de accesos no autorizados y de violaciones de datos.

- Monitoreo y Rendimiento: Para mantener un rendimiento óptimo en MongoDB, es crucial implementar prácticas de monitoreo y ajuste. Utilizar herramientas como "MongoDB Atlas" o "MongoDB Ops Manager" permite a los desarrolladores y administradores de bases de datos supervisar el rendimiento, identificar problemas y optimizar las consultas. El monitoreo regular de métricas como la latencia de las consultas, el uso de la memoria y la carga del servidor ayuda a anticipar problemas y a implementar soluciones proactivas.

- Manejo de Datos No Estructurados: MongoDB es especialmente útil para almacenar datos no estructurados o semi-estructurados, como documentos JSON, imágenes o archivos. Utilizar la característica de "GridFS" de MongoDB permite almacenar y gestionar archivos grandes de manera eficiente. Sin embargo, es recomendable evaluar si se requiere almacenar datos directamente en la base de datos o si sería más apropiado almacenar rutas a archivos en un sistema de archivos externo, lo que puede mejorar el rendimiento y la escalabilidad.

- Estrategias de Backup y Recuperación: Implementar una estrategia sólida de respaldo y recuperación es esencial para proteger los datos en MongoDB. Utilizar las herramientas de respaldo integradas en MongoDB, así como prácticas recomendadas como el respaldo incremental y la replicación, asegura que los datos estén disponibles y sean recuperables en caso de fallos. Además, se deben realizar pruebas periódicas de los procedimientos de recuperación para asegurar que los respaldos sean efectivos y que la restauración de datos se realice de manera fluida y sin interrupciones en el servicio.

### 4.1.4. Software Deployment Configuration.

En esta sección, se detallará la configuración necesaria para implementar la solución, enfocándose exclusivamente en el despliegue del Backend del proyecto. El backend se desarrollará utilizando Java junto con el framework SpringBoot, lo que proporcionará una arquitectura robusta, escalable y fácil de mantener. Comenzaremos por crear un repositorio en GitHub destinado a almacenar todo el código relacionado con la lógica del servidor, controladores, servicios, y los modelos de datos que interactuarán con la base de datos MongoDB. 

Este repositorio permitirá a los desarrolladores gestionar de manera eficiente la colaboración y el control de versiones, asegurando que cada miembro del equipo trabaje en su propia rama "feature" para desarrollar nuevas funcionalidades del backend, tales como la autenticación de usuarios, el manejo de solicitudes, o la gestión de sesiones. Posteriormente, se llevará a cabo el proceso de merge con la rama principal "develop", lo que asegura que la lógica del backend esté siempre actualizada y optimizada con las últimas mejoras y correcciones.

## 4.2. Software Development & Implementation.

A continuación, se presenta una descripción detallada del enfoque técnico que adoptaremos para la implementación y despliegue de nuestra infraestructura backend en el proyecto de Roademics. Este enfoque se centra en la creación y gestión de servicios web, además de la integración con la base de datos y el manejo eficiente de las APIs necesarias para garantizar el correcto funcionamiento de la aplicación.

El proceso contempla varias etapas fundamentales. En primer lugar, se procederá al desarrollo de servicios backend escalables, diseñados para manejar un volumen creciente de solicitudes y datos, lo que asegurará la disponibilidad y el rendimiento óptimo de la aplicación en diferentes escenarios de carga. Además, se llevará a cabo una validación exhaustiva mediante pruebas unitarias y de integración. Estas pruebas son esenciales para identificar y corregir errores en fases tempranas del desarrollo, garantizando que cada componente funcione correctamente tanto de forma aislada como en conjunto.

Finalmente, antes de cada ciclo de despliegue en el entorno de producción, se implementarán estrategias de optimización del rendimiento. Esto incluirá la revisión y ajuste de consultas a la base de datos, la implementación de cachés y el análisis del tiempo de respuesta de las APIs. Este enfoque proactivo no solo mejorará la eficiencia del sistema, sino que también contribuirá a una experiencia de usuario fluida y satisfactoria.

**Despliegue de la arquitectura BackEnd de Roademics:**

Comenzaremos el proceso estableciendo un repositorio en GitHub, el cual funcionará como el repositorio central para todo el código y los recursos que componen nuestra aplicación de Backend, desarrollada en Java, con el framework de SpringBoot y organizada bajo Clean Architecture. Este repositorio servirá como base para gestionar la estructura del proyecto y contener los módulos esenciales de la aplicación, incluyendo el manejo de la API principal, la lógica de negocio establecida junto a los endpoints adecuados, y la integración con servicios externos como Firebase Authentication, Twilio y Stripe. Una vez que el repositorio esté configurado, cada desarrollador trabajará en su propia rama "feature" para implementar y mejorar funcionalidades específicas, permitiendo que cada contribución sea independiente y esté organizada. Una vez cada desarrollador termine su sección de feature, esas ramas serán eliminadas y se pasaran a las ramas principales.

Al completar el desarrollo de una funcionalidad, el siguiente paso será integrar el código en la rama "develop". Este proceso de fusión (merge) es fundamental, ya que asegura que la rama principal de desarrollo esté siempre actualizada con las implementaciones más recientes y con el trabajo colaborativo del equipo. Para garantizar una integración fluida, vamos a realizar revisiones de código a profundidad antes de realizar el merge. Estas revisiones y pruebas ayudarán a mantener la calidad del código y a detectar posibles conflictos o errores en una etapa temprana, evitando problemas en el entorno de producción.

Una vez que la rama "develop" esté lista y el código esté validado, configuraremos Railway para desplegar automáticamente nuestra aplicación de Servicios. Railway es una plataforma de infraestructura como servicio (IaaS) que facilita el despliegue, administración y escalabilidad de aplicaciones de backend, APIs y bases de datos. Esta plataforma facilitará el despliegue continuo al habilitar la actualización de la aplicación cada vez que se realice un merge en la rama "develop", permitiendo que la aplicación esté accesible de manera pública o en un entorno de pruebas, según las necesidades del proyecto. Esta configuración en Railway no solo optimiza el proceso de despliegue, sino que también proporciona un enlace que puede compartirse con los miembros del equipo y las partes interesadas, permitiendo una retroalimentación rápida y eficaz sobre el rendimiento y las funcionalidades del Backend.

A continuación, detallaremos los pasos necesarios para realizar este despliegue en Railway, con un enfoque en las mejores prácticas y consideraciones técnicas que asegurarán una implementación robusta y libre de contratiempos. Esta guía tiene como objetivo alinear al equipo y asegurar una implementación exitosa y eficiente de nuestra aplicación de Backend.

1. El primer paso para utilizar plenamente las funcionalidades de Railway es registrarse en su plataforma principal, lo que habilita el acceso a sus herramientas de despliegue continuo y administración de aplicaciones. Este registro puede realizarse de manera sencilla, pero se recomienda vincular la cuenta de Railway directamente con GitHub, ya que esto no solo facilita el acceso, sino que permite una integración continua con nuestros repositorios de código, como el de nuestro proyecto Roademics. De esta forma, Railway podrá monitorear y sincronizar automáticamente el branch "main" en GitHub, agilizando el proceso de despliegue sin necesidad de configuración manual en cada actualización. Una vez completado el registro y vinculadas ambas cuentas, iniciaremos sesión en Railway para acceder a nuestro panel de control, donde podremos gestionar el entorno de despliegue de Roademics. 

2. Después de completar los pasos de autenticación requeridos por Railway para acceder a la plataforma, seremos dirigidos a la página de inicio, donde encontraremos la sección principal para la creación de un nuevo proyecto mediante el panel de control. En esta sección, seleccionaremos la opción "Deploy from GitHub repository", que permite conectar directamente un repositorio de GitHub para configurar el despliegue de manera continua. Esta opción es ideal para proyectos como Roademics, ya que simplifica la integración con el repositorio y facilita la implementación automática de cambios realizados en la rama principal (main), asegurando que la aplicación esté siempre actualizada en el entorno de producción o pruebas, según corresponda.

3. Al haber vinculado nuestra cuenta de Railway con la de GitHub, la plataforma mostrará automáticamente todos los repositorios en los que tenemos permisos de administrador. Esto nos permitirá seleccionar el repositorio específico de Roademics para proceder con su despliegue. Railway detectará las ramas disponibles en el repositorio, como la rama principal (main) y cualquier otra rama de desarrollo que deseemos utilizar, ofreciendo así un control total sobre el entorno de despliegue y las versiones de código que se publicarán.

4. A continuación, se nos presentará una sección para la configuración de variables de entorno, las cuales son esenciales para el correcto funcionamiento de nuestra aplicación. En este caso, dado que estamos utilizando Java con Spring Boot, deberemos definir las variables que normalmente se encuentran en el archivo "application.properties" de nuestro proyecto. Estas variables pueden incluir credenciales de acceso a bases de datos, claves API de servicios externos, o configuraciones específicas del entorno de producción. Configurar correctamente estas variables en Railway garantiza que la aplicación se ejecute con los valores apropiados en cada despliegue, manteniendo la seguridad y permitiendo una adaptación flexible entre distintos entornos (desarrollo, pruebas, producción).

5. Una vez que hayamos definido todas las variables de entorno necesarias, procederemos a hacer clic en el botón "*Deploy Now*", lo cual iniciará el proceso de build y deploy de nuestra aplicación en Railway. Durante esta fase, Railway compilará el proyecto y gestionará la implementación, verificando que todas las configuraciones, dependencias y servicios externos estén correctamente conectados y configurados. Es importante monitorear el progreso en esta etapa para asegurarnos de que no haya errores en la compilación o despliegue, lo cual puede tardar unos minutos dependiendo de la complejidad del proyecto.

6. Para acceder a la interfaz gráfica de Swagger para nuestro backend, utilizaremos el dominio proporcionado por Railway y añadiremos la ruta "/swagger-ui/index.html#/" al final de la URL. Esto le indica a Swagger que queremos usar su interfaz para interactuar con los métodos HTTP de nuestra API, evitando hacer peticiones directas a los endpoints. Así, obtendremos una URL similar a la siguiente:
  
   "https://wehaveidea-production.up.railway.app/swagger-ui/index.html#/"

   Este enlace nos permitirá visualizar y probar todos los endpoints de nuestra API en un entorno controlado, facilitando la documentación y verificación de los servicios expuestos por el backend.

   Como podemos observar, nuestro backend ha sido desplegado exitosamente y está listo para ser utilizado. La plataforma de Railway confirma que el proceso de build y deploy se ha completado sin errores, permitiéndonos ahora acceder a todos los servicios y funcionalidades de la API. Esto nos asegura que la aplicación está disponible en el entorno de producción y lista para recibir solicitudes y responder a los endpoints configurados, cumpliendo así con los requerimientos del proyecto y facilitando el acceso a los desarrolladores y usuarios autorizados.

7. Como podemos observar, nuestro backend ha sido desplegado exitosamente y está listo para ser utilizado. La plataforma de Railway confirma que el proceso de build y deploy se ha completado sin errores, permitiéndonos ahora acceder a todos los servicios y funcionalidades de la API. Esto nos asegura que la aplicación está disponible en el entorno de producción y lista para recibir solicitudes y responder a los endpoints configurados, cumpliendo así con los requerimientos del proyecto y facilitando el acceso a los desarrolladores y usuarios autorizados.

8. Al probar nuestro enlace en Postman para contactar un endpoint específico, recibimos un response con el código de estado 200, lo que indica que la solicitud fue procesada exitosamente.

### 4.2.1. Sprint 1

En esta sección, se registrará y explicará el avance en términos de producto y trabajo colaborativo correspondiente al Sprint número 1 de la Implementación del Backend. Este registro detallado documentará cada aspecto del progreso logrado, incluyendo el desarrollo, el historial de cambios, y el avance colectivo aportado por cada integrante del equipo de trabajo sobre el propio Backend y sus Endpoints. Se hará hincapié en la importancia de la colaboración y la comunicación efectiva entre los miembros del equipo para alcanzar los objetivos del sprint.

Todas las especificaciones y resultados presentados en esta sección se derivan del Product Backlog establecido en el Capítulo 2, en la sección de requerimientos. Este alineamiento garantiza que los desarrollos realizados durante el sprint sean consistentes con las expectativas del proyecto y contribuyan a la visión general del producto.

#### 4.2.2.1 Sprint Planning 1.

En esta sección se explicarán los detalles presentados y analizados durante la reunión del Sprint Planning para el Sprint número 1 de la implementación del Backend. El objetivo principal de esta reunión es establecer un plan claro y realista que guíe el desarrollo del backend, identificando las tareas específicas a realizar y comprometiéndose con un conjunto de entregables concretos que contribuyan al avance del proyecto. Este enfoque permite asegurar que todos los miembros del equipo tengan una comprensión compartida de los objetivos y las expectativas del sprint, lo que resulta esencial para la coordinación y efectividad en el trabajo colaborativo.

###### Tabla 23
*Tabla del planeamiento a profundidad del Sprint 1*
<table>
        <tr>
            <td colspan="1">Sprint #</td>
            <td colspan="1">Sprint 1</td>
        </tr>
        <tr>
            <td colspan="2">Sprint Planning Background</td>
        </tr>
        <tr>
            <td>Date</td>
            <td>2024-09-01</td>
        </tr>
          <tr>
            <td>Time</td>
            <td>18:01</td>
        </tr>
            <tr>
            <td>Location</td>
            <td>Discord</td>
        </tr>
            <tr>
            <td>Prepared by</td>
            <td>Yen Cerna, Lucio Heli</td>
        </tr>
            <tr>
            <td>Attendees (to planning meeting)</td>
            <td>Pescorán Angulo, Juan Fabritzzio; Trigueros Chumacero, Flavio Eduardo; Valenzuela Huillcaya, Aldhair Johan Juan; Yen Cerna, Lucio Heli</td>
        </tr>
            <tr>
            <td>Sprint 1 Review Summary</td>
            <td>Al concluir el Sprint 1, se llevó a cabo la reunión de Sprint Review en la que se evaluó el progreso realizado en el desarrollo del Backend de nuestra aplicación. Durante este sprint, el enfoque principal se centró en la creación de los Endpoints para el proceso de autenticación y autorización (IAM), así como en la implementación de la funcionalidad de Roadmaps. <br><br> La reunión fue exitosa en términos de avance en los productos de software y en la colaboración del equipo. Tras realizar un análisis exhaustivo de los objetivos establecidos y recopilar valiosa retroalimentación, se identificaron áreas de mejora que contribuyeron significativamente a la calidad del desarrollo. La integración de las recomendaciones recibidas permitió optimizar varios aspectos del código y mejorar la eficiencia de los nuevos Endpoints, lo que a su vez facilitó una experiencia de usuario más fluida y segura. </td> 
        </tr>
            <tr>
            <td>Sprint 1 Retrospective Summary</td>
            <td>En el proceso de Sprint Retrospective para el Sprint 1, nuestro equipo se dedicó a revisar detenidamente toda la retroalimentación recibida tras la finalización del primer sprint. Este análisis exhaustivo del desempeño general e individual de cada miembro del equipo nos permitió identificar áreas clave de mejora que son fundamentales para optimizar nuestra aplicación móvil. <br><br> A través de este proceso reflexivo, se plantearon varias estrategias para garantizar la entrega de un trabajo de mayor calidad y un producto que cumpla con las expectativas de nuestros clientes. <br><br> Para este sprint en particular, hemos acordado implementar mejoras en la esquematización de los reportes, junto con la creación de diagramas que faciliten la comprensión y el seguimiento del progreso del desarrollo. Además, se propone una revisión integral del diseño del Backend, buscando optimizar su rendimiento y escalabilidad para garantizar una experiencia de usuario fluida en la aplicación móvil.</td>
        </tr>
            <tr>
            <td colspan="2">Sprint Goal & User Stories</td>
        </tr>
              <tr>
            <td>Sprint 1 Goal</td>
            <td>Alcanzar una métrica de cumplimiento del 100%, lo que indicará que se ha logrado todos los objetivos del sprint 1 con todas las historias de usuario y otros materiales necesarios.</td>
        </tr>
              <tr>
            <td>Sprint 1 Velocity</td>
            <td>Con el equipo para este sprint 1 decidimos aceptar 5 Story Points</td>
        </tr>
              <tr>
            <td>Sum of Story Points</td>
            <td>La suma de los Story Points para los User Stories que se están incluyendo en este Sprint 1 es XX</td>
        </tr>
    </table>

#### 4.2.2.2 Sprint Backlog 1.

En esta sección se revisará todo el proceso relacionado con el Sprint Backlog número 1, en el cual nuestro equipo de trabajo se centró principalmente en el diseño del Backend y en la preparación de ciertas características correspondientes a la lógica de negocio y a los modelos de datos que interactúan con la base de datos mediante el uso de Endpoints documentados. Este enfoque abarcó la definición de las rutas de la API, la implementación de controladores, y la creación de servicios que soportan las funcionalidades requeridas por el sistema.

Además, se abordaron los modelos de datos que estructuran la información en la base de datos MongoDB, asegurando que cada componente del backend esté alineado con los requisitos funcionales y no funcionales establecidos en la fase de planificación. También se discutieron las interacciones necesarias entre los distintos módulos del backend y la integración con MongoDB Atlas para garantizar un rendimiento óptimo y una alta disponibilidad de los datos. Este proceso de diseño y preparación fue crucial para sentar las bases del desarrollo efectivo en los siguientes sprints, asegurando que cada elemento del backend esté bien definido y listo para su implementación.

###### Tabla 59
*Tabla principal del planeamiento del Sprint Backlog 1*
<table>
        <tr>
            <td colspan="2">Sprint #</td>
            <td colspan="6">Sprint 1</td>
        </tr>
        <tr>
            <td colspan="2">User Story</td>
            <td colspan="6">Work-Item / Task</td>
        </tr>
        <tr>
            <td>Id</td>
            <td>Title</td>
            <td>Id</td>
            <td>Title</td>
            <td>Descripcion</td>
            <td>Estimation (Hours)</td>
            <td>Assigned To</td>
            <td>Status (To-do / In / Process / ToReview / Done)</td>
        </tr>
        <tr>
            <td>US21</td>
            <td>Creación de roadmap académico básico</td>
            <td>T01</td>
            <td>Creación de roadmap básico</td>
            <td>Como usuario interesado en planificar su trayectoria profesional, quiero crear un roadmap académico básico en la plataforma,para visualizar y gestionar mi progreso académico y planificar mis cursos y metas profesionales.</td>
            <td>3 horas</td>
            <td>Pescoran Angulo, Juan Fabrizzio</td>
            <td>Done</td>
        </tr>
                <tr>
            <td>US24</td>
            <td>Edición de roadmap académico básico</td>
            <td>T02</td>
            <td>Edición de roadmap básico</td>
            <td>Como usuario que ha creado un roadmap básico, quiero poder editar el roadmap, para actualizar la información, ajustar mis objetivos y modificar mis planes según mis necesidades.</td>
            <td>4 horas</td>
            <td>Pescoran Angulo, Juan Fabrizzio</td>
            <td>Done</td>
        </tr>
                <tr>
            <td>US25</td>
            <td>Acceso a herramienta de edición avanzada para usuarios Premium</td>
            <td>T03</td>
            <td>Acceso a herramientas de edición avanzada</td>
            <td>Como usuario Premium, quiero tener acceso a una herramienta de edición avanzada, para aprovechar funcionalidades adicionales y más detalladas al modificar mis roadmaps profesionales, optimizando mi planificación y gestión de objetivos.</td>
            <td>2 horas</td>
            <td>Pescoran Angulo, Juan Fabrizzio</td>
            <td>Done</td>
        </tr>
                <tr>
            <td>US26</td>
            <td>Eliminación de roadmaps que no se requieren</td>
            <td>T04</td>
            <td>Eliminación de roadmaps que no se requieren</td>
            <td>Como usuario registrado, quiero poder eliminar roadmaps que ya no necesito, para mantener mi perfil organizado y libre de información obsoleta o innecesaria.</td>
            <td>3 horas</td>
            <td>Pescoran Angulo, Juan Fabrizzio</td>
            <td>Done</td>
        </tr>
                <tr>
            <td>US27</td>
            <td>Visualizar limitaciones respecto a la cantidad de roadmaps que el usuario podrá gestionar</td>
            <td>T05</td>
            <td>Visualizar limitaciones respecto a la cantidad de roadmaps</td>
            <td>Como usuario registrado, quiero visualizar las limitaciones respecto a la cantidad de roadmaps que puedo gestionar, para asegurarme de no gastar espacio.</td>
            <td>4 horas</td>
            <td>Pescoran Angulo, Juan Fabrizzio</td>
            <td>Done</td>
        </tr>
                <tr>
            <td>US28</td>
            <td>Creación de roadmaps personalizados ilimitados y compartirlos con los demás usuarios de la aplicación</td>
            <td>T06</td>
            <td>Creación de roadmaps y compartirlos con los demás usuarios de la aplicación</td>
            <td>Como usuario interesado en planificar su trayectoria profesional, quiero crear un roadmap académico básico en la plataforma,para visualizar y gestionar mi progreso académico y planificar mis cursos y metas profesionales.</td>
            <td>4 horas</td>
            <td>Pescoran Angulo, Juan Fabrizzio</td>
            <td>Done</td>
        </tr>
                </tr>
                <tr>
            <td>US29</td>
            <td>Recibir análisis avanzados sobre mi propio roadmap</td>
            <td>T07</td>
            <td>Recibir análisis avanzados sobre mi propio roadmap</td>
            <td>Como usuario Premium, quiero recibir análisis avanzados sobre mi propio roadmap, para obtener información detallada y perspicaz que me ayude a optimizar mi planificación y alcanzar mis objetivos profesionales más eficientemente..</td>
            <td>4 horas</td>
            <td>Pescoran Angulo, Juan Fabrizzio</td>
            <td>Done</td>
        </tr>
                </tr>
    </table>

Con el fin de que la lista de tareas en el sprint pueda ser visualizada a más profundidad, se mostrara un enlace directo a la sección de trabajo designada por el equipo junto a todas las actividades planificadas de forma completa: 

###### Figura 58
*Presentación de la tabla de actividades designada para el Sprint 1 en ClickUp.*
<img src="/assets/img/Lista de Tareas-Sprint2.png" alt="Lista de Tareas del Sprint 1 En ClickUp">

#### 5.2.2.3 Development Evidence for Sprint Review.

En esta sección se explica y presenta los avances en implementación con relación a los productos de la solución según el alcance del Sprint: Web Application. Aquí se dejara cada uno de los commits ya implementados dentro del repositorio de Github, junto a toda la información referente y a los cambios concluidos.

###### Tabla XX
*Tabla de los commits realizados y relacionados con el desarrollo de todas las secciones del Sprint Backlog 1*
| Repository | Branch| Commit Id| Commit Message| Commit Message Body|Commited on (Date) |
|------------|-------|----------|---------------|--------------------|-------------------|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|2085a4451325f1d0668047d8cb6b2ea986d11b59|Initial commit| 15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|97844950e2f718610501441269a798e12a09335e|feat(pom)|added dependencies and pluggins to work with|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|e0bff2d2c61620faebff1677756d311003cf2710|feat(shared) | added aggregate and entity for model in shared|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|e0bff2d2c61620faebff1677756d311003cf2710|feat(shared) | added openapi documentation|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|2b25ddce453a9cc5607d5d84605a366aafc60f3d|feat(shared) | added messageresource to handling errors|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|c61c607c468d92badf5782a17f68a146de5b3156|feat(shared) | added mongodb connection string with environment variables|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|529d6cd57e62dd85b5e7481673baf93753637540|feat(shared) | added getter annotation for auditable root|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|a2c7bcfef24588dff3c58e7e12e7e8c18678e05b|feat(iam) | add queries and commands for domain model|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|eef09f53e6a0def5c69d68eeecc7d946c8dc6046|feat(iam) | add aggregate, entity and value object|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|563a45cf85acf62a3b6188c9825aa44e623c048c|feat(iam) | add services into domain model for role and user|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|d4b16c16c6187ea0b631c6e9ebfd34418573639d|feat(iam) | add aggregate and entity into domain model|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|01ef289b8e06c608437e83fe9f784942133aab16|feat(iam) | add repositories into infrastructure using spring data mongodb|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|b772481b7f9265fa7cdd7755547df926a8d0c3c9|feat | add configurations to run application|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|dad58f32480d06eb505510c553488c63dfdf575a|feat(iam) | add endpoints for roles, users and iam|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|eaad313305eea6cc6ad968962a9c12220f68640d|feat(iam) | add resources and transform into interfaces directory to work with endpoints|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|06e2d6ad69877a6a17ccc4d3b407fb4433647cbe|fix(shared) | changed id from string to long|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|c461a5a847ab8e04a064edc5eb6afc50dafd3ae2|fix(iam) | fix variable type for these files|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|ff2fb2a6c541ffb7572bf0e47de580ab81655e08|feat(iam) | add implementation for services|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|8439db4b61723bda9a4d78319cad58f62188022e|feat(iam) | add security measures for tokens, login, etc|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|a0960fb7e3c2852f56e96310e284f263c1a43b15|feat(iam) | add services for tokens, hashing, etc|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|43b1bbbef36b5347980e1a24189be88b57055619|feat(iam) | add facade to interact with other bounded contexts|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|446d39aec1d5012e434eb6ee0dbf0ce20617c19c|refactor(pom) | add management dependencies|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|52bedcd93b6974510c1c8eea0e45e74194b13a70|refactor(pom) | refactored pom.xml|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|aa04417c3937ea4646487613b11352f9f2e9460d|refactor(pom) | refactored application.properties|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|f360d9db097b676f756a7c783673acad7bb8b6d7|feat(pom) | add dependencies to pom for openai service and apache http components|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|5138178d855314fc986d7527266533a8a93c56ea|feat(roadmap) | add command and queries for domain model|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|6ab57299e68457af7250c3cf33c2d08dbd7085fc|feat(roadmap) | add outbound service in application layer|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|eaa28f963e1abc9f32012ce68d32ce9d5469038f|feat(roadmap) | add entities, value objects and aggregates for domain layer|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|131c8525f8e9ded47671249807295f7961f76e2c|feat(roadmap) | add service interfaces for roadmap aggregate and both, ai interaction and ai recommendations|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|e33627bc8c10b32d81bbb8b2eab5cb07344e59da|feat(roadmap) | add service implementation for roadmap aggregate and both, ai interaction and ai recommendations|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|90d29b3a2d8224de3d92f3fad82b9ba3e1d49cdd|feat(roadmap) | add repository for roadmap aggregate and ai recommendations|15/09/24|

#### 5.2.2.4 Testing Suite Evidence for Sprint Review. 

En esta sección presentaremos la evidencia detallada de las pruebas rigurosas realizadas durante el sprint. Para garantizar la calidad y funcionalidad del producto, hemos empleado la metodología Gherkin para definir escenarios de prueba claros y concisos. Cada uno de estos escenarios se ha registrado meticulosamente en commits específicos en nuestro repositorio de código, lo que proporciona un registro completo y transparente de nuestro proceso de prueba.

###### Tabla 26
*Tabla de los modelos de pruebas realizados y relacionados con el desarrollo de todas las secciones del Sprint Backlog 2*
| Repository                        | Branch              | Commit Id                          | Commit Message                   | Commit Message Body           |Commited on (Date) |
|-----------------------------------|---------------------|------------------------------------|----------------------------------|-------------------------------|-------------------|
| upc-pre-202401--si730-WS52-SmarTech-AcceptanceTests | feat(.features): added More User Stories - Ruben - 1 | ff860b5 | feat(.features): added More User Stories | En esta sección se implementaron todos los Acceptance Test para el Sprint 2 de Propertunity | 30/04/24 |

#### 5.2.2.5 Execution Evidence for Sprint Review. 

#### 5.2.2.6 Services Documentation Evidence for Sprint Review. 

En esta sección, presentamos la relación de Endpoints documentados con OpenAPI, que están directamente vinculados con el alcance del Sprint. Iniciamos con una breve introducción que resume los logros alcanzados en relación con la Documentación de Web Services durante este período de desarrollo. A continuación, proporcionamos una tabla detallada que enumera cada Endpoint, junto con las acciones implementadas y los enlaces correspondientes a la documentación desplegada o la URL local en Sprints anteriores al despliegue de Web Services.

El siguiente enlace proporcionará acceso al modelo de DBJson utilizado como una representación simulada de API antes de la integración y construcción de una API completa y final para Propertunity. Este enlace está ubicado dentro de nuestra plataforma FrontEnd y sirve como punto de referencia crucial durante el proceso de desarrollo y prueba.

Al hacer clic en este enlace, los desarrolladores y miembros del equipo pueden acceder al modelo de datos completo en formato JSON, que representa de manera precisa la estructura y la organización de los datos utilizados en nuestra aplicación. Este modelo de DBJson sirve como un punto de partida fundamental para comprender la lógica subyacente de nuestra aplicación y cómo interactúa con la base de datos: https://github.com/SmarTech-Propertunity/upc-pre-202401--si730-WS52-SmarTech-FrontEnd/blob/main/server/db.json

En la tabla, se indican las acciones soportadas para cada Endpoint, incluyendo el verbo HTTP (GET, POST, PUT, DELETE, PATCH), la sintaxis de llamada, la especificación de posibles parámetros y se incluye un ejemplo junto con una explicación del response correspondiente. Además de la tabla, se presentan capturas de pantalla que ilustran la interacción con la documentación elaborada, utilizando datos de muestra para demostrar cómo se utiliza cada Endpoint. En este caso, vamos a dar una explicación completa de 3 clases con respecto a todo el modelo del DBJson para poder dar una idea completa y, a la vez, no abrumar al lector con grandes cúmulos de información base en un modelo CRUD:

###### Tabla 27
*Tabla del modelo de escritura para el Bounded Context de IAM*
| Método  | Descripción                                  | Ejemplo de llamada         | Parámetros                                     | Respuesta                                                                                 |
|---------|----------------------------------------------|----------------------------|------------------------------------------------|-------------------------------------------------------------------------------------------|
| GET     | Obtener todos los usuarios                   | GET /usuarios               | Ninguno                                        | Lista de usuarios en formato JSON con detalles como nombre, correo, fecha de registro, etc.|
| POST    | Crear un nuevo usuario                       | POST /usuarios              | `username`, `email`, `password`                | Detalles del nuevo usuario creado en formato JSON, incluyendo ID y fecha de creación.      |
| PUT     | Actualizar la información de un usuario      | PUT /usuarios/{id}          | `username`, `email`, `password`                | Usuario actualizado con los nuevos datos proporcionados.                                  |
| DELETE  | Eliminar un usuario                          | DELETE /usuarios/{id}       | `id` del usuario                               | Mensaje de confirmación de eliminación del usuario.                                        |
| GET     | Obtener detalles de un usuario específico    | GET /usuarios/{id}          | `id` del usuario                               | Detalles del usuario solicitado, incluyendo roles, fecha de registro, y demás datos.       |
| POST    | Autenticación de usuario                     | POST /usuarios/authenticate | `username`, `password`                         | Token JWT válido para autenticar las siguientes peticiones del usuario.                    |
| POST    | Actualizar la contraseña de un usuario       | POST /usuarios/{id}/password| `id`, `newPassword`, `oldPassword`             | Confirmación de la actualización de la contraseña.                                         |


###### Tabla 28
Tabla del modelo de escritura para el Bounded Context de Roadmaps:
| Método  | Descripción                                            | Ejemplo de llamada               | Parámetros                                                      | Respuesta                                                                                 |
|---------|--------------------------------------------------------|----------------------------------|-----------------------------------------------------------------|-------------------------------------------------------------------------------------------|
| GET     | Obtener todos los roadmaps disponibles                 | GET /roadmaps                    | Ninguno                                                         | Lista de roadmaps en formato JSON con detalles como título, descripción, nodos, edges, etc.|
| POST    | Crear un nuevo roadmap                                 | POST /roadmaps                   | `title`, `description`, `nodes[]`, `edges[]`                    | Detalles del nuevo roadmap creado, incluyendo ID y fecha de creación.                     |
| PUT     | Modificar un roadmap existente                         | PUT /roadmaps/{id}               | `title`, `description`, `nodes[]`, `edges[]`                    | Roadmap actualizado con la nueva información proporcionada.                               |
| DELETE  | Eliminar un roadmap                                    | DELETE /roadmaps/{id}            | `id` del roadmap                                                | Mensaje de confirmación de eliminación del roadmap.                                        |
| GET     | Obtener detalles de un roadmap específico              | GET /roadmaps/{id}               | `id` del roadmap                                                | Detalles del roadmap solicitado, con nodos y edges.                                       |
| POST    | Generar recomendaciones mediante IA para un roadmap    | POST /roadmaps/{id}/recommendations | `id`, `userPrompt`, `aiToken`                                   | Respuesta de la IA con sugerencias personalizadas para el roadmap.                        |
| GET     | Obtener todas las interacciones con IA relacionadas    | GET /roadmaps/{id}/ai-interactions | `id` del roadmap                                                | Lista de interacciones y respuestas de la IA relacionadas con el roadmap.                 |
| POST    | Finalizar el roadmap                                   | POST /roadmaps/{id}/finish       | `id`, `feedback`                                                | Confirmación de finalización del roadmap y detalles de la retroalimentación proporcionada. |

#### 5.2.2.7 Software Deployment Evidence for Sprint Review.

Dentro del Sprint 1, no se realizo ningún despliegue.

#### 5.2.2.8 Team Collaboration Insights during Sprint.

Durante el Sprint 1 de la sección Software Development & Implementation, nos enfocamos en el desarrollo colaborativo del propio BackEnd de la aplicación móvil de Roademics, donde cada miembro del equipo contribuyó con sus habilidades y conocimientos. Esta colaboración se refleja en los numerosos commits realizados en nuestro repositorio de código, los cuales están respaldados por capturas de pantalla adjuntas para una documentación detallada.

Nuestro equipo se reunió tanto en persona como virtualmente para asignar tareas y discutir la estrategia de desarrollo del proyecto. Estas reuniones fueron cruciales para clarificar nuestras responsabilidades individuales y asegurar un desempeño óptimo. Para maximizar la eficiencia, decidimos asignar a cada miembro del equipo una sección específica del BackEnd para desarrollar, lo que nos permitió avanzar rápidamente y cumplir con los plazos establecidos.

Además, programamos sesiones regulares de brainstorming y resolución de problemas, donde compartimos ideas y abordamos cualquier duda o dificultad que surgiera durante el proceso de desarrollo. Estas reuniones fueron fundamentales para resolver obstáculos de manera efectiva y garantizar un progreso constante en la elaboración del FrontEnd del Web Application.

###### Figura 88
*Reporte completo de contribuciones para el desarrollo del BackEnd de la Aplicación Móvil de Roademics durante el Sprint 1 de Software Development & Implementation.*

<img src="/assets/img/Pulse-backend-for-main-sprint1.png" alt="Pulse for the Main Branch in Software Development and Implementation">
<img src="/assets/img/Contributions-backend-for-main-sprint1.png" alt=Contributions for the Main Branch in Software Development and Implementation ">
<img src="/assets/img/Individual-contributions-for-main-sprint1.png" alt="Individual Contributions for the Main Branch in Software Development and Implementation">

---

### 4.2.2. Sprint 2

En esta sección, se registrará y explicará el avance en términos de producto y trabajo colaborativo correspondiente al Sprint número 2 de la Implementación del Backend. Este registro detallado documentará cada aspecto del progreso logrado, incluyendo el desarrollo, el historial de cambios, y el avance colectivo aportado por cada integrante del equipo de trabajo sobre el propio Backend y sus Endpoints. Se hará hincapié en la importancia de la colaboración y la comunicación efectiva entre los miembros del equipo para alcanzar los objetivos del sprint.

Todas las especificaciones y resultados presentados en esta sección se derivan del Product Backlog establecido en el Capítulo 2, en la sección de requerimientos. Este alineamiento garantiza que los desarrollos realizados durante el sprint sean consistentes con las expectativas del proyecto y contribuyan a la visión general del producto.

#### 4.2.2.2 Sprint Planning 2.

En esta sección se explicaran los detalles presentados y analizados durante la reunión del Sprint Planning para el número 2. El objetivo principal de esta reunión es establecer un plan claro y realista para el sprint, identificando las tareas a realizar y comprometiéndose con un conjunto de entregables concretos que contribuyan al avance del proyecto. A continuación, se presenta el resumen del Sprint Planning Meeting, que proporcionará una visión general de los temas discutidos y las decisiones tomadas durante la reunión.

###### Tabla XX
*Tabla del planeamiento a profundidad del Sprint 2.*
<table>
        <tr>
            <td colspan="1">Sprint #</td>
            <td colspan="1">Sprint 2</td>
        </tr>
        <tr>
            <td colspan="2">Sprint Planning Background</td>
        </tr>
        <tr>
            <td>Date</td>
            <td>2024-09-18</td>
        </tr>
          <tr>
            <td>Time</td>
            <td>18:27</td>
        </tr>
            <tr>
            <td>Location</td>
            <td>Discord</td>
        </tr>
            <tr>
            <td>Prepared by</td>
            <td>Yen Cerna, Lucio Heli</td>
        </tr>
            <tr>
            <td>Attendees (to planning meeting)</td>
            <td>Pescorán Angulo, Juan Fabritzzio; Trigueros Chumacero, Flavio Eduardo; Valenzuela Huillcaya, Aldhair Johan Juan; Yen Cerna, Lucio Heli</td>
        </tr>
            <tr>
            <td>Sprint 2 - 2 Review Summary</td>
            <td>Después de un realizar todos los procedimientos establecidos para la identificación de objetivos y áreas de retroalimentación, hemos podido concluir la reunión del sprint 1 con éxito en términos de avance en los productos de software y en la colaboración general del equipo. El proceso de mejora con la retroalimentación y la programación de varias secciones nuevas en la Aplicación Web significó un gran proceso de mejora para la construcción y realización del sprint, además de reforzar el compromiso de nuestro equipo y la mejora exponencial de las actividades indicadas.</td> 
        </tr>
            <tr>
            <td>Sprint 2 – 2 Retrospective Summary</td>
            <td>Para el proceso de la retrospectiva del Sprint 1, fue necesario que nuestro equipo revisara a detalle toda la retroalimentación recibida ante el primer sprint realizado, para luego generar un análisis a profundidad del desempeño general e individual de todos los miembros del equipo de trabjo. Después de ese proceso, pudimos identificar varias áreas de mejora en las cuales centrarnos para así poder garantizar la entrega de un mejor trabajo y un buen producto para todos nuestros clientes, promoviendo la mejora continua y optimizando los métodos de trabajo en los próximos sprints durante el ciclo de vida del proyecto. Para el caso de este sprint, hemos planteado la mejora en la esquematización del reporte junto a sus diagramas, además de una mejora general en todo el diseño del BackEnd.</td>
        </tr>
            <tr>
            <td colspan="2">Sprint Goal & User Stories</td>
        </tr>
              <tr>
            <td>Sprint 1 Goal</td>
            <td>Alcanzar una métrica de cumplimiento del 100%, lo que indicará que se ha logrado todos los objetivos del sprint 1 con todas las historias de usuario y otros materiales necesarios.</td>
        </tr>
              <tr>
            <td>Sprint 2 Velocity</td>
            <td>Con el equipo para este sprint 1 decidimos aceptar 5 Story Points</td>
        </tr>
              <tr>
            <td>Sum of Story Points</td>
            <td>La suma de los Story Points para los User Stories que se están incluyendo en este Sprint 1 es XX</td>
        </tr>
    </table>

#### 4.2.2.2 Sprint Backlog 2.

En esta sección se revisara todo el proceso dado para el Sprint Backlog número 1, en el cual nuestro equipo de trabajo se centró principalmente en el diseño de , junto a la preparación de ciertas caracteristicas correspondientes a la interfaz y a los modelos de navegación y componentes. 

###### Tabla 59
*Tabla principal del planeamiento del Sprint Backlog 1*
<table>
        <tr>
            <td colspan="2">Sprint #</td>
            <td colspan="6">Sprint 1</td>
        </tr>
        <tr>
            <td colspan="2">User Story</td>
            <td colspan="6">Work-Item / Task</td>
        </tr>
        <tr>
            <td>Id</td>
            <td>Title</td>
            <td>Id</td>
            <td>Title</td>
            <td>Descripcion</td>
            <td>Estimation (Hours)</td>
            <td>Assigned To</td>
            <td>Status (To-do / In / Process / ToReview / Done)</td>
        </tr>
        <tr>
            <td>TS001</td>
            <td>Integrar un sistema de registro con Firebase Authentication</td>
            <td>T08</td>
            <td>Integración de un sistema de registro con Firebase Authentication</td>
            <td><strong>Como</strong> desarrollador de Roademics <strong>quiero</strong> integrar un sistema de registro utilizando Firebase Authentication, <strong>para</strong> garantizar un proceso de autenticación seguro para los usuarios.</td>
            <td>1 hora</td>
            <td>Trigueros Chumacero, Flavio Eduardo</td>
            <td>Done</td>
        </tr>
                <tr>
            <td>TS002</td>
            <td>Implementación de validaciones de credenciales</td>
            <td>T09</td>
            <td>Implementación de validaciones de las credenciales de usuario</td>
            <td><strong>Como</strong> desarrollador de la plataforma, <strong>quiero</strong> implementar validaciones de credenciales durante el proceso de registro <strong>para</strong> asegurar que los usuarios ingresen información válida.</td>
            <td>3 horas</td>
            <td>Pescoran Angulo, Juan Fabrizzio</td>
            <td>Done</td>
        </tr>
                <tr>
            <td>TS003</td>
            <td>Encriptación de datos del usuario cuando estén tanto en tránsito como en reposo</td>
            <td>T10</td>
            <td>Encriptación de los datos de usuarios cuando estén presentes en tránsito o en reposo</td>
            <td><strong>Como</strong> desarrollador de la plataforma, <strong>quiero</strong> encriptar los datos del usuario tanto cuando estén en tránsito como en reposo, <strong>para</strong> garantizar la seguridad y privacidad de la información.</td>
            <td>2 horas</td>
            <td>Pescoran Angulo, Juan Fabrizzio</td>
            <td>Done</td>
        </tr>
                <tr>
            <td>TS004</td>
            <td>Integración de sistema de autenticación con Firebase Authentication</td>
            <td>T11</td>
            <td>Integración de sistemas de autenticación con la API Firebase Authentication</td>
            <td><strong>Como</strong> desarrollador de la plataforma, <strong>quiero</strong> integrar Firebase Authentication para el proceso de inicio de sesión, <strong>para</strong> asegurar que los usuarios puedan autenticarse de manera segura y rápida utilizando los servicios de Firebase.</td>
            <td>1 hora</td>
            <td>Trigueros Chumacero, Flavio Eduardo</td>
            <td>Done</td>
        </tr>
                <tr>
            <td>TS005</td>
            <td>Implementar un sistema de autenticación segura en el backend</td>
            <td>T12</td>
            <td>Implementación de un sistema de autenticación segura en el backend</td>
            <td><strong>Como</strong> desarrollador de la plataforma, <strong>quiero</strong> implementar un sistema de autenticación segura, <strong>para</strong> proteger las credenciales de los usuarios y asegurar el acceso a la plataforma.</td>
            <td>2 horas</td>
            <td>Yen Cerna, Lucio Heli</td>
            <td>Done</td>
        </tr>
                <tr>
            <td>US28</td>
            <td>Creación de roadmaps personalizados ilimitados y compartirlos con los demás usuarios de la aplicación</td>
            <td>T06</td>
            <td>Creación de roadmaps y compartirlos con los demás usuarios de la aplicación</td>
            <td>Como usuario interesado en planificar su trayectoria profesional, quiero crear un roadmap académico básico en la plataforma,para visualizar y gestionar mi progreso académico y planificar mis cursos y metas profesionales.</td>
            <td>4 horas</td>
            <td>Pescoran Angulo, Juan Fabrizzio</td>
            <td>Done</td>
        </tr>
                </tr>
                <tr>
            <td>US29</td>
            <td>Recibir análisis avanzados sobre mi propio roadmap</td>
            <td>T07</td>
            <td>Recibir análisis avanzados sobre mi propio roadmap</td>
            <td>Como usuario Premium, quiero recibir análisis avanzados sobre mi propio roadmap, para obtener información detallada y perspicaz que me ayude a optimizar mi planificación y alcanzar mis objetivos profesionales más eficientemente..</td>
            <td>4 horas</td>
            <td>Pescoran Angulo, Juan Fabrizzio</td>
            <td>Done</td>
        </tr>
                </tr>
    </table>

Con el fin de que la lista de tareas en el sprint pueda ser visualizada a más profundidad, se mostrara un enlace directo a la sección de trabajo designada por el equipo junto a todas las actividades planificadas de forma completa: 

###### Figura 58
*Presentación de la tabla de actividades designada para el Sprint 2 en ClickUp.*
<img src="/assets/img/Lista de Tareas-Sprint2.png" alt="Lista de Tareas del Sprint 1 En ClickUp">

#### 5.2.2.3 Development Evidence for Sprint Review.

En esta sección se explica y presenta los avances en implementación con relación a los productos de la solución según el alcance del Sprint: Web Application. Aquí se dejara cada uno de los commits ya implementados dentro del repositorio de Github, junto a toda la información referente y a los cambios concluidos.

###### Tabla XX
*Tabla de los commits realizados y relacionados con el desarrollo de todas las secciones del Sprint Backlog 2*
| Repository | Branch| Commit Id| Commit Message| Commit Message Body|Commited on (Date) |
|------------|-------|----------|---------------|--------------------|-------------------|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|2085a4451325f1d0668047d8cb6b2ea986d11b59|Initial commit| 15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|97844950e2f718610501441269a798e12a09335e|feat(pom)|added dependencies and pluggins to work with|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|e0bff2d2c61620faebff1677756d311003cf2710|feat(shared) | added aggregate and entity for model in shared|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|e0bff2d2c61620faebff1677756d311003cf2710|feat(shared) | added openapi documentation|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|2b25ddce453a9cc5607d5d84605a366aafc60f3d|feat(shared) | added messageresource to handling errors|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|c61c607c468d92badf5782a17f68a146de5b3156|feat(shared) | added mongodb connection string with environment variables|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|529d6cd57e62dd85b5e7481673baf93753637540|feat(shared) | added getter annotation for auditable root|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|a2c7bcfef24588dff3c58e7e12e7e8c18678e05b|feat(iam) | add queries and commands for domain model|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|eef09f53e6a0def5c69d68eeecc7d946c8dc6046|feat(iam) | add aggregate, entity and value object|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|563a45cf85acf62a3b6188c9825aa44e623c048c|feat(iam) | add services into domain model for role and user|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|d4b16c16c6187ea0b631c6e9ebfd34418573639d|feat(iam) | add aggregate and entity into domain model|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|01ef289b8e06c608437e83fe9f784942133aab16|feat(iam) | add repositories into infrastructure using spring data mongodb|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|b772481b7f9265fa7cdd7755547df926a8d0c3c9|feat | add configurations to run application|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|dad58f32480d06eb505510c553488c63dfdf575a|feat(iam) | add endpoints for roles, users and iam|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|eaad313305eea6cc6ad968962a9c12220f68640d|feat(iam) | add resources and transform into interfaces directory to work with endpoints|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|06e2d6ad69877a6a17ccc4d3b407fb4433647cbe|fix(shared) | changed id from string to long|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|c461a5a847ab8e04a064edc5eb6afc50dafd3ae2|fix(iam) | fix variable type for these files|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|ff2fb2a6c541ffb7572bf0e47de580ab81655e08|feat(iam) | add implementation for services|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|8439db4b61723bda9a4d78319cad58f62188022e|feat(iam) | add security measures for tokens, login, etc|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|a0960fb7e3c2852f56e96310e284f263c1a43b15|feat(iam) | add services for tokens, hashing, etc|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|43b1bbbef36b5347980e1a24189be88b57055619|feat(iam) | add facade to interact with other bounded contexts|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|446d39aec1d5012e434eb6ee0dbf0ce20617c19c|refactor(pom) | add management dependencies|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|52bedcd93b6974510c1c8eea0e45e74194b13a70|refactor(pom) | refactored pom.xml|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|aa04417c3937ea4646487613b11352f9f2e9460d|refactor(pom) | refactored application.properties|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|f360d9db097b676f756a7c783673acad7bb8b6d7|feat(pom) | add dependencies to pom for openai service and apache http components|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|5138178d855314fc986d7527266533a8a93c56ea|feat(roadmap) | add command and queries for domain model|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|6ab57299e68457af7250c3cf33c2d08dbd7085fc|feat(roadmap) | add outbound service in application layer|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|eaa28f963e1abc9f32012ce68d32ce9d5469038f|feat(roadmap) | add entities, value objects and aggregates for domain layer|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|131c8525f8e9ded47671249807295f7961f76e2c|feat(roadmap) | add service interfaces for roadmap aggregate and both, ai interaction and ai recommendations|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|e33627bc8c10b32d81bbb8b2eab5cb07344e59da|feat(roadmap) | add service implementation for roadmap aggregate and both, ai interaction and ai recommendations|15/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|develop|90d29b3a2d8224de3d92f3fad82b9ba3e1d49cdd|feat(roadmap) | add repository for roadmap aggregate and ai recommendations|15/09/24|

#### 5.2.2.4 Testing Suite Evidence for Sprint Review. 

En esta sección presentaremos la evidencia detallada de las pruebas rigurosas realizadas durante el sprint. Para garantizar la calidad y funcionalidad del producto, hemos empleado la metodología Gherkin para definir escenarios de prueba claros y concisos. Cada uno de estos escenarios se ha registrado meticulosamente en commits específicos en nuestro repositorio de código, lo que proporciona un registro completo y transparente de nuestro proceso de prueba.

###### Tabla 26
*Tabla de los modelos de pruebas realizados y relacionados con el desarrollo de todas las secciones del Sprint Backlog 2*
| Repository                        | Branch              | Commit Id                          | Commit Message                   | Commit Message Body           |Commited on (Date) |
|-----------------------------------|---------------------|------------------------------------|----------------------------------|-------------------------------|-------------------|
| upc-pre-202401--si730-WS52-SmarTech-AcceptanceTests | feat(.features): added More User Stories - Ruben - 1 | ff860b5 | feat(.features): added More User Stories | En esta sección se implementaron todos los Acceptance Test para el Sprint 2 de Propertunity | 30/04/24 |

#### 5.2.2.5 Execution Evidence for Sprint Review. 

#### 5.2.2.6 Services Documentation Evidence for Sprint Review. 

En esta sección, presentamos la relación de Endpoints documentados con OpenAPI, que están directamente vinculados con el alcance del Sprint. Iniciamos con una breve introducción que resume los logros alcanzados en relación con la Documentación de Web Services durante este período de desarrollo. A continuación, proporcionamos una tabla detallada que enumera cada Endpoint, junto con las acciones implementadas y los enlaces correspondientes a la documentación desplegada o la URL local en Sprints anteriores al despliegue de Web Services.

El siguiente enlace proporcionará acceso al modelo de DBJson utilizado como una representación simulada de API antes de la integración y construcción de una API completa y final para Propertunity. Este enlace está ubicado dentro de nuestra plataforma FrontEnd y sirve como punto de referencia crucial durante el proceso de desarrollo y prueba.

Al hacer clic en este enlace, los desarrolladores y miembros del equipo pueden acceder al modelo de datos completo en formato JSON, que representa de manera precisa la estructura y la organización de los datos utilizados en nuestra aplicación. Este modelo de DBJson sirve como un punto de partida fundamental para comprender la lógica subyacente de nuestra aplicación y cómo interactúa con la base de datos: https://github.com/SmarTech-Propertunity/upc-pre-202401--si730-WS52-SmarTech-FrontEnd/blob/main/server/db.json

En la tabla, se indican las acciones soportadas para cada Endpoint, incluyendo el verbo HTTP (GET, POST, PUT, DELETE, PATCH), la sintaxis de llamada, la especificación de posibles parámetros y se incluye un ejemplo junto con una explicación del response correspondiente. Además de la tabla, se presentan capturas de pantalla que ilustran la interacción con la documentación elaborada, utilizando datos de muestra para demostrar cómo se utiliza cada Endpoint. En este caso, vamos a dar una explicación completa de 3 clases con respecto a todo el modelo del DBJson para poder dar una idea completa y, a la vez, no abrumar al lector con grandes cúmulos de información base en un modelo CRUD:

###### Tabla 27
*Tabla del modelo de escritura para el Bounded Context de IAM*
| Método  | Descripción                                  | Ejemplo de llamada         | Parámetros                                     | Respuesta                                                                                 |
|---------|----------------------------------------------|----------------------------|------------------------------------------------|-------------------------------------------------------------------------------------------|
| GET     | Obtener todos los usuarios                   | GET /usuarios               | Ninguno                                        | Lista de usuarios en formato JSON con detalles como nombre, correo, fecha de registro, etc.|
| POST    | Crear un nuevo usuario                       | POST /usuarios              | `username`, `email`, `password`                | Detalles del nuevo usuario creado en formato JSON, incluyendo ID y fecha de creación.      |
| PUT     | Actualizar la información de un usuario      | PUT /usuarios/{id}          | `username`, `email`, `password`                | Usuario actualizado con los nuevos datos proporcionados.                                  |
| DELETE  | Eliminar un usuario                          | DELETE /usuarios/{id}       | `id` del usuario                               | Mensaje de confirmación de eliminación del usuario.                                        |
| GET     | Obtener detalles de un usuario específico    | GET /usuarios/{id}          | `id` del usuario                               | Detalles del usuario solicitado, incluyendo roles, fecha de registro, y demás datos.       |
| POST    | Autenticación de usuario                     | POST /usuarios/authenticate | `username`, `password`                         | Token JWT válido para autenticar las siguientes peticiones del usuario.                    |
| POST    | Actualizar la contraseña de un usuario       | POST /usuarios/{id}/password| `id`, `newPassword`, `oldPassword`             | Confirmación de la actualización de la contraseña.                                         |


###### Tabla 28
Tabla del modelo de escritura para el Bounded Context de Roadmaps:
| Método  | Descripción                                            | Ejemplo de llamada               | Parámetros                                                      | Respuesta                                                                                 |
|---------|--------------------------------------------------------|----------------------------------|-----------------------------------------------------------------|-------------------------------------------------------------------------------------------|
| GET     | Obtener todos los roadmaps disponibles                 | GET /roadmaps                    | Ninguno                                                         | Lista de roadmaps en formato JSON con detalles como título, descripción, nodos, edges, etc.|
| POST    | Crear un nuevo roadmap                                 | POST /roadmaps                   | `title`, `description`, `nodes[]`, `edges[]`                    | Detalles del nuevo roadmap creado, incluyendo ID y fecha de creación.                     |
| PUT     | Modificar un roadmap existente                         | PUT /roadmaps/{id}               | `title`, `description`, `nodes[]`, `edges[]`                    | Roadmap actualizado con la nueva información proporcionada.                               |
| DELETE  | Eliminar un roadmap                                    | DELETE /roadmaps/{id}            | `id` del roadmap                                                | Mensaje de confirmación de eliminación del roadmap.                                        |
| GET     | Obtener detalles de un roadmap específico              | GET /roadmaps/{id}               | `id` del roadmap                                                | Detalles del roadmap solicitado, con nodos y edges.                                       |
| POST    | Generar recomendaciones mediante IA para un roadmap    | POST /roadmaps/{id}/recommendations | `id`, `userPrompt`, `aiToken`                                   | Respuesta de la IA con sugerencias personalizadas para el roadmap.                        |
| GET     | Obtener todas las interacciones con IA relacionadas    | GET /roadmaps/{id}/ai-interactions | `id` del roadmap                                                | Lista de interacciones y respuestas de la IA relacionadas con el roadmap.                 |
| POST    | Finalizar el roadmap                                   | POST /roadmaps/{id}/finish       | `id`, `feedback`                                                | Confirmación de finalización del roadmap y detalles de la retroalimentación proporcionada. |


#### 5.2.2.7 Software Deployment Evidence for Sprint Review.

#### 5.2.2.8 Team Collaboration Insights during Sprint.

Durante el Sprint 1 de la sección Software Development & Implementation, nos enfocamos en el desarrollo colaborativo del propio BackEnd de la aplicación móvil de Roademics, donde cada miembro del equipo contribuyó con sus habilidades y conocimientos. Esta colaboración se refleja en los numerosos commits realizados en nuestro repositorio de código, los cuales están respaldados por capturas de pantalla adjuntas para una documentación detallada.

Nuestro equipo se reunió tanto en persona como virtualmente para asignar tareas y discutir la estrategia de desarrollo del proyecto. Estas reuniones fueron cruciales para clarificar nuestras responsabilidades individuales y asegurar un desempeño óptimo. Para maximizar la eficiencia, decidimos asignar a cada miembro del equipo una sección específica del BackEnd para desarrollar, lo que nos permitió avanzar rápidamente y cumplir con los plazos establecidos.

Además, programamos sesiones regulares de brainstorming y resolución de problemas, donde compartimos ideas y abordamos cualquier duda o dificultad que surgiera durante el proceso de desarrollo. Estas reuniones fueron fundamentales para resolver obstáculos de manera efectiva y garantizar un progreso constante en la elaboración del FrontEnd del Web Application.

###### Figura 88
*Reporte completo de contribuciones para el desarrollo del BackEnd de la Aplicación Móvil de Roademics durante el Sprint 2 de Software Development & Implementation.*

<img src="/assets/img/Pulse-backend-for-main-sprint1.png" alt="Pulse for the Main Branch in Software Development and Implementation">
<img src="/assets/img/Contributions-backend-for-main-sprint1.png" alt=Contributions for the Main Branch in Software Development and Implementation ">
<img src="/assets/img/Individual-contributions-for-main-sprint1.png" alt="Individual Contributions for the Main Branch in Software Development and Implementation">

