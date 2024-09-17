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

**Requirements Management**: Para asegurar una organización efectiva del trabajo en nuestro equipo, en esta sección hemos implementado una metodología que utiliza herramientas diseñadas para la asignación y seguimiento de tareas, así como para la gestión de los requisitos del proyecto. En particular, h

- Organización de tareas: Hemos adoptado ClickUp como nuestra herramienta principal para la gestión de tareas del backend. La plataforma ofrece una interfaz amigable que facilita la división de las actividades relacionadas con la infraestructura y el desarrollo del backend entre los miembros del equipo. Al crear tableros personalizados y asignar tareas específicas del backend, podemos establecer plazos, asignar responsables y monitorear el progreso de cada tarea técnica de manera eficiente. Esta configuración nos permite evaluar el avance en la implementación de la API, servicios externos y despliegues, así como analizar el desempeño general del equipo de backend. ClickUp también permite revisar las contribuciones individuales y el trabajo realizado en la parte del servidor, promoviendo la transparencia y la colaboración efectiva dentro del equipo técnico.

Página oficial de ClickUp: https://clickup.com/ 

---

**Product Architecture Design**: Esta sección se centra en el desarrollo y diseño de la arquitectura del backend a lo largo de todo su ciclo de vida. Las herramientas seleccionadas deben ofrecer aplicaciones que permitan la creación de diagramas detallados y complejos de cada capa de la arquitectura del backend. Esto incluye la identificación de los componentes clave, como bases de datos, APIs y servicios externos, así como los frameworks, entornos de desarrollo (IDEs) y lenguajes de programación que se utilizarán. La capacidad de representar de manera clara y precisa la estructura del backend es esencial para asegurar que todos los aspectos técnicos sean comprensibles, bien documentados y alineados con los requisitos del sistema.

- Diagramas C4: Para diseñar los diagramas C4 del backend de nuestro proyecto, nuestro equipo ha optado por utilizar "Visual Paradigm". Esta herramienta ha sido seleccionada por sus características específicas que facilitan el modelado claro y efectivo de las vistas de arquitectura del backend según el enfoque C4. "Visual Paradigm" se destaca por su simplicidad en la creación de diagramas estructurados y su capacidad para ofrecer una representación visual comprensible tanto para desarrolladores como para partes interesadas no técnicas. La elección de esta herramienta se basa en su capacidad para generar diagramas detallados y precisos del backend sin necesidad de codificación de bajo nivel, lo que la convierte en una opción accesible y eficaz para documentar la arquitectura del backend de nuestro proyecto.

Página oficial de Visual Paradigm: https://www.visual-paradigm.com/

- Diagrama UML: Para el diseño de los diagramas UML relacionados con la arquitectura del backend de nuestro proyecto, hemos optado por "LucidChart". Esta plataforma es especialmente adecuada para la creación de diagramas UML del backend debido a su interfaz intuitiva y su amplia gama de herramientas específicas para el modelado de sistemas. "LucidChart" permite crear diagramas detallados y bien estructurados que representan con precisión la arquitectura del backend, incluyendo la estructura de bases de datos, relaciones entre microservicios y flujos de datos. La facilidad de uso y las opciones avanzadas para organizar y estructurar los diagramas hacen que "LucidChart" sea la herramienta ideal para garantizar una representación clara y completa de la arquitectura del backend. Su capacidad para integrar y organizar partes del diagrama facilita la colaboración y la comunicación entre los miembros del equipo técnico, especialmente entre los desarrolladores y arquitectos de software involucrados en el proyecto.

Página oficial de LucidChart: https://lucidchart.com/

- Diseño de Diagrama de Bases de Datos: Para el diseño de la base de datos no relacional de nuestro proyecto, hemos optado por "Moon Modeler". Esta herramienta es eficaz para el modelado y visualización de bases de datos no relacionales, como MongoDB. Ofrece una interfaz intuitiva que facilita la creación de diagramas detallados y bien estructurados, permitiendo diseñar esquemas claros y precisos para la estructura de datos del backend. "Moon Modeler" proporciona funcionalidades como la generación automática de documentación y la exportación de diseños en varios formatos, lo cual es esencial para una correcta representación y documentación de la base de datos. Aunque la herramienta está diseñada para el trabajo individual y no está orientada a la colaboración en tiempo real, permite la creación y revisión de modelos de datos, con la colaboración facilitada a través del intercambio de archivos exportados. Esta característica debe ser considerada al integrar el diseño de bases de datos en el flujo de trabajo del equipo de backend.

Página oficial de Moon Modeler: https://www.datensen.com/data-modeling/moon-modeler-for-databases.html 

---

**Web Services**: En esta sección estarán las herramientas de desarrollo del Web Services con el Backend. Es esencial adoptar frameworks y metodologías que garanticen una programación eficiente y la implementación de un backend robusto y de alto rendimiento. Utilizaremos frameworks que proporcionen bibliotecas preimplementadas para facilitar la creación, configuración y manejo de los servicios web. Estos frameworks permiten una integración fluida de los servicios, optimizando el rendimiento y asegurando que el backend pueda manejar de manera eficiente las solicitudes y respuestas entre los diferentes componentes del sistema.

- Modelo de Arquitectura: El estilo arquitectónico elegido para la aplicación será RESTful API, conocido por su eficacia en establecer una comunicación eficiente y directa entre clientes y servidores. Este enfoque es ampliamente reconocido por su capacidad para alinearse con las mejores prácticas de diseño y seguridad, lo que resulta fundamental para cualquier aplicación moderna. Al adoptar este estilo arquitectónico, se garantiza la creación de un backend no solo robusto, sino también altamente escalable, capaz de adaptarse a las crecientes demandas del sistema. Esto, a su vez, promueve un desarrollo coherente y seguro, estableciendo las bases necesarias para un rendimiento óptimo y una experiencia de usuario fiable.

Página de guía y seguimiento para el modelo REST: https://es.apis.support.brightcove.com/getting-started/learning-guide-using-rest-apis.html 

- Desarrollo de código: Para el desarrollo propio del código del backend, se optará por utilizar Java junto con el framework Spring Boot. Spring Boot facilita enormemente la creación de aplicaciones basadas en Spring, ya que ofrece un conjunto completo de funcionalidades preconfiguradas para construir servicios web eficientes y rápidos. Mientras tanto, Java es un lenguaje de programación altamente robusto y versátil, conocido por su eficiencia, seguridad y amplia comunidad de soporte. Esta combinación de tecnologías permite establecer un entorno de desarrollo sólido y flexible, adaptado a las necesidades actuales del proyecto. Al emplear Spring Boot con Java, se garantiza una infraestructura capaz de manejar las demandas de un backend de alto rendimiento, ofreciendo escalabilidad, mantenibilidad y una integración más fluida con otros componentes del sistema.

Página oficial de Spring Boot: https://spring.io/projects/spring-boot

Página de guía y seguimiento para Java: https://www.oracle.com/java/technologies/javase-jdk11-downloads.html

- Entorno de desarrollo integrado: El IDE seleccionado para este proceso será IntelliJ IDEA, que forma parte del conjunto de herramientas de JetBrains Toolbox. IntelliJ IDEA es ampliamente reconocido por sus potentes características específicas para el desarrollo en Java, brindando un entorno que facilita enormemente la codificación, depuración y gestión de proyectos. Gracias a sus funciones avanzadas, como la autocompletación inteligente, análisis de código en tiempo real y herramientas de refactorización, se logra un proceso de desarrollo más ágil y productivo, reduciendo significativamente los errores y mejorando la calidad del código.

Página oficial de IntelliJ IDEA: https://www.jetbrains.com/idea/

- Documentación de servicios webs se empleará Swagger, basado en la OpenAPI Specification. Swagger se ha consolidado como un estándar en la industria para la documentación de APIs, ya que ofrece una estructura clara y coherente que facilita su comprensión y uso, tanto por desarrolladores internos como externos. Además, Swagger permite registrar y reflejar rápidamente los cambios realizados en la API durante el proceso de desarrollo, garantizando que la documentación se mantenga precisa y actualizada en todo momento. Esto no solo mejora la comunicación entre los equipos, sino que también asegura un desarrollo más eficiente y colaborativo.

Página oficial de Swagger: https://swagger.io/

---

**Software Deployment**: Esta sección se centra en las herramientas y aplicaciones necesarias para llevar a cabo el despliegue e implementación efectiva del backend desarrollado a lo largo del ciclo de vida del proyecto. Los recursos seleccionados deben ser fáciles de usar y ofrecer alta confiabilidad para garantizar que el backend se implemente sin problemas de rendimiento o inconsistencias en su funcionamiento. 

Para el despliegue del backend, se optará por utilizar servicios en la nube como AWS o Heroku, que proporcionan un entorno robusto y confiable para alojar aplicaciones. Estas plataformas ofrecen escalabilidad y monitorización en tiempo real, lo que asegura que el backend pueda manejar las demandas del sistema de manera eficiente. Además, su facilidad de configuración y despliegue automatizado contribuye a un proceso de implementación fluido y seguro.

Página oficial de GitHub Pages: https://pages.github.com/

---

**Software Document**: Esta sección detalla las herramientas y aplicaciones seleccionadas para la documentación exhaustiva del código y del software a lo largo del ciclo de vida del proyecto. Las herramientas deben ser intuitivas para todos los miembros del equipo y capaces de gestionar documentación extensa, con soporte para imágenes y una estructura de secciones clara y organizada.

Para la documentación, se utilizará un repositorio en GitHub, estructurado en múltiples ramas según las necesidades del equipo. La redacción de la documentación se llevará a cabo principalmente en Markdown, lo que garantiza una visualización coherente en la web a través de diferentes dispositivos, además de facilitar la compresión y el cifrado de los datos. En situaciones donde Markdown no sea suficiente, como para la creación de tablas complejas, se empleará HTML para lograr una representación más precisa y detallada.

Página oficial de GitHub: https://github.com/

Guía de uso de Markdown: https://www.markdownguide.org/

Guía y seguimiento para HTML5: https://www.w3schools.com/html/

### 4.1.2. Source Code Management.

En esta sección, se definirá la estrategia para utilizar GitHub como plataforma de control de versiones y colaboración durante el ciclo de vida del desarrollo del backend. Se emplearán todas las herramientas proporcionadas por GitHub para garantizar una gestión eficaz del código fuente, incluyendo el seguimiento de versiones y la colaboración entre miembros del equipo. Se mantendrá un registro exhaustivo de las versiones del backend, permitiendo rastrear cambios, identificar nuevos desarrollos y corregir errores de manera precisa.

Se establecerán ramas específicas para diferentes etapas del desarrollo, tales como la integración continua, las pruebas y la producción. Además, se implementarán políticas de pull requests y revisiones de código para asegurar la calidad y coherencia del backend. Esta metodología permitirá un control riguroso del ciclo de vida del desarrollo, facilitando la colaboración y asegurando que todos los cambios se registren de forma clara y ordenada.

A continuación, se proporciona una lista con los enlaces a la organización de GitHub de WHAI y a los repositorios específicos relacionados con el desarrollo del backend dentro de esta organización:

Repositorios en GitHub:

- Organización: https://github.com/GRUPO-3-MOVILES 

- BackEnd: https://github.com/GRUPO-3-MOVILES/upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd 

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

Formato de Commit:

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

En esta sección, nuestro equipo explicará y establecerá las referencias que adoptaremos para nombrar y programar en los lenguajes de programación que se utilizarán en el desarrollo de nuestra solución de software, incluyendo la Landing Page y la Web Application. A continuación, especificaremos las convenciones para los siguientes lenguajes y herramientas:

- Guía de Estilo para Spring Boot: https://docs.spring.io/spring-boot/docs/current/reference/html/
- Guía de Estilo para Java del AOSP para colaboradores: https://source.android.com/docs/setup/contribute/code-style?hl=es-419
- Manual Completo de Código en Java: https://www.manualweb.net/java/
- Modelo de Convenciones de codificación Java: https://codegym.cc/es/groups/posts/es.491.convenciones-de-codificacion-de-java-cuales-seguir-y-por-que
- Convenciones de Gherkin para especificaciones legibles: https://specflow.org/gherkin/gherkin-conventions-for-readable-specifications/

**Convenciones que Usaremos**

**Java:**
- Usar nombres descriptivos y claros para clases, métodos y variables. Aplicar PascalCase para nombres de clases y camelCase para nombres de métodos y variables.
- Organizar el código en paquetes lógicos para mantener la modularidad y la estructura del proyecto.
- Documentar el código con comentarios Javadoc para explicar el propósito de las clases, métodos y parámetros. Mantener la documentación actualizada y precisa.
- Seguir el principio de responsabilidad única, asegurando que cada clase y método tenga una única responsabilidad.
- Implementar manejo de excepciones utilizando bloques try-catch y definir excepciones personalizadas cuando sea necesario para manejar errores específicos.
- Utilizar interfaces y clases abstractas para promover la reutilización del código y la extensibilidad.
- Adoptar los principios SOLID para diseñar clases y sistemas mantenibles y escalables.

**Spring Boot**:
- Seguir la estructura de proyecto recomendada por Spring Boot, separando las capas de presentación, lógica de negocio y acceso a datos.
- Utilizar la inyección de dependencias proporcionada por Spring para gestionar los componentes y servicios de la aplicación, promoviendo la modularidad y la testabilidad.
- Aplicar el patrón de diseño MVC (Modelo-Vista-Controlador) o el patrón de arquitectura de microservicios según la complejidad del proyecto.
- Configurar las propiedades de la aplicación utilizando archivos application.properties o application.yml y gestionar la configuración mediante perfiles de entorno.
- Implementar la gestión de errores y excepciones utilizando el soporte de manejo global de errores de Spring y definir controladores de errores personalizados.
- Usar la caché proporcionada por Spring para mejorar el rendimiento, almacenando datos que se acceden con frecuencia y que son costosos de recuperar.
- Asegurar la aplicación mediante autenticación y autorización utilizando los mecanismos de seguridad integrados de Spring Security.
- Implementar pruebas unitarias y de integración utilizando el soporte de pruebas de Spring Boot para asegurar la calidad del código y la funcionalidad de la aplicación.

### 4.1.4. Software Deployment Configuration.

En esta sección, detallaremos la configuración necesaria para implementar la solución, centrándonos específicamente en el despliegue del Backend. Comenzaremos creando un repositorio en GitHub destinado a almacenar los archivos HTML, CSS y JavaScript que componen nuestra página de destino. Una vez establecido el repositorio, cada miembro del equipo trabajará en su propia rama "feature" para desarrollar las diferentes características del Landing Page. Tras completar una característica específica, se llevará a cabo el proceso de merge con la rama "develop", garantizando así que la página de destino esté siempre actualizada con las últimas modificaciones y mejoras implementadas.

## 4.2. Software Development & Implementation.

A continuación, describimos en detalle el enfoque técnico que adoptaremos para la implementación, pruebas y despliegue de nuestra infraestructura backend, centrado en la creación y gestión de los servicios web, así como en la integración con la base de datos y el manejo eficiente de las API necesarias para el correcto funcionamiento de la aplicación. Este proceso abarca el desarrollo de servicios backend escalables, la validación exhaustiva mediante pruebas unitarias y de integración, y la optimización del rendimiento antes de cada ciclo de despliegue en el entorno de producción. 

### 4.2.1. Sprint 1

En esta sección se registra y explica el avance en términos de producto y trabajo colaborativo para el Sprint número 1. Todo el avance descriptivo se muestra aquí junto a su desarrollo, historial y avance en conjunto dado por cada intengrante del equipo de trabajo. Todas las especificaciones siguen desde el Product Backlog del Capitulo 2 en la sección de requerimientos.

#### 5.2.2.1 Sprint Planning 1.

En esta sección se explicaran los detalles presentados y analizados durante la reunión del Sprint Planning para el número 1. El objetivo principal de esta reunión es establecer un plan claro y realista para el sprint, identificando las tareas a realizar y comprometiéndose con un conjunto de entregables concretos que contribuyan al avance del proyecto. A continuación, se presenta el resumen del Sprint Planning Meeting, que proporcionará una visión general de los temas discutidos y las decisiones tomadas durante la reunión.

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
            <td>2024-09-07</td>
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
            <td>Sprint 1 - 1 Review Summary</td>
            <td>Después de un realizar todos los procedimientos establecidos para la identificación de objetivos y áreas de retroalimentación, hemos podido concluir la reunión del sprint 1 con éxito en términos de avance en los productos de software y en la colaboración general del equipo. El proceso de mejora con la retroalimentación y la programación de varias secciones nuevas en la Aplicación Web significó un gran proceso de mejora para la construcción y realización del sprint, además de reforzar el compromiso de nuestro equipo y la mejora exponencial de las actividades indicadas.</td> 
        </tr>
            <tr>
            <td>Sprint 1 – 1 Retrospective Summary</td>
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
            <td>Sprint 1 Velocity</td>
            <td>Con el equipo para este sprint 1 decidimos aceptar 5 Story Points</td>
        </tr>
              <tr>
            <td>Sum of Story Points</td>
            <td>La suma de los Story Points para los User Stories que se están incluyendo en este Sprint 1 es XX</td>
        </tr>
    </table>

#### 5.2.2.2 Sprint Backlog 1.

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

(Mejorar)

### 4.2.2. Sprint 2

En esta sección se registra y explica el avance en términos de producto y trabajo colaborativo para el Sprint número 1. Todo el avance descriptivo se muestra aquí junto a su desarrollo, historial y avance en conjunto dado por cada intengrante del equipo de trabajo. Todas las especificaciones siguen desde el Product Backlog del Capitulo 2 en la sección de requerimientos.

#### 5.2.2.2 Sprint Planning 2.

En esta sección se explicaran los detalles presentados y analizados durante la reunión del Sprint Planning para el número 1. El objetivo principal de esta reunión es establecer un plan claro y realista para el sprint, identificando las tareas a realizar y comprometiéndose con un conjunto de entregables concretos que contribuyan al avance del proyecto. A continuación, se presenta el resumen del Sprint Planning Meeting, que proporcionará una visión general de los temas discutidos y las decisiones tomadas durante la reunión.

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
            <td>Sprint 1 - 1 Review Summary</td>
            <td>Después de un realizar todos los procedimientos establecidos para la identificación de objetivos y áreas de retroalimentación, hemos podido concluir la reunión del sprint 1 con éxito en términos de avance en los productos de software y en la colaboración general del equipo. El proceso de mejora con la retroalimentación y la programación de varias secciones nuevas en la Aplicación Web significó un gran proceso de mejora para la construcción y realización del sprint, además de reforzar el compromiso de nuestro equipo y la mejora exponencial de las actividades indicadas.</td> 
        </tr>
            <tr>
            <td>Sprint 1 – 1 Retrospective Summary</td>
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

#### 5.2.2.2 Sprint Backlog 1.

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
