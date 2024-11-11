# Capítulo 5: Product Implementation & Validation

## 5.1. Software Configuration Management.
En la gestión de la configuración del frontend para la aplicación móvil Roademics, nos centramos en el desarrollo de una interfaz de usuario altamente intuitiva y responsiva, utilizando Flutter y Dart. Estos lenguajes permiten la creación de aplicaciones nativas multiplataforma, lo que optimiza el rendimiento y la experiencia del usuario en dispositivos móviles. La estructura del código se organiza de manera modular, lo que facilita la colaboración entre los miembros del equipo y permite una rápida iteración en el desarrollo.

Adicionalmente, se implementan sistemas de control de versiones mediante Git, asegurando un manejo riguroso de las versiones del código fuente y promoviendo la cohesión del equipo. Los componentes de la interfaz se desarrollan siguiendo las mejores prácticas de diseño, garantizando una experiencia de usuario fluida y atractiva. También se establecen pipelines de CI/CD (Integración Continua y Despliegue Continuo) para automatizar pruebas de interfaz, asegurando que cualquier nueva funcionalidad cumpla con los estándares de calidad antes de ser integrada en el entorno de producción.

Asimismo, la Landing Page de Roademics juega un papel fundamental en la presentación de la aplicación, actuando como la primera interacción que los usuarios tienen con la plataforma. Esta página está diseñada para ser visualmente atractiva y funcional, brindando información clara sobre las características y beneficios de la aplicación. Se implementan elementos de diseño responsivo que permiten que la página se adapte a diferentes tamaños de pantalla, asegurando una experiencia de usuario óptima en todos los dispositivos.

La correcta implementación del frontend es crítica para garantizar que tanto los reclutadores y empresas, como los estudiantes y profesionales, puedan interactuar de manera efectiva con la plataforma. Al proporcionar un acceso sencillo a la exploración y gestión de los roadmaps profesionales, se mejora la satisfacción del usuario y se fomenta una mayor participación. Esta sólida base en el frontend, junto con la integración armoniosa de los elementos visuales y funcionales, se complementa con la infraestructura que se detallará en los capítulos posteriores de esta documentación, asegurando una plataforma robusta y escalable capaz de responder ágilmente a las necesidades de los usuarios finales.

### 5.1.1. Software Development Environment Configuration.

En esta sección, el equipo de desarrollo detallará las herramientas de software esenciales para el frontend de la aplicación móvil, especificando el nombre de cada producto, su propósito dentro del proyecto y el método de acceso o instalación. Para las herramientas basadas en SaaS (Software como Servicio), se proporcionará la URL de acceso a sus respectivas páginas web, mientras que para aquellas que requieren instalación local, se indicará la ruta de descarga adecuada.

Las herramientas seleccionadas abarcan actividades críticas para el desarrollo del frontend, incluyendo la gestión de componentes de interfaz de usuario, el control de versiones, el desarrollo y la prueba de aplicaciones. Cada herramienta ha sido cuidadosamente elegida para optimizar el flujo de trabajo del equipo, asegurando una colaboración efectiva y un desarrollo ágil. Estas herramientas no solo facilitan la implementación de una interfaz de usuario atractiva y funcional, sino que también permiten realizar pruebas exhaustivas y automatizar procesos repetitivos, lo que contribuye a una mayor eficiencia en el ciclo de desarrollo.

**Project Management**: Esta sección aborda la planificación y supervisión del proyecto durante todo su ciclo de vida, incluyendo la coordinación del equipo, la gestión de sus tareas y colaboraciones, así como la asignación de responsabilidades previamente establecidas. Para estructurar esta gestión, hemos dividido el enfoque en métodos distintos de comunicación y administración del equipo.

- Reuniones de Trabajo: Para la coordinación de las tareas del equipo de frontend, utilizamos Discord como nuestra plataforma principal de comunicación. Esta elección se fundamenta en la familiaridad del equipo con la herramienta, lo que permite una comunicación ágil y efectiva para la discusión de temas técnicos relacionados con el desarrollo de la interfaz de usuario y la experiencia del usuario. A pesar de que Discord puede no contar con ciertas características avanzadas que ofrecen otras plataformas, su interfaz intuitiva y la posibilidad de realizar reuniones sin restricciones de tiempo nos facilitan la planificación detallada de los componentes de la aplicación y la resolución de problemas complejos relacionados con el frontend. Además, los canales temáticos en Discord permiten organizar conversaciones específicas sobre desarrollo de UI, pruebas de usabilidad, optimización del rendimiento, y gestión de bibliotecas y frameworks, lo que mejora significativamente el seguimiento de los temas relevantes al frontend. 

Página oficial de Discord: https://discord.com/

- Control de Versiones: Para la gestión del control de versiones del frontend, utilizamos las herramientas integradas de GitHub. Esta plataforma permite al equipo colaborar de manera eficiente a través de commits y pull requests específicos para el código de la interfaz de usuario. Los commits documentan detalladamente los cambios realizados en la lógica del cliente, así como en los componentes visuales y estilos CSS, proporcionando un historial claro que facilita la revisión y el seguimiento de las modificaciones en el frontend. Los pull requests permiten una revisión exhaustiva y discusión de los cambios propuestos antes de su integración en la rama principal, asegurando que las nuevas funcionalidades y mejoras en la interfaz se implementen de forma controlada y sin comprometer la estabilidad y la usabilidad de la aplicación. Además, el uso de GitHub como herramienta de control de versiones facilita la implementación de estrategias de ramificación, lo que permite a los miembros del equipo trabajar en características individuales o mejoras sin afectar el flujo de trabajo general.

Página oficial de Github: https://github.com/

---

**Requirements Management**: Para asegurar una organización efectiva del trabajo en nuestro equipo de frontend, en esta sección hemos implementado una metodología que utiliza herramientas específicamente diseñadas para la asignación y seguimiento de tareas relacionadas con el desarrollo de la interfaz de usuario. Estas herramientas no solo facilitan la gestión de los requisitos del proyecto, sino que también permiten una comunicación fluida entre los miembros del equipo, asegurando que cada uno esté alineado con los objetivos y plazos establecidos.

- Organización de tareas: Hemos adoptado ClickUp como nuestra herramienta principal para la gestión de tareas del frontend. La plataforma ofrece una interfaz amigable que facilita la división de las actividades relacionadas con el diseño y desarrollo de la interfaz de usuario entre los miembros del equipo. Al crear tableros personalizados y asignar tareas específicas del frontend, podemos establecer plazos, designar responsables y monitorear el progreso de cada tarea técnica de manera eficiente. Esta configuración nos permite evaluar el avance en la implementación de componentes de interfaz, pruebas de usabilidad y optimización del rendimiento, así como analizar el desempeño general del equipo de frontend. ClickUp también proporciona la capacidad de revisar las contribuciones individuales y el trabajo realizado en la parte visual de la aplicación, promoviendo la transparencia y la colaboración efectiva.
  
Página oficial de ClickUp: https://clickup.com/ 

---

**Product Architecture Design**: Esta sección se centra en el desarrollo y diseño de las diferentes capas de la arquitectura del producto a lo largo de su ciclo de vida. Las herramientas seleccionadas deben ofrecer una amplia gama de funcionalidades y estilos, permitiendo la creación de diagramas complejos que capturen de manera precisa cada componente de la arquitectura, incluidos los frameworks, IDEs y lenguajes de programación utilizados. La capacidad para diagramar de manera clara y detallada es crucial para identificar cada una de las capas que componen nuestra solución.

- Diagramas C4: Para la creación de los diagramas C4 relacionados con la arquitectura del producto, el equipo ha optado unánimemente por la plataforma VisualParadigm. Esta elección se fundamenta en varios aspectos clave que consideramos esenciales para un modelado claro, comprensible y efectivo, dirigido tanto a miembros técnicos como no técnicos del proyecto. VisualParadigm se distingue por ofrecer modelos optimizados y especializados para el desarrollo de diagramas C4, que permiten una representación clara de los sistemas complejos del FrontEnd. Su enfoque en la arquitectura y la visualización facilita la creación de diagramas que no solo son comprensibles para los desarrolladores, sino también para otros stakeholders, lo que es fundamental para alinear a todo el equipo en la evolución del proyecto. A diferencia de otras herramientas como Structurizr, VisualParadigm no requiere trabajar con código de bajo nivel para construir los diagramas, lo que lo hace mucho más accesible y eficiente para nuestro equipo.

Página oficial de Visual Paradigm: https://www.visual-paradigm.com/

- Diagramas UML: Para abordar el diseño de todos los diagramas UML relacionados con el frontend de nuestro proyecto y asegurar una representación precisa y detallada de la estructura de la interfaz y la interacción entre los componentes, nuestro equipo ha decidido unánimemente utilizar LucidChart. Esta plataforma es reconocida por su especialización en la creación de diagramas UML, lo que la convierte en la herramienta perfecta para nuestras necesidades de modelado de la interfaz de usuario y flujo de datos en el frontend. LucidChart proporciona una amplia variedad de herramientas y características específicamente orientadas a la creación de diagramas UML, lo que nos permite representar de manera clara y eficiente cada uno de los componentes de la interfaz, las interacciones entre ellos, y los flujos de datos que se producen dentro de la aplicación móvil desarrollada en Flutter y Dart. Gracias a su interfaz intuitiva, el proceso de diagramación se vuelve ágil, permitiendo que todo el equipo visualice y diseñe el frontend de forma colaborativa y productiva. Además, LucidChart ofrece opciones avanzadas para organizar y separar las diferentes capas y componentes dentro del diagrama UML, lo que facilita la estructuración de elementos como widgets, controladores de interfaz y flujos de navegación. 

Página oficial de LucidChart: https://lucidchart.com/

---

**Product UX/UI Design:** Esta sección respecta al desarrollo y diseñado de las secciones basadas en el UX y UI correspondientes a nuestro proyecto durante todo su ciclo de vida. Las herramientas utilizadas deben estar compuestas de varias aplicaciones con estilos varios que permitan modificar la estetica de todas las páginas que vamos a programar y como estas se verían para nuestros clientes finales, siguiendo las historias de usuario y toda metodologia de desarrollo web. Asimismo, estas herramientas también deben permitir la estructuración y diagramación de todas las tablas y organizadores necesarios.

- Mapas de guía: En relación con el diseño de los diagramas necesarios para el frontend de la aplicación, como el Empathy Map, el Journey Map y el Impact Map, hemos llegado a la conclusión unánime de que la plataforma UXPressia es la opción más adecuada para llevar a cabo esta tarea. Esta decisión se fundamenta en varios aspectos que consideramos esenciales para un proceso de diseño eficaz y colaborativo en el desarrollo de la interfaz de usuario. UXPressia se destaca por ofrecer un entorno de diseño más cómodo y accesible en comparación con otras soluciones disponibles en el mercado. Su interfaz intuitiva y herramientas integradas simplifican la creación de mapas de experiencia de usuario de manera rápida y precisa, lo cual es clave para el diseño centrado en el usuario. Además, la plataforma soporta un flujo de trabajo colaborativo, lo que permite que nuestro equipo de frontend trabaje de forma coordinada y eficiente en la creación de los mapas. 

- User Personas: En cuanto al diseño de User Personas para cada segmento objetivo identificado en nuestra startup y producto, hemos decidido utilizar la plataforma UXPressia. Aunque somos conscientes de que existen otras herramientas que ofrecen características más avanzadas, consideramos que UXPressia proporciona modelos predefinidos y formatos visualmente atractivos que nos permiten crear User Personas de manera eficaz y comprensible. Si bien reconocemos que la plataforma presenta algunas limitaciones en cuanto al desarrollo de gráficos más grandes y diagramas complejos, las ventajas que ofrece en términos de usabilidad, simplicidad y diseño compensan estos aspectos. Además, su interfaz amigable nos permite trabajar de manera ágil, enfocándonos en la creación de perfiles que reflejen con precisión los comportamientos, necesidades y objetivos de nuestros usuarios, facilitando así el desarrollo de una estrategia más centrada en el usuario.

Página oficial de UXPressia: https://uxpressia.com/ 

- Escenarios: Para la creación de escenarios correspondientes al AS-IS y TO-BE para nuestros segmentos de mercado, hemos seleccionado la plataforma web Miro como nuestra herramienta principal. Miro es una solución extremadamente versátil que ofrece una amplia gama de funcionalidades para el modelado de escenarios, tanto del estado actual (AS-IS) como del estado ideal o futuro (TO-BE). La plataforma permite visualizar y mapear fácilmente todos los puntos de contacto y acciones que el cliente realiza, ayudando a identificar las áreas de mejora y potenciales innovaciones en nuestro producto. Asimismo, la usabilidad de las plantillas de Miro permite a los diseñadores concentrarse en el análisis y la resolución de problemas sin tener que preocuparse por las cuestiones técnicas o de diseño que puedan surgir durante el modelado. Además, la función de trabajo colaborativo de Miro ofrece una ventaja significativa. Varios miembros del equipo pueden trabajar de manera simultánea y en tiempo real sobre un mismo tablero, lo que favorece la participación activa.

Página oficial de Miro: https://miro.com/ 

- Wireframes, Mock-ups y Prototypes: Para el desarrollo de wireframes, mock-ups y prototipos relacionados con la landing page de nuestra startup y todas las secciones de la aplicación móvil orientada al frontend, hemos decidido utilizar la plataforma Figma. Esta herramienta ha sido seleccionada por su especialización en el diseño de interfaces de usuario para aplicaciones móviles y sitios web, ofreciendo un conjunto robusto de características que abordan las necesidades tanto de diseñadores como de desarrolladores de productos digitales. Su capacidad para crear prototipos interactivos y simular experiencias reales de usuario nos permite probar y validar conceptos antes de pasar al desarrollo final. Otra de las razones clave para esta elección es el enfoque colaborativo de Figma, que permite que múltiples miembros del equipo trabajen simultáneamente en un mismo diseño. Otro aspecto importante de Figma es su vasta biblioteca de recursos y modelos predefinidos. Estos recursos proporcionan a nuestro equipo una base sólida sobre la cual construir los wireframes iniciales, mock-ups visuales y prototipos interactivos. Por último, la capacidad de Figma para simular la experiencia del usuario final en dispositivos móviles y navegadores es fundamental para garantizar que la aplicación web y la landing page proporcionen una experiencia de usuario óptima en todos los dispositivos y plataformas.

Página oficial de Figma: https://figma.com/ 

---

**Software Development**: Esta sección aborda las herramientas y aplicaciones necesarias para la programación de la Landing Page y la Mobile Application asociadas a nuestro proyecto, garantizando que su desarrollo se mantenga alineado con los principios metodológicos y funcionales del ciclo de vida completo del producto. Los instrumentos seleccionados abarcan IDEs, lenguajes de programación, bibliotecas y frameworks, todos ellos elegidos para asegurar que el diseño y la programación cumplan con los objetivos propuestos y respondan adecuadamente a las historias de usuario y esquemas arquitectónicos planteados.

- Landing Page: En el desarrollo de la landing page, hemos implementado un conjunto específico de herramientas que aseguran tanto la programación como la esquematización del proyecto de forma eficiente y escalable. Para ello, hemos optado por el uso combinado de HTML5, CSS3, y JavaScript, cada uno organizado en secciones individuales dentro del repositorio del equipo. Esta decisión responde a la versatilidad que ofrecen dichos lenguajes, indispensables en la creación de páginas web que cumplan con los estándares de calidad requeridos para un entorno de producción. El diseño visual seguirá las directrices del Material Design, una metodología ampliamente reconocida por su claridad, coherencia y estructura optimizada para la experiencia de usuario. Con este enfoque, buscamos no solo una apariencia atractiva, sino también garantizar una navegación intuitiva y efectiva que maximice la interacción del usuario con la página. El IDE seleccionado para este proyecto es Visual Studio Code, el cual será empleado para la edición y desarrollo del código. A pesar de ser un entorno de desarrollo más simple en comparación con IDEs más robustos, su amplia gama de funcionalidades y extensiones lo hace ideal para proyectos como este. Su interfaz sencilla y la posibilidad de integrar múltiples herramientas lo convierten en una opción práctica para la gestión ágil de código en la landing page.

Página oficial de Visual Studio Code: https://code.visualstudio.com/

Página de guía y seguimiento para HTML5: https://www.w3schools.com/html/ 

Página de guía y seguimiento para CSS3: https://www.w3schools.com/css/default.asp

Página de guía y seguimiento para JavaScript: https://developer.mozilla.org/es/docs/Web/JavaScript

Página de guía y seguimiento para el modelo del Material Design: https://m3.material.io/

- Mobile Application: En el proceso de desarrollo de la aplicación móvil frontend, se utilizarán una variedad de herramientas con el objetivo de asegurar una programación eficiente y una estructura coherente para cada uno de los componentes visuales y funcionales. Para este propósito, hemos optado por el uso del framework Flutter, que ofrece una sólida base para el desarrollo de aplicaciones móviles multiplataforma, con un enfoque centrado en la creación de interfaces de usuario fluidas y eficientes. Este framework, combinado con el lenguaje Dart, proporcionará un entorno técnico robusto para el desarrollo y permitirá una optimización adecuada de los componentes de la interfaz de usuario. Además, se aprovechará la biblioteca de widgets nativos de Flutter, que facilita la creación de elementos visuales coherentes y altamente personalizables, contribuyendo a la mantenibilidad y elegancia del código. Esto asegurará que la experiencia de usuario sea consistente en diferentes dispositivos y plataformas, permitiendo una navegación fluida y una interfaz altamente responsiva. En cuanto al entorno de desarrollo integrado (IDE), se empleará Visual Studio Code (VSCode). Este IDE ha sido seleccionado por su versatilidad, amplia gama de extensiones, y su capacidad para integrar de manera efectiva las herramientas necesarias para el desarrollo de aplicaciones móviles con Flutter. VSCode también destaca por su eficiencia en la depuración de código, permitiendo realizar actualizaciones inmediatas sin interrumpir el flujo de desarrollo. 

Página oficial de Visual Studio Code: https://code.visualstudio.com/

Página oficial de Flutter: https://flutter.dev/ 

Página oficial de Dart: https://dart.dev/ 

Página de guía y seguimiento para el modelo del Material Design: https://m3.material.io/

---

**Software Deployment**: Esta sección se centra en las herramientas y aplicaciones necesarias para llevar a cabo el despliegue e implementación efectiva de la Landing Page desarrollada a lo largo del ciclo de vida del proyecto. Los recursos seleccionados deben ser fáciles de usar y ofrecer alta confiabilidad para garantizar que el backend se implemente sin problemas de rendimiento o inconsistencias en su funcionamiento. 

- Despliegue del Backend: Se optará por utilizar los propios servicios proporcionados por la página de GitHub Pages, que proporcionan un entorno robusto y confiable para alojar aplicaciones. Estas plataformas ofrecen rendimiento y escalabilidad en tiempo real, lo que asegura que el frontend pueda manejar las demandas del sistema de manera eficiente. Además, su facilidad de configuración y despliegue automatizado contribuye a un proceso de implementación fluido y seguro.

Página oficial de GitHub Pages: https://pages.github.com/

---

**Software Document**: Esta sección detalla las herramientas y aplicaciones seleccionadas para la documentación exhaustiva del código y del software a lo largo del ciclo de vida del proyecto. Las herramientas deben ser intuitivas para todos los miembros del equipo y capaces de gestionar documentación extensa, con soporte para imágenes y una estructura de secciones clara y organizada.

- Documentación del proceso e informe de software: Se utilizará un repositorio en GitHub, estructurado en múltiples ramas según las necesidades del equipo. La redacción de la documentación se llevará a cabo principalmente en Markdown, lo que garantiza una visualización coherente en la web a través de diferentes dispositivos, además de facilitar la compresión y el cifrado de los datos. En situaciones donde Markdown no sea suficiente, como para la creación de tablas complejas, se empleará HTML para lograr una representación más precisa y detallada.

Página oficial de GitHub: https://github.com/

Guía de uso de Markdown: https://www.markdownguide.org/

Guía y seguimiento para HTML5: https://www.w3schools.com/html/

### 5.1.2. Source Code Management.

En esta sección, se definirá la estrategia para utilizar GitHub como plataforma de control de versiones y colaboración durante el ciclo de vida del desarrollo del frontend. Se emplearán todas las herramientas proporcionadas por GitHub para garantizar una gestión eficaz del código fuente, incluyendo el seguimiento de versiones y la colaboración entre miembros del equipo. Se mantendrá un registro exhaustivo de las versiones del frontend, permitiendo rastrear cambios, identificar nuevos desarrollos y corregir errores de manera precisa.

Se establecerán ramas específicas para diferentes etapas del desarrollo, tales como la integración continua, las pruebas y la producción. Además, se implementarán políticas de pull requests y revisiones de código para asegurar la calidad y coherencia del frontend. Esta metodología permitirá un control riguroso del ciclo de vida del desarrollo, facilitando la colaboración y asegurando que todos los cambios se registren de forma clara y ordenada.

**Repositorios en GitHub:**

A continuación, se proporciona una lista con los enlaces a la organización de GitHub de WHAI y a los repositorios específicos relacionados con el desarrollo del frontend dentro de esta organización:

- Repositorio principal de la organización de Roademics: https://github.com/GRUPO-3-MOVILES 

- Repositorio del reporte y documentación: https://github.com/GRUPO-3-MOVILES/upc-pre-202402-cc-238-WV61-WeHaveAnIdea-report 

- Repositorio con todo el código correspondiente a la Aplicación Móvil de Roademics: https://github.com/GRUPO-3-MOVILES/upc-pre-202402-cc-238-WV61-WeHaveAnIdea-MobileApplication

- Repositorio con todo el código correspondiente a la Landing Page de Roademics: https://github.com/GRUPO-3-MOVILES/upc-pre-202402-cc-238-WV61-WeHaveAnIdea-landingPage 

Asimismo, se brinda un enlace a todos los puntos desplegados de la aplicación por el lado del BackEnd:

Enlace del punto de visualización de Swagger del BackEnd de Roademics: https://wehaveidea-production.up.railway.app/swagger-ui/index.html#/

**Integrantes de la organización**:
En esta sección, se presentarán todos los usuarios que forman parte de la organización de GitHub del proyecto WHAI, junto con sus nombres de usuario correspondientes. El objetivo es evitar confusiones sobre los autores de los commits en GitHub y facilitar la identificación de los colaboradores al revisar y analizar el reporte y el código desarrollado por nuestro equipo.

###### Tabla 23.

*Modelo de integrantes del equipo dentro de la página de organización de Github*

|**Nombre de Usuario**|**Imagen de Perfil**|**Nombre del Integrante del Equipo**|
| ----- | ------ | ----- |
| JuanPescoran | <img src="/assets/img/capitulo-5/github-profiles/juan-pescoran-angulo-github-profile.png" alt="Imagen de perfil de Github del integrante Pescorán Angulo, Juan Fabritzzio">| Pescorán Angulo, Juan Fabritzzio - U20221C936 |
| FlavioTrigueros | <img src="/assets/img/capitulo-5/github-profiles/flavio-trigueros-chumacero-github-profile.png" alt="Imagen de perfil de Github del integrante Trigueros Chumacero, Flavio Eduardo"> | Trigueros Chumacero, Flavio Eduardo - U202210190 |
| AldhaValenzuelaH | <img src="/assets/img/capitulo-5/github-profiles/aldhair-valenzuela-huillcaya-github-profile.png" alt="Imagen de perfil de Github del integrante Valenzuela Huillcaya, Aldhair Johan Juan"> | Valenzuela Huillcaya, Aldhair Johan Juan - U20201F572 |
| LucioY250 | <img src="/assets/img/capitulo-5/github-profiles/lucio-yen-cerna-github-profile.png" alt="Imagen de perfil de Github del integrante Yen Cerna, Lucio Heli"> | Yen Cerna, Lucio Heli - U202213143 |

**GitFlow Workflow**:

En nuestro proyecto, implementaremos el modelo GitFlow para el control de versiones, el cual está estructurado en torno a ramas principales y secundarias. Las ramas principales actúan como las bases fundamentales para el desarrollo y la implementación final del frontend. La rama master representa la versión estable y en producción, mientras que develop se utiliza para integrar todas las características y correcciones que se encuentran en desarrollo.

Las ramas secundarias se utilizan para gestionar desarrollos específicos y modificaciones puntuales. Estas ramas se crean para el desarrollo de nuevas funcionalidades, para abordar errores críticos en producción y para preparar la versión para su liberación final. Cada una de estas ramas se fusiona con develop a través de pull requests, los cuales son revisados por el equipo para asegurar la calidad y coherencia del código. Este enfoque asegura que cada cambio se maneje de manera organizada y que los errores críticos se aborden de forma eficiente, manteniendo la estabilidad del proyecto en todo momento.

Esta metodología garantiza una organización efectiva del flujo de trabajo, facilita la colaboración entre los miembros del equipo y optimiza la gestión de versiones del frontend, asegurando que todos los cambios se integren de manera controlada y que el historial del proyecto sea claro y manejable. A continuación, se detallan las convenciones para nombrar las ramas dentro de nuestra organización:

**Ramas Principales**:

- `master`: Esta rama contiene la versión final y estable del frontend, lista para su despliegue en el entorno de producción. Las integraciones a esta rama deben pasar por una revisión exhaustiva por parte del equipo técnico para asegurar la calidad y estabilidad del código del frontend.
  
- `develop`: Esta rama agrupa los elementos en desarrollo relacionados con el frontend, que han sido aprobados por al menos un miembro del equipo diferente del autor de las modificaciones. Sirve como etapa de integración y prueba de nuevas funcionalidades del frontend antes de ser fusionadas con `master`.

**Ramas de Funcionalidades (Feature Branches)**:

###### Tabla 24.

*Modelo de todas las ramas implementadas dentro de la organización del proyecto en Github.*

| Nombre | Descripción |
|--------|-------------|
| feat/iam | Gestiona los cambios relacionados con la implementación del sistema de gestión de identidades y accesos (IAM) en el backend. Esta implementación asegura la autenticación, autorización y control de permisos de usuarios, garantizando la seguridad del sistema y un acceso adecuado a los recursos según los roles asignados. |
| feat/roadmaps | Agrupa los cambios correspondientes a la gestión de los roadmaps en el backend, incluyendo la lógica para la creación, almacenamiento y procesamiento de los datos relacionados con los roadmaps de los usuarios. Esto abarca la implementación de endpoints para la manipulación de datos, así como la optimización de consultas y almacenamiento en la base de datos para asegurar un rendimiento eficiente. |

**Ramas Individuales**: Estas ramas se utilizan para desarrollos individuales realizados por los miembros del equipo en el frontend. Los cambios se integran a las ramas principales mediante pull requests, que deben ser aprobados por el líder del equipo. Una vez que los cambios han sido completados y fusionados, estas ramas se eliminan para evitar la acumulación innecesaria de ramas y mantener un repositorio limpio y organizado.

---

Para asegurar una convención clara y coherente en el nombramiento de ramas, así como en los modelos de pull requests y commits realizados por los miembros del equipo de frontend, hemos establecido el siguiente formato estándar:

Formato de Commit:

|feat(branch): verb + brief description in English|
|-------------------------------------------------|

En este formato, "branch" debe indicar la rama en la que se han realizado los cambios propuestos para una nueva funcionalidad del backend. La descripción debe estar escrita en inglés y comenzar con un verbo que refleje claramente la naturaleza del cambio implementado. A continuación, se presenta una tabla con verbos recomendados para los mensajes de commit:

###### Tabla 25
*Modelo de escritura de verbos para todos los commits realizados en el proyecto de Github*

| Verbo | Traducción | Uso en el proyecto de programación |
|-------|------------|------------------------------------|
|Add  |Añadir  | Utilizado para añadir nuevas funcionalidades, componentes o módulos al frontend. Ideal para commits en los que se implementan nuevas vistas, estilos o scripts, incrementando la capacidad del sistema sin afectar las funcionalidades existentes.  |
|Create  |Crear  | Empleado para la creación de nuevos componentes, estilos o rutas en la aplicación frontend. Este verbo se usa cuando se inicia el desarrollo de una nueva característica o diseño dentro del sistema, estableciendo la base técnica sobre la cual se expandirá la funcionalidad. |
|Update  |Actualizar  | Usado para realizar modificaciones menores en las funcionalidades existentes del frontend, como la actualización de estilos, optimización de scripts o ajustes en la lógica de interacción. Se aplica en casos donde los cambios no alteran significativamente la estructura, pero mejoran el rendimiento o corrigen comportamientos. |
|Modify  |Modificar  | Aplicado cuando se realizan cambios significativos en la lógica del frontend, como la reestructuración de componentes o la implementación de nuevas políticas de diseño en la capa de presentación. Esto incluye cambios que afectan la arquitectura general o que impactan directamente en la interacción entre componentes. |
|Correct  | Corregir  | Utilizado para corregir errores menores en la implementación del frontend, como ajustes en las validaciones de formularios, corrección de rutas de navegación, o fallos en configuraciones que afectan el correcto funcionamiento de la interfaz. Este verbo se reserva para pequeñas correcciones sin grandes implicaciones. |
|Fix  |Arreglar  | Usado para solucionar bugs críticos o problemas que afectan directamente la funcionalidad del frontend. Esto puede incluir arreglar errores en la lógica de interacción, problemas de visualización o fallos en la autenticación de usuarios. También es comúnmente utilizado para resolver errores en la integración continua o el despliegue automático. |
|Delete  |Borrar  | Aplicado para la eliminación de componentes, estilos o recursos que ya no son necesarios en el frontend. Debe utilizarse cuando se elimina código obsoleto o componentes que han sido reemplazados por implementaciones más eficientes o actualizadas. |
|Drop  |Tirar  | Exclusivo para la eliminación de rutas, estilos o configuraciones en el frontend. Debe ser utilizado con precaución, ya que este tipo de cambios puede tener implicaciones críticas en la presentación de datos y la estructura general de la interfaz. Suele aplicarse cuando se reorganiza o limpia el sistema de archivos en el proceso de migración o refactorización. |

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

### 5.1.3. Source Code Style Guide & Conventions.

En esta sección, nuestro equipo explicará y establecerá las referencias que adoptaremos para nombrar, estructurar, organizar y programar en los lenguajes de programación que se utilizarán en el desarrollo de nuestra solución de software, con un enfoque exclusivo en la implementación del frontend. Se detallarán las convenciones y mejores prácticas que se seguirán para asegurar un código coherente y eficiente en el uso de Flutter, Dart, CSS, HTML y JavaScript, que son las principales herramientas del proyecto. Estas convenciones de codificación garantizarán la claridad, mantenibilidad y escalabilidad del código, facilitando la colaboración entre los diferentes miembros del equipo de desarrollo frontend.

Asimismo, también investigaremos y presentaremos las directrices para la interacción con las interfaces de usuario y la implementación de una experiencia de usuario fluida y atractiva. Esto incluirá la gestión adecuada de los componentes visuales, la optimización del rendimiento en la renderización y el manejo efectivo de la interacción del usuario con la aplicación:

- Guía de Estilos y Convenciones de Codigo para HTML: https://www.w3schools.com/html/html5_syntax.asp 
- Guía de Estilos de Google para HTML Y CSS: https://google.github.io/styleguide/htmlcssguide.html 
- Convenciones de Gherkin para especificaciones legibles: https://specflow.org/gherkin/gherkin-conventions-for-readable-specifications/ 
- Guía de Google para el Estilo de JavaScript: https://google.github.io/styleguide/jsguide.html
- Guía de Pautas de Javascript de MDN (Mozilla): https://developer.mozilla.org/en-US/docs/MDN/Writing_guidelines/Writing_style_guide/Code_style_guide/JavaScript
- Guía de Estilos de Javascript del consorcio W3: https://www.w3schools.com/js/js_conventions.asp
- Guía Oficial del Framework de Flutter: https://docs.flutter.dev/get-started/learn-flutter
- Conjunto de Datos con Recursos de Aprendizaje de Flutter: https://github.com/rafathefull/flutterverso
- Guía Oficial de Dart: https://dart.dev/language
- Guía de Librerías Oficiales de Dart: https://dart.dev/libraries

#### Convenciones que Usaremos:

**HTML:**

- Estructura Semántica: Al construir una página web, es crucial utilizar etiquetas HTML semánticas que reflejen el significado del contenido. Las etiquetas como `<header>`, `<footer>`, `<article>`, `<section>`, y `<aside>` no solo mejoran la accesibilidad para tecnologías de asistencia, sino que también ayudan a los motores de búsqueda a comprender mejor la estructura de la página. Esto permite que los desarrolladores mantengan un código más limpio y comprensible, facilitando futuras modificaciones y la colaboración entre diferentes equipos. Al emplear etiquetas semánticas, se promueve una estructura lógica y ordenada que mejora la experiencia del usuario y optimiza el SEO.
  
- Uso de Atributos "Alt" en Imágenes: Cada vez que se utilicen imágenes en una página web, es fundamental incluir el atributo "alt" en la etiqueta `<img>`. Este atributo proporciona una descripción textual de la imagen, lo que es esencial para la accesibilidad, ya que permite a los lectores de pantalla transmitir información sobre el contenido visual a personas con discapacidades visuales. Además, el texto alternativo también actúa como un indicador para los motores de búsqueda, mejorando el SEO. Es recomendable que el contenido del atributo "alt" sea breve y descriptivo, evitando frases genéricas como "imagen de" y enfocándose en el contexto que aporta la imagen a la página.

- Uso Adecuado de Encabezados: La jerarquía de encabezados en HTML es fundamental para estructurar el contenido de manera lógica y accesible. Se debe utilizar la etiqueta `<h1>` para el título principal de la página, seguido por `<h2>`, `<h3>`, y así sucesivamente, para subsecciones. Esto no solo ayuda a los usuarios a escanear el contenido rápidamente, sino que también facilita a los motores de búsqueda rastrear la estructura del contenido, mejorando la indexación y el SEO. Es importante evitar saltar niveles de encabezados porque esto puede confundir a los lectores y desorganizar la estructura semántica de la página.

- Validación del Código HTML: Realizar una validación del código HTML es una práctica esencial para garantizar que la página se renderice correctamente en todos los navegadores. Utilizar herramientas como el validador de HTML del W3C permite identificar errores y advertencias en el código que pueden causar problemas de visualización o accesibilidad. La validación no solo mejora la calidad del código, sino que también asegura que se sigan las especificaciones HTML, lo que es crucial para el mantenimiento a largo plazo del proyecto. Un código bien validado también puede aumentar la confianza del usuario en la calidad del contenido que se presenta.

- Evitar Inline CSS y JavaScript: Es recomendable evitar el uso de estilos y scripts en línea directamente en las etiquetas HTML, optando en su lugar por archivos CSS y JavaScript externos. Esta práctica mejora la organización del código, ya que separa la estructura del contenido de su presentación y funcionalidad. Al tener hojas de estilo y archivos de scripts separados, se facilita la reutilización del código, la gestión y el mantenimiento a medida que el proyecto crece. Además, cargar archivos CSS y JavaScript de manera externa permite a los navegadores cachear estos recursos, mejorando el tiempo de carga de la página y la experiencia del usuario.

- Comentarios Claros y Concisos: Incluir comentarios en el código HTML es una práctica valiosa que facilita la comprensión del propósito y la funcionalidad de secciones específicas del código. Los comentarios deben ser claros y concisos, explicando qué hace un bloque de código o por qué se implementó de cierta manera. Esto es especialmente útil en equipos de desarrollo donde múltiples personas trabajan en el mismo proyecto, ya que permite a los miembros del equipo comprender rápidamente las decisiones tomadas por otros. Sin embargo, es importante no abusar de los comentarios; el código debe ser lo suficientemente claro para que, en muchos casos, no se necesiten explicaciones adicionales.
  
- Uso de Clases y IDs Descriptivos: Al asignar clases e identificadores a los elementos HTML, es fundamental utilizar nombres descriptivos que reflejen la función o el contenido del elemento. Esto no solo facilita la comprensión del código, sino que también mejora la mantenibilidad y el trabajo en equipo, ya que otros desarrolladores pueden entender fácilmente la finalidad de cada clase o ID sin necesidad de un contexto adicional. Además, los nombres descriptivos son especialmente útiles cuando se trabaja con JavaScript y CSS, permitiendo a los desarrolladores aplicar estilos y comportamientos de manera más efectiva. Se recomienda seguir una convención de nomenclatura coherente, como BEM (Block Element Modifier), para asegurar uniformidad en todo el proyecto.

- Mantenimiento de la Accesibilidad: La accesibilidad es un aspecto fundamental en el desarrollo web, y al crear HTML, se deben implementar prácticas que aseguren que el contenido sea accesible para todos los usuarios, independientemente de sus habilidades. Esto incluye el uso de etiquetas adecuadas, como `<label>` para formularios, la inclusión de atributos ARIA cuando sea necesario y el cumplimiento de los estándares de accesibilidad como WCAG. También es esencial realizar pruebas de accesibilidad utilizando herramientas y tecnologías de asistencia para garantizar que el contenido sea legible y utilizable por personas con discapacidades. Al priorizar la accesibilidad, no solo se cumple con las normativas legales, sino que también se mejora la experiencia del usuario y se amplía el alcance del contenido.

- Evitación de Elementos Obsoletos: A medida que el estándar HTML evoluciona, ciertos elementos se vuelven obsoletos y deben ser evitados en el desarrollo de nuevas páginas web. Por ejemplo, elementos como `<font>` y `<center>` han sido reemplazados por CSS, y su uso puede causar problemas de compatibilidad con navegadores modernos y disminuir la mantenibilidad del código. Al mantenerse al día con las mejores prácticas y las especificaciones actuales de HTML, los desarrolladores garantizan que su código sea limpio, moderno y compatible con futuras actualizaciones. Es recomendable consultar las especificaciones del W3C para conocer qué elementos están obsoletos y cuáles son las alternativas recomendadas.

- Minimización de Redundancias: La redundancia en el código HTML puede llevar a un aumento innecesario del tamaño de la página y dificultar su mantenimiento. Se debe buscar evitar la duplicación de elementos y atributos, utilizando listas, clases y componentes reutilizables en su lugar. Al reducir la redundancia, se mejora la legibilidad del código y se optimiza el rendimiento de la página, lo que es crucial para una buena experiencia del usuario. Además, al tener un código más limpio y menos redundante, se facilita la colaboración entre desarrolladores, ya que es más fácil entender y trabajar con un código bien organizado. Implementar un enfoque de diseño modular también puede contribuir a la reducción de redundancias y a una mejor estructura del proyecto.
  
**CSS**:

- Estructura Modular y Organizativa: Al escribir CSS, es fundamental adoptar una estructura modular que facilite la organización y el mantenimiento del código. Esto se puede lograr mediante la división de archivos CSS en módulos o componentes, donde cada archivo o sección esté dedicado a un aspecto específico de la interfaz de usuario, como botones, formularios o elementos de navegación. Esta metodología no solo mejora la claridad del código, sino que también facilita la reutilización de estilos en diferentes partes del proyecto. Al implementar esta estructura, los desarrolladores pueden trabajar de manera más eficiente y reducir el tiempo dedicado a realizar modificaciones en el futuro, ya que las reglas de estilo están claramente organizadas y categorizadas.

- Uso de Nombres Descriptivos en Clases: Es esencial utilizar nombres descriptivos y coherentes al definir clases en CSS. Un buen nombre de clase debe reflejar la función o el propósito del elemento que estiliza, facilitando así la comprensión del código tanto para el autor original como para otros desarrolladores que puedan trabajar en el mismo proyecto. Adoptar una convención de nomenclatura, como BEM (Block Element Modifier), puede ser extremadamente útil en este sentido, ya que proporciona un marco claro para nombrar clases de manera estructurada y coherente. Esto no solo mejora la legibilidad del código, sino que también facilita la búsqueda y la modificación de estilos específicos en el futuro.

- Uso Eficiente de Selectores: Al escribir CSS, es importante utilizar selectores de manera eficiente para evitar la sobreespecificación y garantizar que el estilo se aplique correctamente. Se recomienda limitar el uso de selectores de ID y evitar el uso excesivo de selectores descendentes complejos, ya que esto puede hacer que el código sea menos mantenible y más difícil de entender. En su lugar, se debe optar por selectores de clase que sean más flexibles y reutilizables. Además, el uso de combinaciones de selectores, como combinadores y pseudo-clases, puede ayudar a mantener el código limpio y organizado, permitiendo que los estilos se apliquen de manera efectiva sin redundancias innecesarias.

- Incorporación de Comentarios Claros: Incluir comentarios en el código CSS es una práctica valiosa que permite a los desarrolladores explicar el propósito de ciertos estilos o agrupaciones de reglas. Esto es especialmente útil en proyectos grandes donde múltiples desarrolladores pueden estar trabajando en diferentes secciones del código. Los comentarios deben ser claros y concisos, proporcionando contexto sobre por qué se aplican ciertos estilos o cómo interactúan con otros elementos en la página. Sin embargo, es importante no abusar de los comentarios; el objetivo es que el código sea lo suficientemente claro para que no se necesiten explicaciones extensas. Al proporcionar comentarios adecuados, se mejora la comprensión y la mantenibilidad del código a lo largo del tiempo.

- Uso de Variables y Preprocesadores: La utilización de variables y preprocesadores CSS, como SASS o LESS, puede mejorar significativamente la mantenibilidad y la escalabilidad del código. Al definir variables para colores, fuentes, y tamaños en un solo lugar, se facilita la gestión de estilos en todo el proyecto, permitiendo cambios rápidos y coherentes sin necesidad de buscar y reemplazar valores en múltiples lugares. Esto no solo ahorra tiempo, sino que también reduce la posibilidad de errores. Los preprocesadores también permiten el uso de anidamiento y mixins, lo que contribuye a la organización del código y mejora la legibilidad. Adoptar esta práctica puede resultar en un CSS más limpio y modular, ideal para proyectos de mayor envergadura.

- Consistencia en Espaciado y Alineación: Mantener una consistencia en el espaciado y la alineación de los elementos es crucial para lograr una presentación visual armoniosa. Se recomienda establecer un sistema de espaciado, como un espacio base o una escala de espaciado, que se aplique de manera uniforme a lo largo del proyecto. Utilizar unidades relativas, como `rem` o `em`, en lugar de píxeles permite una mejor adaptabilidad en diferentes dispositivos y resoluciones. Además, aplicar un enfoque coherente para la alineación de textos y elementos contribuye a una experiencia de usuario más fluida y agradable. Al seguir estas prácticas, se mejora no solo la estética de la interfaz, sino también la usabilidad general del sitio.
  
- Optimización del Rendimiento CSS: La optimización del rendimiento es una consideración importante al escribir CSS, ya que un código ineficiente puede afectar negativamente la velocidad de carga y la experiencia del usuario. Para optimizar el rendimiento, se recomienda reducir el uso de selectores complejos y evitar el uso excesivo de propiedades que requieran reflujo o repintado, como `box-shadow` y `opacity`. Además, la minificación del código CSS antes de su despliegue puede reducir el tamaño del archivo y mejorar los tiempos de carga. Utilizar herramientas de análisis de rendimiento, como Lighthouse, puede ayudar a identificar áreas de mejora y garantizar que el CSS esté optimizado para un rendimiento óptimo.

- Evitar el Uso de !important: Aunque el uso de la declaración `!important` puede parecer una solución rápida para resolver problemas de sobreespecificación, su uso excesivo puede llevar a un código difícil de mantener y depurar. En su lugar, se recomienda estructurar el CSS de tal manera que se eviten los conflictos de estilo mediante una adecuada jerarquía de selectores y un diseño modular. Si se encuentra la necesidad de utilizar `!important`, es fundamental reconsiderar la estructura del CSS y determinar si hay una forma más limpia de alcanzar el mismo resultado. Al evitar el uso innecesario de `!important`, se promueve un código más limpio y mantenible que es más fácil de comprender y modificar en el futuro.

- Responsividad y Diseño Adaptable: La creación de un diseño responsivo es esencial en la actualidad, dado el creciente uso de dispositivos móviles. Al escribir CSS, se deben emplear técnicas como Media Queries para adaptar los estilos a diferentes tamaños de pantalla y resoluciones. Esto incluye ajustar las propiedades de diseño, como el ancho, la altura y el espaciado, para asegurar que el contenido se presente de manera óptima en todos los dispositivos. Utilizar unidades relativas y un enfoque de diseño fluido también contribuye a crear una experiencia de usuario más flexible y agradable. Al priorizar la responsividad, se mejora la accesibilidad y se asegura que el sitio sea funcional y estéticamente atractivo en cualquier dispositivo.

- Pruebas y Validación del CSS: Realizar pruebas y validaciones regulares del CSS es una práctica esencial para garantizar que todos los estilos se apliquen correctamente y que no existan errores que puedan afectar la experiencia del usuario. Utilizar herramientas de validación de CSS puede ayudar a identificar problemas de sintaxis o propiedades obsoletas que deban ser corregidas. Además, es recomendable probar el sitio en diferentes navegadores y dispositivos para asegurarse de que los estilos se comporten de manera consistente. Al llevar a cabo estas pruebas y validaciones, se mejora la calidad del código y se minimizan los errores, lo que resulta en una experiencia de usuario más fluida y profesional.

**JavaScript:**

- Uso de `let` y `const` en lugar de `var`: Es fundamental adoptar el uso de `let` y `const` para declarar variables en lugar de `var`, ya que esto ayuda a evitar confusiones relacionadas con el alcance de las variables y la hoisting (elevación). `let` permite declarar variables con un alcance de bloque, lo que significa que su visibilidad está limitada al bloque en el que se define, mientras que `const` se utiliza para declarar constantes que no deben cambiar su valor. Al emplear `const` para valores que no se reasignarán, y `let` para aquellos que lo harán, se mejora la claridad del código y se previene la re-declaración accidental de variables. Esta práctica también fomenta un estilo de programación más predecible y controlado, lo cual es vital en proyectos de gran escala.

- Nomenclatura Consistente y Descriptiva: Adoptar una convención de nomenclatura clara y consistente para las variables, funciones y clases es crucial para mantener la legibilidad del código. Los nombres deben ser descriptivos y reflejar claramente la función o el propósito de la variable o función. Esto no solo facilita la comprensión del código, sino que también ayuda a los desarrolladores a identificar rápidamente la funcionalidad sin necesidad de leer toda la implementación. Mantener esta consistencia a lo largo del proyecto asegura que el código sea accesible para todos los miembros del equipo, mejorando así la colaboración y el mantenimiento.
  
- Funciones Puramente Declarativas: Es recomendable escribir funciones que sean puramente declarativas y que no dependan de estados externos. Esto significa que las funciones deben recibir todos los datos necesarios como argumentos y no modificar el estado de las variables externas ni depender de ellas. Al seguir esta práctica, se logra que las funciones sean más predecibles, fáciles de probar y reutilizables. Las funciones puras también permiten un mejor rendimiento y optimización, ya que el compilador puede identificar que no hay efectos secundarios asociados. Esta metodología no solo mejora la calidad del código, sino que también simplifica el proceso de depuración y prueba.
  
- Uso de Promesas y `async/await` para Manejo de Asincronía: Con el creciente uso de operaciones asincrónicas en JavaScript, es crucial emplear Promesas y la sintaxis `async/await` para manejar el flujo asincrónico de manera más legible y controlada. Al utilizar `async/await`, el código se vuelve más fácil de entender, ya que se asemeja a la escritura sincrónica, eliminando la complejidad de las cadenas de Promesas y los callbacks anidados. Esta práctica no solo mejora la claridad del código, sino que también permite un mejor manejo de errores mediante bloques `try/catch`, lo que facilita la detección y resolución de problemas. Implementar esta técnica asegura que el código sea más limpio, comprensible y mantenible.

- Validación de Datos y Manejo de Errores: Es esencial implementar la validación de datos y un adecuado manejo de errores en todas las funciones y métodos que interactúan con entradas externas, como formularios o APIs. Esto implica verificar que los datos recibidos sean del tipo y formato esperados antes de realizar cualquier operación, así como manejar situaciones donde los datos no cumplan con los criterios establecidos. Utilizar bloques `try/catch` para capturar errores y manejar excepciones de manera controlada no solo mejora la robustez de la aplicación, sino que también ofrece una mejor experiencia al usuario al proporcionar mensajes de error claros y útiles. Al seguir esta práctica, se minimizan los errores inesperados y se facilita el diagnóstico y la resolución de problemas.
  
- Modularización del Código: Organizar el código en módulos es una práctica fundamental que facilita la escalabilidad y el mantenimiento de aplicaciones más grandes. Al dividir el código en módulos lógicos, cada uno encargado de una funcionalidad específica, se permite un desarrollo más eficiente y una colaboración más fluida entre los miembros del equipo. Esta modularización puede lograrse utilizando ES6 Modules o herramientas de empaquetado como Webpack o Rollup, que permiten importar y exportar funciones y variables entre diferentes archivos. Esta estructura no solo mejora la organización del código, sino que también promueve la reutilización de componentes, lo que es esencial en el desarrollo ágil y moderno.

- Uso de Comentarios Efectivos: Los comentarios en el código son una herramienta poderosa para facilitar la comprensión y el mantenimiento del mismo. Es fundamental utilizar comentarios efectivos que expliquen la lógica detrás de secciones complejas del código o que proporcionen contexto sobre las decisiones tomadas. Sin embargo, los comentarios deben ser claros y precisos; no deben ser redundantes ni obvios, ya que esto puede llevar a la acumulación de comentarios innecesarios. En lugar de comentar lo que hace el código, es preferible explicar por qué se hace de esa manera. Esta práctica mejora la legibilidad y la claridad del código, ayudando a otros desarrolladores (o al mismo autor en el futuro) a entender rápidamente la lógica sin tener que deducirla de la implementación.
  
- Consistencia en la Formateación del Código: Mantener una consistencia en la formateación del código es vital para mejorar su legibilidad y facilitar el trabajo en equipo. Esto incluye el uso uniforme de espacios, tabulaciones, y convenciones de colocación de llaves y paréntesis. Utilizar herramientas de formateo automático, como Prettier, puede ayudar a asegurar que todo el código siga un estilo común, lo que elimina discrepancias y promueve una mejor colaboración. Además, establecer un estilo de código claro y documentado al inicio del proyecto ayuda a alinear a todos los miembros del equipo y a reducir la posibilidad de conflictos de estilo en el futuro. Esta práctica no solo mejora la apariencia del código, sino que también facilita la revisión y comprensión del mismo.

- Optimización del Rendimiento: La optimización del rendimiento es una consideración clave al escribir JavaScript, especialmente en aplicaciones web donde la velocidad de carga y la interacción del usuario son esenciales. Esto implica evitar la creación de funciones innecesarias dentro de bucles, reducir el uso de operaciones costosas y minimizar el acceso al DOM, que puede ser lento. Además, emplear técnicas como la delegación de eventos puede ayudar a mejorar la eficiencia al reducir el número de escuchadores de eventos en el DOM. Utilizar herramientas de análisis y optimización, como Lighthouse, permite identificar áreas de mejora y garantizar que la aplicación se ejecute de manera fluida. Esta atención al rendimiento asegura que los usuarios tengan una experiencia positiva y que la aplicación funcione de manera eficiente en diversos dispositivos.

- Implementación de Pruebas Automatizadas: La implementación de pruebas automatizadas es una práctica esencial para garantizar la calidad y la funcionalidad del código en JavaScript. Al escribir pruebas unitarias y de integración, se puede verificar que cada parte del código se comporte como se espera, lo que ayuda a detectar errores y regresiones en el futuro. Utilizar frameworks de prueba, como Jest o Mocha, permite ejecutar pruebas de manera sencilla y organizar el código de prueba en módulos. Además, la integración continua y la entrega continua (CI/CD) pueden facilitar la ejecución automática de pruebas en cada cambio, lo que asegura que el código se mantenga en un estado funcional en todo momento. Esta práctica no solo mejora la confiabilidad del software, sino que también contribuye a un proceso de desarrollo más ágil y eficiente.

**Dart:**

- Uso de `final` y `const` en lugar de variables mutables: En Dart, es fundamental hacer uso de `final` y `const` para definir variables cuando se desea que su valor no cambie. La palabra clave `final` permite definir variables que se inicializan una sola vez y no pueden ser modificadas posteriormente, mientras que `const` se utiliza para definir constantes en tiempo de compilación. Utilizar estas palabras clave ayuda a asegurar la inmutabilidad de los valores y a prevenir errores en el código, ya que evita la modificación accidental de variables que deberían permanecer constantes. Esta práctica no solo mejora la claridad del código, sino que también optimiza el rendimiento, ya que Dart puede realizar ciertas optimizaciones cuando sabe que las variables no cambiarán.

- Nomenclatura Clara y Descriptiva: La elección de nombres claros y descriptivos para clases, funciones y variables es esencial para mejorar la legibilidad del código en Dart. Los nombres deben reflejar la intención y el propósito de los elementos del código, lo que permite a otros desarrolladores (o a uno mismo en el futuro) entender rápidamente su funcionalidad. Esta práctica no solo facilita la comprensión y el mantenimiento del código, sino que también fomenta una colaboración más efectiva dentro del equipo, ya que cada miembro puede entender el propósito de cada componente sin necesidad de revisar toda la implementación.

- Evitar el Uso de `dynamic`: En Dart, el tipo `dynamic` permite que una variable tome cualquier tipo de valor, lo que puede llevar a errores en tiempo de ejecución y disminuir la claridad del código. Es recomendable evitar el uso de `dynamic` siempre que sea posible y, en su lugar, utilizar tipos específicos para las variables y parámetros de función. Esto permite que el compilador realice verificaciones de tipo y proporciona una mejor documentación del código al definir claramente qué tipos se esperan en cada contexto. Además, esta práctica mejora la mantenibilidad y la refactorización del código, ya que los desarrolladores pueden identificar fácilmente las relaciones entre tipos y las operaciones permitidas.

- Organización en Módulos y Paquetes: La organización del código en módulos y paquetes es crucial para la escalabilidad y el mantenimiento de aplicaciones en Dart. Al dividir el código en archivos y directorios lógicos, cada uno con una funcionalidad específica, se facilita la colaboración entre miembros del equipo y se mejora la estructura del proyecto. Utilizar la convención de nombres en minúsculas y guiones bajos para nombres de archivos y directorios ayuda a mantener un orden claro y accesible. Esta práctica también permite reutilizar componentes en otros proyectos o secciones de la misma aplicación, lo que ahorra tiempo y esfuerzo en el desarrollo y mejora la coherencia en el uso de funciones y clases.

- Uso de Métodos y Clases de Extensión: Dart permite el uso de métodos y clases de extensión, lo que permite agregar nuevas funcionalidades a las clases existentes sin necesidad de modificar su código original. Esta técnica es útil para mejorar la legibilidad del código y para reutilizar la lógica en diferentes partes de la aplicación. Al crear extensiones, se pueden agrupar métodos relacionados y aplicarlos a tipos específicos, lo que permite una escritura de código más limpia y unificada. Sin embargo, es importante utilizar esta práctica con moderación y no abusar de ella, ya que podría llevar a una confusión si se extienden demasiados tipos sin un propósito claro. Al seguir esta práctica, se fomenta un diseño más flexible y modular en el desarrollo de aplicaciones Dart.

- Implementación de Manejo de Errores: El manejo adecuado de errores es esencial para garantizar que las aplicaciones Dart sean robustas y confiables. Utilizar bloques `try-catch permite capturar excepciones y manejar errores de manera controlada, lo que ayuda a prevenir fallos inesperados en la aplicación. Además, se debe proporcionar información útil al usuario y a los desarrolladores sobre los errores que ocurren, utilizando mensajes claros y descriptivos. Implementar un manejo de errores efectivo no solo mejora la experiencia del usuario, sino que también facilita el diagnóstico y la resolución de problemas durante el desarrollo. Esta práctica asegura que la aplicación se mantenga en un estado funcional y predecible, incluso en situaciones inesperadas.

- Uso de `async` y `await` para Operaciones Asincrónicas: Dart es un lenguaje orientado a la programación asincrónica, y es fundamental utilizar `async` y `await` para manejar operaciones asincrónicas de manera clara y efectiva. Al marcar funciones con `async`, se puede utilizar la palabra clave `await` para esperar el resultado de una operación asincrónica antes de continuar con la ejecución del código. Esta práctica mejora la legibilidad del código y reduce la complejidad asociada con las cadenas de callbacks, permitiendo que el flujo del código sea más fácil de seguir. Al adoptar esta metodología, se minimizan los errores relacionados con la asincronía y se facilita la depuración, lo que resulta en aplicaciones más robustas y confiables.

- Utilización de `pubspec.yaml` para la Gestión de Dependencias: En Dart, el archivo `pubspec.yaml` es fundamental para gestionar las dependencias del proyecto. Es esencial mantener este archivo actualizado y organizado, listando todas las bibliotecas y paquetes necesarios para el proyecto, así como sus versiones específicas. Utilizar un manejo adecuado de las versiones, como las versiones de rango o exactas, garantiza que el proyecto permanezca estable y libre de conflictos de dependencia. Esta práctica no solo facilita la gestión de las bibliotecas utilizadas en el proyecto, sino que también permite a otros desarrolladores entender rápidamente qué recursos son necesarios para ejecutar o desarrollar la aplicación. Mantener una buena documentación dentro del archivo también ayuda a otros miembros del equipo a seguir las convenciones y dependencias utilizadas en el desarrollo.

- Implementación de Pruebas Unitarias y de Integración: Las pruebas son una parte crítica del desarrollo de software, y en Dart, es esencial implementar pruebas unitarias y de integración para garantizar la calidad del código. Utilizar el paquete de pruebas de Dart permite a los desarrolladores escribir pruebas que verifiquen el comportamiento de funciones y métodos individuales, así como la interacción entre diferentes componentes. Al realizar pruebas periódicas, se pueden detectar errores y regresiones antes de que se conviertan en problemas críticos, lo que mejora la confiabilidad del software. Esta práctica fomenta un ciclo de desarrollo más ágil y eficiente, ya que los cambios en el código se pueden implementar con confianza, sabiendo que están respaldados por un conjunto sólido de pruebas.

- Documentación Clara y Consistente: La documentación es un aspecto fundamental del desarrollo en Dart, y es vital proporcionar comentarios claros y consistentes en el código. Utilizar comentarios en línea para explicar partes complejas del código y proporcionar descripciones de funciones, parámetros y clases ayuda a otros desarrolladores a comprender rápidamente la intención y la lógica detrás de la implementación. Dart también ofrece la posibilidad de generar documentación automática a partir de comentarios estructurados, lo que facilita la creación de guías y referencias útiles para otros desarrolladores. Al adoptar esta práctica, se asegura que el código sea accesible y comprensible, mejorando la colaboración y el mantenimiento a largo plazo del proyecto.

**Flutter:**

- Estructura de Proyecto Modular: Al desarrollar aplicaciones con Flutter, es crucial seguir una estructura de proyecto modular que divida la aplicación en componentes lógicos y reutilizables. Esta práctica no solo mejora la legibilidad del código, sino que también facilita la colaboración en equipos grandes, ya que diferentes miembros pueden trabajar en módulos específicos sin interferir con el trabajo de otros. Al organizar el código en directorios claramente definidos, como `lib/models`, `lib/views`, `lib/widgets`, y `lib/services`, se crea un mapa claro de cómo se interconectan los distintos elementos de la aplicación. Esta estructura modular también permite una fácil escalabilidad, ya que se pueden agregar nuevas funcionalidades o realizar refactorizaciones sin afectar el resto del sistema.

- Uso de Widgets Compuestos y Personalizados: Flutter promueve la reutilización de widgets, por lo que es recomendable crear widgets compuestos y personalizados que encapsulen la lógica y la presentación de partes de la interfaz de usuario. En lugar de duplicar código en diferentes partes de la aplicación, se deben diseñar widgets que sean configurables y que se puedan reutilizar en diferentes contextos. Esto no solo reduce el tamaño del código y mejora la mantenibilidad, sino que también asegura que los cambios realizados en un widget se reflejen en todas las instancias donde se utiliza. Además, se pueden aplicar principios de diseño más consistentes en toda la aplicación, mejorando la experiencia del usuario.

- Adopción del Patrón BLoC para Gestión de Estado: La gestión del estado es un aspecto crítico en las aplicaciones de Flutter, y adoptar el patrón BLoC (Business Logic Component) es una buena práctica para separar la lógica de negocio de la interfaz de usuario. Este patrón utiliza flujos de datos (Streams) y eventos para comunicar la información entre la UI y la lógica de negocio, permitiendo una arquitectura más limpia y mantenible. Al emplear BLoC, los desarrolladores pueden mantener el estado de la aplicación de manera eficiente y predecible, facilitando las pruebas y el mantenimiento. Además, esta práctica permite una mejor gestión de las dependencias y una mayor claridad en la forma en que los datos fluyen a través de la aplicación.

- Optimización del Rendimiento con ListViews y Grids: En Flutter, las listas y cuadrículas pueden volverse pesadas si no se optimizan correctamente. Utilizar widgets como `ListView.builder` y `GridView.builder` en lugar de `ListView` o `GridView` convencionales es fundamental para mejorar el rendimiento, especialmente en aplicaciones que muestran grandes volúmenes de datos. Estos constructores crean elementos de lista o cuadrícula de manera perezosa, lo que significa que solo renderizan los elementos visibles en la pantalla en lugar de todos los elementos al mismo tiempo. Esta optimización reduce el uso de memoria y mejora la velocidad de carga, proporcionando una experiencia de usuario más fluida y receptiva.

- Gestión de Rutas con `Navigator` y Rutas Nombradas: Al gestionar la navegación en una aplicación Flutter, es recomendable utilizar el widget `Navigator` junto con rutas nombradas. Este enfoque permite mantener una navegación estructurada y fácil de seguir, lo que es especialmente útil en aplicaciones grandes. Definir rutas en un solo lugar, como en el `MaterialApp`, ayuda a centralizar la configuración de la navegación y a evitar duplicaciones. Este enfoque también facilita la implementación de funcionalidades como el paso de argumentos entre pantallas, la gestión del historial de navegación y la personalización de transiciones entre vistas, mejorando así la experiencia del usuario y la coherencia de la aplicación.

- Uso de `pubspec.yaml` para Gestionar Dependencias: El archivo `pubspec.yaml` es fundamental para la gestión de dependencias en Flutter. Mantener este archivo organizado y documentado es esencial para el éxito del proyecto. Es recomendable especificar las versiones de las dependencias de manera clara y evitar el uso de versiones no especificadas, lo que puede conducir a conflictos en el futuro. Además, se deben eliminar las dependencias que ya no se utilizan, manteniendo el proyecto limpio y optimizado. Este enfoque no solo asegura que la aplicación funcione correctamente, sino que también facilita el trabajo colaborativo, ya que todos los desarrolladores tienen acceso a la misma configuración de dependencias.

- Implementación de Pruebas de Widget y de Integración: Las pruebas son fundamentales para garantizar la calidad del software en Flutter, y es crucial implementar pruebas de widget y de integración. Las pruebas de widget permiten verificar el comportamiento de los widgets individuales en diferentes estados y contextos, asegurando que funcionen como se espera. Por otro lado, las pruebas de integración se utilizan para verificar la interacción entre múltiples widgets y componentes en la aplicación. Implementar un conjunto completo de pruebas desde el inicio del desarrollo no solo ayuda a identificar errores de manera temprana, sino que también mejora la confianza en el proceso de desarrollo, permitiendo a los desarrolladores realizar cambios con mayor seguridad

- Adopción de Temas Globales para Consistencia Visual: Al desarrollar aplicaciones con Flutter, es importante establecer y utilizar un tema global que defina los estilos de la interfaz de usuario, como colores, tipografía y tamaños de fuente. Al definir un tema en el "MaterialApp", se puede asegurar que todos los widgets de la aplicación sigan un estilo coherente, lo que mejora la experiencia del usuario y la identidad de la marca. Esta práctica no solo simplifica la gestión de estilos, sino que también facilita los cambios en la apariencia de la aplicación, ya que cualquier modificación en el tema se refleja en todos los widgets que lo utilizan. Además, esta consistencia visual es clave para crear una interfaz de usuario más atractiva y profesional.

- Documentación y Comentarios Claros: La documentación es esencial para mantener la claridad y la comprensión del código en proyectos de Flutter. Al utilizar comentarios claros y concisos para explicar la lógica de los widgets, las funciones y las clases, se facilita la colaboración y la comprensión del código por parte de otros desarrolladores. Además, Flutter permite generar documentación automática utilizando comentarios de estilo Dart, lo que puede ayudar a crear documentación técnica útil para los usuarios y desarrolladores de la aplicación. Esta práctica no solo mejora la mantenibilidad del proyecto, sino que también fomenta una cultura de codificación responsable y profesional dentro del equipo.

- Adopción de Prácticas de Accesibilidad: La accesibilidad es un aspecto fundamental en el desarrollo de aplicaciones móviles, y es esencial seguir prácticas que aseguren que la aplicación sea utilizable para personas con discapacidades. Utilizar widgets de accesibilidad como "Semantics" en Flutter permite mejorar la experiencia de los usuarios que utilizan tecnologías de asistencia, como lectores de pantalla. Además, es importante probar la aplicación en diferentes dispositivos y entornos para garantizar que la experiencia del usuario sea óptima para todos. Invertir en accesibilidad no solo mejora la usabilidad de la aplicación, sino que también expande el alcance de la misma, permitiendo que más personas la utilicen y disfruten.

### 5.1.4. Software Deployment Configuration.

En esta sección, procederemos a detallar de manera exhaustiva la configuración necesaria para implementar y desplegar nuestra solución, centrándonos específicamente en las áreas del FrontEnd. A lo largo de este análisis, enfatizaremos las mejores prácticas que deben seguirse, así como las herramientas más adecuadas a utilizar y los flujos de trabajo recomendados para garantizar una implementación eficaz y coordinada de ambas partes de nuestra solución. Además, discutiremos cómo cada decisión técnica impacta en la funcionalidad y la experiencia del usuario, proporcionando así un enfoque integral para el desarrollo de nuestras aplicaciones.

**Landing Page:**

Comenzaremos el proceso creando un repositorio en GitHub, que servirá como el almacén centralizado para todos los archivos que componen nuestra página de destino, incluyendo HTML, CSS y JavaScript. Una vez que el repositorio esté establecido, cada miembro del equipo colaborará en su propia rama "feature" para desarrollar distintas características y funcionalidades del Landing Page, garantizando así que cada contribución se realice de manera aislada y organizada. Al finalizar el desarrollo de una característica específica, se procederá a llevar a cabo el proceso de fusión (merge) con la rama "develop". Este proceso de integración es crucial, ya que asegura que la página de destino se mantenga siempre actualizada con las últimas modificaciones y mejoras que se hayan implementado por parte de los miembros del equipo. Para facilitar esta integración, se recomienda que se realicen revisiones de código y pruebas antes de completar el merge, lo que contribuirá a mantener la calidad del código y a detectar posibles conflictos o errores en etapas tempranas.

Posteriormente, configuraremos GitHub Pages para que publique automáticamente la página de destino utilizando la rama "develop". Este paso es fundamental, ya que permitirá que nuestra Landing Page sea accesible públicamente, facilitando su visualización y prueba por parte de los interesados y usuarios finales. Esta configuración no solo simplifica el proceso de despliegue, sino que también proporciona un enlace directo que puede compartirse fácilmente con el equipo y las partes interesadas, permitiendo una retroalimentación más rápida y eficiente.

A continuación, proporcionaremos una descripción detallada de los pasos necesarios para llevar a cabo este proceso de despliegue en GitHub Pages. Cada uno de estos pasos se elaborará con suficiente profundidad para asegurar una implementación eficiente y sin contratiempos de nuestra solución, destacando las mejores prácticas y consideraciones técnicas que deberán tenerse en cuenta a lo largo del proceso. Con esta guía, buscamos garantizar que el equipo esté alineado y preparado para llevar a cabo una implementación exitosa del Landing Page.

1. El primer paso en nuestro proceso de despliegue es la creación de un repositorio público en GitHub. Para ello, asignaremos un nombre adecuado al repositorio que refleje el propósito y contenido de nuestra página de destino. Una vez creado el repositorio, procederemos a añadir los archivos necesarios para la construcción y funcionamiento del Landing Page. Es fundamental seleccionar un nombre significativo que identifique claramente el propósito del repositorio y la naturaleza de los archivos que contendrá. Esto facilitará la gestión y colaboración en el desarrollo del proyecto, asegurando que todos los miembros del equipo puedan identificar y acceder al repositorio de manera eficiente. Una vez completada esta tarea, estaremos listos para iniciar el proceso de desarrollo y construcción de nuestro Landing Page, utilizando el repositorio recién creado como punto de partida. Este enfoque nos proporcionará una base sólida y organizada desde la cual avanzar en el desarrollo de nuestra solución.

    ###### Figura ##
    *Imagen de presentación del nuevo repositorio creado y designado en Github para la Landing Page de Roademics*
    <img src="/assets/img/capitulo-5/deployments/deployment-landing-page-image1-repository.png" alt="Nuevo repositorio creado y designado en Github para la Landing Page.">

2. El segundo paso implica dirigirse a la sección de ajustes en GitHub y seleccionar la pestaña Pages. Una vez allí, podremos acceder a las configuraciones relacionadas con la publicación de páginas web directamente desde nuestro repositorio. Esta acción nos permitirá habilitar la funcionalidad de GitHub Pages para nuestro repositorio, lo que nos permitirá alojar y publicar nuestro Landing Page de forma rápida y sencilla. La pestaña Pages ofrece una interfaz intuitiva que nos guiará a través del proceso de configuración, permitiéndonos personalizar diversos aspectos de nuestra página web, como la rama a utilizar para el despliegue y el dominio personalizado, si así lo deseamos. Al acceder a esta sección y realizar las configuraciones necesarias, estaremos un paso más cerca de hacer que nuestro Landing Page esté disponible públicamente para su visualización y acceso por parte de los usuarios finales

    ###### Figura ##
    *Imagen de presentación de la sección de ajustes del nuevo repositorio designado para la Landing Page de Roademics*
    <img src="/assets/img/capitulo-5/deployments/deployment-landing-page-image2-settings-section.png" alt="Sección de ajustes del nuevo repositorio designado para la Landing Page.">

    ###### Figura ##
    *Imagen de presentación de la pestaña Pages en la sección de ajustes del nuevo repositorio designado para la Landing Page de Roademics*
    <img src="/assets/img/capitulo-5/deployments/deployment-landing-page-image3-pages-section.png" alt="Pestaña Pages en la sección de ajustes del nuevo repositorio designado para la Landing Page.">

3. El tercer paso implica dirigirnos al apartado de configuración específico para GitHub Pages en nuestro repositorio. Una vez en esta sección, podremos ajustar diferentes aspectos relacionados con la publicación de nuestro sitio web, como la rama a utilizar, el directorio desde el que se servirán los archivos, y otras opciones de configuración avanzadas. Esta parte del proceso nos brinda la oportunidad de personalizar aún más la forma en que nuestra página web será desplegada y accesible para los usuarios finales. Por ejemplo, podemos seleccionar la rama específica que contiene los archivos de nuestro Landing Page y especificar el directorio raíz desde el cual se servirán los archivos HTML, CSS y JavaScript.

    ###### Figura ##
    *Imagen de presentación del apartado de configuración específico para Github Pages en la sección de ajustes del nuevo repositorio designado para la Landing Page de Roademics.*
    <img src="/assets/img/capitulo-5/deployments/deployment-landing-page-image4-github-pages.png" alt="Apartado de configuración específico para Github Pages en la sección de ajustes del nuevo repositorio designado para la Landing Page.">

4. El cuarto paso implica dirigirse al apartado de "branch" dentro de la configuración de GitHub Pages y seleccionar el branch "main" donde se realizará el despliegue del Landing Page. Es importante asegurarse de elegir el branch correcto donde se encuentran los archivos actualizados de nuestra página web para garantizar que la versión más reciente se despliegue correctamente. Durante este proceso, es recomendable dejar las demás configuraciones con sus valores predeterminados, a menos que tengamos necesidades específicas que requieran ajustes adicionales. Mantener estas configuraciones en sus valores predeterminados ayuda a simplificar el proceso y reduce la posibilidad de errores durante el despliegue.

5. Una vez seleccionada la rama correspondiente, se generará un enlace que permitirá acceder al Landing Page desplegado. Este enlace proporciona una forma rápida y sencilla para que los usuarios accedan a nuestra página web y puedan interactuar con su contenido. Es importante tener en cuenta que cualquier modificación realizada en el branch "main" se actualizará automáticamente en el Landing Page desplegado. Esto significa que cualquier cambio que realicemos en nuestros archivos HTML, CSS o JavaScript se reflejará de inmediato en la versión en vivo de nuestra página web. Este proceso de actualización automática garantiza que nuestro Landing Page esté siempre sincronizado con las últimas modificaciones realizadas en el código fuente, lo que proporciona una experiencia consistente y actualizada para los usuarios que acceden a nuestra página web."

    ###### Figura ##
    *Imagen de presentación del enlace generado en Github Pages en la sección de ajustes para la Landing Page de Roademics.*
    <img src="/assets/img/capitulo-5/deployments/deployment-landing-page-image5-link.png" alt="Enlace generado en Github Pages en la sección de ajustes para la Landing Page.">

6. Una vez completados los pasos anteriores, el Landing Page estará desplegado y listo para ser visualizado y utilizado. Los usuarios podrán acceder al enlace generado y explorar el contenido de nuestra página web. Es importante realizar pruebas adicionales después del despliegue para asegurarse de que la página web se vea y funcione correctamente en diferentes dispositivos y navegadores. Esto garantizará una experiencia de usuario óptima para todos los visitantes de nuestro sitio. En caso los lectores quieran revisar el link desplegado de la Landing Page de Roademics de forma directa y rápida, pueden usar el siguiente enlace: https://grupo-3-moviles.github.io/upc-pre-202402-cc-238-WV61-WeHaveAnIdea-landingPage/   

## 5.2. Software Development & Implementation.

A continuación, describimos en detalle el enfoque técnico que adoptaremos para la implementación, pruebas y despliegue de nuestra infraestructura FrontEnd, centrado en la creación y gestión de los componentes de la interfaz de usuario, así como en la integración con los servicios externos y el manejo eficiente de las API necesarias para el correcto funcionamiento de la aplicación. Este proceso abarca el desarrollo de interfaces FrontEnd escalables, el diseño de la Landing Page, la validación exhaustiva mediante pruebas unitarias y de integración, y la optimización del rendimiento antes de cada ciclo de despliegue en el entorno de producción. Durante esta fase, nos aseguraremos de que cada componente se alinee con las mejores prácticas de desarrollo y diseño, garantizando así una experiencia de usuario fluida y atractiva. Además, se prestará especial atención a la accesibilidad y la compatibilidad en diferentes navegadores, asegurando que nuestra aplicación sea inclusiva y utilizable por la mayor cantidad de usuarios posible.

### 5.2.1. Sprint 1

En esta sección, se registrará y explicará el avance en términos de producto y trabajo colaborativo correspondiente al Sprint número 1 de la Implementación del FrontEnd. Este registro detallado documentará cada aspecto del progreso logrado, incluyendo el desarrollo de la interfaz para el registro de usuarios e inicio de sesión adecuado, además del desarrollo final del diseño de la Landing Page. Se hará hincapié en la importancia de la colaboración y la comunicación efectiva entre los miembros del equipo para alcanzar los objetivos del sprint, destacando cómo cada aportación individual contribuye al éxito colectivo del proyecto.

Todas las especificaciones y resultados presentados en esta sección se derivan del Product Backlog establecido en el Capítulo 2, en la sección de requerimientos. Este alineamiento garantiza que los desarrollos realizados durante el sprint sean consistentes con las expectativas del proyecto y contribuyan a la visión general del producto, asegurando que la interfaz cumpla con los estándares de calidad y usabilidad deseados.

#### 5.2.1.1 Sprint Planning 1.

En esta sección se explicarán los detalles presentados y analizados durante la reunión del Sprint Planning para el Sprint número 1 de la implementación del FrontEnd. El objetivo principal de esta reunión es establecer un plan claro y realista que guíe el desarrollo de la interfaz de usuario, identificando las tareas específicas a realizar y comprometiéndose con un conjunto de entregables concretos que contribuyan al avance del proyecto por el lado de las funcionalidades principales de generación y edición de roadmaps. Este enfoque permite asegurar que todos los miembros del equipo tengan una comprensión compartida de los objetivos y las expectativas del sprint, lo que resulta esencial para la coordinación y efectividad en el trabajo colaborativo.

Durante esta reunión, se abordarán las características a desarrollar, los plazos para cada tarea y los criterios de aceptación correspondientes. Además, se fomentará un diálogo abierto entre los integrantes del equipo para identificar posibles desafíos y oportunidades de mejora, asegurando que cada aspecto del desarrollo del FrontEnd esté alineado con las metas del proyecto. 

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
            <td>2024-09-14</td>
        </tr>
          <tr>
            <td>Time</td>
            <td>16:34</td>
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
            <td>Al concluir el Sprint 1, se llevó a cabo la reunión de Sprint Review en la que se evaluó el progreso realizado en el desarrollo del FrontEnd de nuestra aplicación. Durante este sprint, el enfoque principal se centró en la creación de la página de la Landing Page utilizada para Roademics, así como en aspectos esenciales de la propia aplicación, como la generación y edición de roadmaps, así como las secciones de inicio de sesión y registro. <br><br> La reunión fue exitosa en términos de avance en los productos de software y en la colaboración del equipo. Se presentaron las funcionalidades desarrolladas, se realizaron demostraciones de la interfaz de usuario y se recopilaron comentarios constructivos por parte de los miembros del equipo y otros interesados. Este intercambio de opiniones fue invaluable, ya que permitió identificar áreas de mejora y ajustar los planes para el próximo sprint. La colaboración y la comunicación efectiva durante esta revisión reforzaron la cohesión del equipo y garantizaban que el desarrollo del FrontEnd se mantuviera alineado con los objetivos generales del proyecto.</td> 
        </tr>
            <tr>
            <td>Sprint 1 Retrospective Summary</td>
            <td>En el proceso de Sprint Retrospective para el Sprint 1, nuestro equipo se dedicó a revisar detenidamente toda la retroalimentación recibida tras la finalización de este primer sprint. Este análisis exhaustivo del desempeño general e individual de cada miembro del equipo nos permitió identificar áreas clave de mejora que son fundamentales para optimizar nuestra aplicación móvil desde la perspectiva del FrontEnd. <br><br> A través de este proceso reflexivo, se plantearon diversas estrategias destinadas a garantizar la entrega de un trabajo de mayor calidad y un producto que cumpla con las expectativas de nuestros usuarios finales. Se discutieron aspectos relacionados con la usabilidad de la interfaz, la coherencia en el diseño y la implementación de mejores prácticas en el desarrollo del FrontEnd. Este intercambio de ideas no solo fortaleció la colaboración del equipo, sino que también sentó las bases para un enfoque más efectivo en los próximos sprints, asegurando así que nuestro producto no solo sea funcional, sino también intuitivo y atractivo para nuestros clientes. </td>
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
            <td>Con el equipo para este sprint 1 decidimos aceptar 3 Story Points</td>
        </tr>
              <tr>
            <td>Sum of Story Points</td>
            <td>La suma de los Story Points para los User Stories que se están incluyendo en este Sprint 1 es 21</td>
        </tr>
    </table>

#### 5.2.1.2 Sprint Backlog 1.

En esta sección, se revisará exhaustivamente todo el proceso relacionado con el Sprint Backlog número 1, en el cual nuestro equipo de trabajo se centró principalmente en el diseño de la Landing Page, así como en la creación de las funcionalidades clave asociadas a los roadmaps y a las sesiones de registro e inicio de sesión en la aplicación móvil principal de Roademics. Este enfoque integral abarcó la definición detallada de las rutas de la API, la implementación de controladores necesarios para gestionar la interacción entre el cliente y el servidor, y la creación de servicios que soportan las funcionalidades requeridas por el sistema.

Durante este sprint, se priorizó la usabilidad y la experiencia del usuario, asegurando que cada componente de la interfaz no solo cumpla con los requisitos funcionales, sino que también ofrezca una navegación intuitiva y atractiva. Además, se llevaron a cabo sesiones de revisión y pruebas para validar que las funcionalidades implementadas se alinearan con las expectativas del Product Backlog. Este enfoque colaborativo y centrado en el usuario es fundamental para garantizar que nuestra solución sea efectiva y satisfaga las necesidades de nuestros clientes.

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
            <td>US041</td>
            <td>Diseñar una landing page persuasiva con un claro llamado a la acción (CTA)</td>
            <td>T001</td>
            <td>Diseño de Landing Page con un Call To Action</td>
            <td><strong>Como</strong> diseñador web, <strong>quiero</strong> diseñar una landing page persuasiva con un claro llamado a la acción (CTA), <strong>para</strong> maximizar la conversión de visitantes en usuarios activos y asegurar que el mensaje principal y las acciones deseadas sean destacadas y fácilmente accesibles.</td>
            <td>3 horas</td>
            <td>Yen Cerna, Lucio Heli</td>
            <td>Done</td>
        </tr>
                <tr>
            <td>US042</td>
            <td>Visualizar contenido de Landing Page</td>
            <td>T02</td>
            <td>Visualización de contenido completo de la Landing Page</td>
            <td><strong>Como</strong> visitante de la plataforma, <strong>quiero</strong> poder visualizar el contenido de la landing page, <strong>para</strong> obtener toda la información relevante sobre los productos o servicios ofrecidos y tomar una decisión informada sobre la acción a seguir.</td>
            <td>2 horas</td>
            <td>Yen Cerna, Lucio Heli</td>
            <td>Done</td>
        </tr>
                <tr>
            <td>US043</td>
            <td>Formulario de contacto</td>
            <td>T03</td>
            <td>Desarrollo y presentación de formulario de contacto</td>
            <td><strong>Como</strong> visitante de la plataforma, <strong>quiero</strong> tener acceso a un formulario de contacto, <strong>para</strong> poder enviar consultas, comentarios o solicitudes a la empresa de manera rápida y sencilla.</td>
            <td>1 hora con 30 minutos</td>
            <td>Trigueros Chumacero, Flavio Eduardo</td> 
            <td>Done</td>
        </tr>
                <tr>
            <td>US044</td>
            <td>Implementación de footer</td>
            <td>T04</td>
            <td>Implementación de la sección de footer</td>
            <td><strong>Como</strong> visitante de la plataforma, <strong>quiero</strong> que el footer esté implementado en todas las páginas, <strong>para</strong> tener acceso a información adicional, enlaces importantes y recursos útiles sin importar en qué sección me encuentre.</td>
            <td>1 hora con 30 minutos</td>
            <td>Valenzuela Huillcaya, Aldhair Johan Juan</td>
            <td>Done</td>
        </tr>
                <tr>
            <td>US045</td>
            <td>Responsive Landing Page</td>
            <td>T05</td>
            <td>Implementación de propiedades Responsive en la Landing Page</td>
            <td><strong>Como</strong> visitante de la plataforma, <strong>quiero</strong> que la landing page se adapte de manera responsiva a diferentes dispositivos y tamaños de pantalla, <strong>para</strong> tener una experiencia de usuario óptima sin importar el dispositivo que utilice para acceder a la página.</td>
            <td>1 hora</td>
            <td>Pescoran Angulo, Juan Fabrizzio</td> 
            <td>Done</td>
        </tr>
                <tr>
            <td>US001</td>
            <td>Registro de cuenta en la plataforma</td>
            <td>T06</td>
            <td>Registro de una cuenta en la aplicación</td>
            <td><strong>Como</strong> un nuevo usuario en la aplicación de Roademics, <strong>quiero</strong> registrarme en la plataforma creando una cuenta personal con el uso de datos pertinentes y adecuadamente informados por la aplicación, <strong>para</strong> obtener acceso completo a todas las funcionalidades de la aplicación, permitiéndome gestionar mi perfil, interactuar con el contenido y beneficiarme de las características ofrecidas.</td>
            <td>2 horas con 30 minutos</td>
            <td>Trigueros Chumacero, Flavio Eduardo</td>
            <td>Done</td>
        </tr>
                  <tr>
            <td>US004</td>
            <td>Inicio de sesión con cuenta de la aplicación</td>
            <td>T07</td>
            <td>Verificación de un Correo Electrónico durante el proceso de registro</td>
            <td><<strong>Como</strong> usuario ya registrado de forma adecuada en la aplicación de Roademics, <strong>quiero</strong> poder iniciar sesión en la plataforma utilizando datos pertinentes como mi correo electrónico y contraseña, <strong>para</strong> acceder a mi cuenta de manera rápida y directa, lo que me permitirá gestionar todas las funcionalidades y datos asociados a la misma de forma eficiente.</td>
            <td>3 horas con 30 minutos</td>
            <td>Valenzuela Huillcaya, Aldhair Johan Juan</td>
            <td>Done</td>
        </tr>
    </table>

#### 5.2.1.3 Development Evidence for Sprint Review.

En esta sección se explicarán y presentarán los avances obtenidos en la implementación, relacionados con los productos de la solución según el alcance definido para el Sprint 1 de la sección de Product Implementation. El enfoque de este apartado será documentar cada uno de los commits ya implementados dentro del repositorio de GitHub, proporcionando detalles técnicos de los cambios realizados y su impacto en el desarrollo de la aplicación móvil junto a todas sus funcionalidades por parte de la interfaz.

###### Tabla XX
*Tabla de los commits realizados y relacionados con el desarrollo de todas las secciones del Sprint Backlog 1*

| Repository | Branch| Commit Id| Commit Message| Commit Message Body|Commited on (Date) |
|------------|-------|----------|---------------|--------------------|-------------------|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-MobileApplication|main|038c4057c4a89f79ee2f4acb77971cc8992a010d|Initial commit| This is the Initial Commit of the repository. With this commit we add all the neccesary archives and base models| 25/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-MobileApplication|develop|038c4057c4a89f79ee2f4acb77971cc8992a010d|Initial commit| This is the Initial Commit of the repository. With this commit we add all the neccesary archives and base models| 25/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-MobileApplication|Home-Profile|038c4057c4a89f79ee2f4acb77971cc8992a010d|Initial commit| This is the Initial Commit of the repository. With this commit we add all the neccesary archives and base models| 25/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-MobileApplication|IAM|038c4057c4a89f79ee2f4acb77971cc8992a010d|Initial commit| This is the Initial Commit of the repository. With this commit we add all the neccesary archives and base models| 25/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-MobileApplication|Roadmap|038c4057c4a89f79ee2f4acb77971cc8992a010d|Initial commit| This is the Initial Commit of the repository. With this commit we add all the neccesary archives and base models| 25/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-MobileApplication|IAM|b041e9872ac33b190bee1245236a39efcd625cd3|feat:add base | With this commit we added the main artifacts and libraries that will be used for the main Identity and Access Management module and functionalities. We also created the main pages for the register and the login section. | 25/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|Home-Profile|2085a4451325f1d0668047d8cb6b2ea986d11b59|feat: add home and profile section| With this commit we added a new set of activities for the home and profile screens of the Mobile Application | 26/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|Roadmap|581d7f7f45d1875ef5187e0db252d6ad275a6a74|feat: add roadmaps| With this commit we added some of the main methods and functions of the Roadmaps Bounded Context, mostly for the manual creationg of one. | 27/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-backEnd|Roadmap|d302fdf41169429e50a37201a261bd4a5f5b88fa|feat: fixed proyect| With this commit we fixed some functions related to the Roadmaps section and the artifacts used. | 27/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-landingPage|main|4fcb94a38a101a987a8bbc86dc11b6623a911789|feat: add html, css, js files| With this commit we added the main documents for the configuration and programming of the landing page of Roademics| 28/09/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-landingPage|main|89f1a3b4b56e51ea6d541acd7e5c58fe3f9373fa|feat: add index and styles with boostrap| With this commit we added the main artifacts needed to use the various styles of springboot. We also implemented some styles combined.| 28/09/24|

#### 5.2.1.4 Testing Suite Evidence for Sprint Review. 

En esta sección presentaremos una evidencia detallada de las rigurosas pruebas realizadas durante el sprint, con el fin de garantizar la calidad y la funcionalidad del producto en desarrollo. Hemos implementado la metodología Gherkin, que permite definir escenarios de prueba de manera clara y concisa, facilitando la comprensión tanto para los desarrolladores como para los interesados no técnicos.

Cada uno de estos escenarios de prueba ha sido meticulosamente registrado en commits específicos dentro de nuestro repositorio de código, lo que asegura un historial completo, detallado y transparente del proceso de prueba. Este enfoque no solo permite rastrear fácilmente los cambios y correcciones asociados a las pruebas, sino que también garantiza que las funcionalidades clave del sistema cumplan con los criterios de aceptación definidos. La metodología adoptada refuerza la integridad del código y la entrega de un producto final robusto y confiable.

###### Tabla 26
*Tabla de los modelos de pruebas realizados y relacionados con el desarrollo de todas las secciones del Sprint Backlog 1*
| Repository                        | Branch              | Commit Id                          | Commit Message                   | Commit Message Body           |Commited on (Date) |
|-----------------------------------|---------------------|------------------------------------|----------------------------------|-------------------------------|-------------------|
| upc-pre-202402-cc-238-WV61-WeHaveAnIdea-AcceptanceTests | Sprint-1 | e7e7f030e2b31007d0f9daf82fecc1889569c491 | feat: add US_Sprint1_Frontend | In this sections, all the Acceptance Test related to the Sprint 1 of Roademic's Product Implementation were implemented using the Gherkin format. | 28/09/24 |

#### 5.2.1.5 Execution Evidence for Sprint Review. 

En esta sección, presentamos de manera exhaustiva y organizada los avances alcanzados durante el primer sprint del proyecto Roademics. Estos logros abarcan principalmente el desarrollo y la implementación de la Landing Page, que ha sido completada utilizando un enfoque eficiente y alineado con los objetivos del sprint. Para su construcción, se emplearon los recursos ofrecidos por el framework Spring Boot, aprovechando sus componentes de diseño predeterminados y la estructura proporcionada por las plantillas base de HTML y CSS. Además, se incorporaron funcionalidades dinámicas mediante JavaScript, logrando una integración fluida entre la interfaz de usuario y las operaciones del backend, asegurando así un rendimiento óptimo.

De manera complementaria, se ha avanzado en la implementación de funcionalidades clave dentro de los módulos de inicio de sesión y registro de la aplicación móvil. Estas funcionalidades iniciales forman parte de la estructura fundamental de la aplicación, permitiendo un primer acercamiento sólido al desarrollo de la capa de autenticación y mejorando la experiencia del usuario desde las primeras fases del proyecto.

Asimismo, se ha realizado la integración de diversas librerías y artefactos de uso común en el mercado tecnológico actual, con el propósito de incorporar estilos modernos y eficientes que respondan a las tendencias vigentes en el desarrollo móvil. Este enfoque asegura no solo una alineación con las mejores prácticas de la industria, sino también una base sólida para la evolución del proyecto en sprints posteriores.

**Landing Page:**

**FrontEnd Web:**

#### 5.2.1.6 Services Documentation Evidence for Sprint Review. 

En esta sección presentamos la relación detallada de los Endpoints documentados utilizando la especificación OpenAPI, los cuales están directamente vinculados con el alcance del Sprint y su implementación en el proyecto Roademics por parte de las áreas presentadas en el BackEnd. Estos Endpoints son esenciales para el funcionamiento de las funcionalidades desarrolladas durante el Sprint 1 del FrontEnd, y describen la interacción entre el propio Backend y la propia Aplicación Móvil.

A continuación, se incluye una tabla exhaustiva donde se especifican las acciones soportadas para cada Endpoint, destacando el verbo HTTP utilizado (GET, POST, PUT, DELETE, PATCH) y proporcionando la sintaxis exacta de la llamada. También se detallan los posibles parámetros que pueden ser incluidos, junto con un ejemplo práctico de cada solicitud. Además, se ofrece una explicación clara y precisa del response correspondiente, asegurando que el equipo de desarrollo y los interesados comprendan cómo se procesan las peticiones y respuestas en el sistema. Esta documentación es clave para garantizar una integración fluida y efectiva entre los componentes del sistema, facilitando la comunicación entre el Backend y el FrontEnd.

###### Tabla 27
*Tabla del modelo de escritura para el Bounded Context de IAM*
| Método  | Descripción                                  | Ejemplo de llamada         | Parámetros                                     | Respuesta                                                                                 |
|---------|----------------------------------------------|----------------------------|------------------------------------------------|-------------------------------------------------------------------------------------------|
| POST    | Crear un nuevo usuario                       | POST /usuarios              | `username`, `email`, `password`                | Detalles del nuevo usuario creado en formato JSON, incluyendo ID y fecha de creación.      |
| GET     | Obtener detalles de un usuario específico    | GET /usuarios/{id}          | `id` del usuario                               | Detalles del usuario solicitado, incluyendo roles, fecha de registro, y demás datos.       |
| POST    | Autenticación de usuario                     | POST /usuarios/authenticate | `username`, `password`                         | Token JWT válido para autenticar las siguientes peticiones del usuario.                    |

#### 5.2.1.7 Software Deployment Evidence for Sprint Review.

En esta sección detallaremos exhaustivamente el proceso de despliegue de los sistemas planificados para este Sprint, abarcando tanto la aplicación móvil como otras plataformas web asociadas. Presentaremos el proceso paso a paso, proporcionando evidencia clara en cada fase del despliegue, y explicando las características técnicas de cada plataforma utilizada para asegurar un despliegue exitoso.

Durante este Sprint 1, se realizó el despliegue de la Landing Page de Roademics como una página web de acceso rápido y directo. Para este propósito, optamos por utilizar GitHub Pages, una herramienta confiable y gratuita proporcionada por GitHub que facilita la publicación de sitios web estáticos directamente desde un repositorio. Esta elección se debió a su facilidad de uso, integración con flujos de trabajo basados en Git y su soporte nativo para dominios personalizados, lo que permite una rápida puesta en marcha sin necesidad de configurar un servidor adicional.

Comenzaremos el proceso creando un repositorio en GitHub, que servirá como el almacén centralizado para todos los archivos que componen nuestra página de destino, incluyendo HTML, CSS y JavaScript. Una vez que el repositorio esté establecido, cada miembro del equipo colaborará en su propia rama "feature" para desarrollar distintas características y funcionalidades del Landing Page, garantizando así que cada contribución se realice de manera aislada y organizada. Al finalizar el desarrollo de una característica específica, se procederá a llevar a cabo el proceso de fusión (merge) con la rama "develop". Este proceso de integración es crucial, ya que asegura que la página de destino se mantenga siempre actualizada con las últimas modificaciones y mejoras que se hayan implementado por parte de los miembros del equipo. Para facilitar esta integración, se recomienda que se realicen revisiones de código y pruebas antes de completar el merge, lo que contribuirá a mantener la calidad del código y a detectar posibles conflictos o errores en etapas tempranas.

Posteriormente, configuraremos GitHub Pages para que publique automáticamente la página de destino utilizando la rama "develop". Este paso es fundamental, ya que permitirá que nuestra Landing Page sea accesible públicamente, facilitando su visualización y prueba por parte de los interesados y usuarios finales. Esta configuración no solo simplifica el proceso de despliegue, sino que también proporciona un enlace directo que puede compartirse fácilmente con el equipo y las partes interesadas, permitiendo una retroalimentación más rápida y eficiente.

A continuación, proporcionaremos una descripción detallada de los pasos necesarios para llevar a cabo este proceso de despliegue en GitHub Pages. Cada uno de estos pasos se elaborará con suficiente profundidad para asegurar una implementación eficiente y sin contratiempos de nuestra solución, destacando las mejores prácticas y consideraciones técnicas que deberán tenerse en cuenta a lo largo del proceso. Con esta guía, buscamos garantizar que el equipo esté alineado y preparado para llevar a cabo una implementación exitosa del Landing Page.

1. El primer paso en nuestro proceso de despliegue es la creación de un repositorio público en GitHub. Para ello, asignaremos un nombre adecuado al repositorio que refleje el propósito y contenido de nuestra página de destino. Una vez creado el repositorio, procederemos a añadir los archivos necesarios para la construcción y funcionamiento del Landing Page. Es fundamental seleccionar un nombre significativo que identifique claramente el propósito del repositorio y la naturaleza de los archivos que contendrá. Esto facilitará la gestión y colaboración en el desarrollo del proyecto, asegurando que todos los miembros del equipo puedan identificar y acceder al repositorio de manera eficiente. Una vez completada esta tarea, estaremos listos para iniciar el proceso de desarrollo y construcción de nuestro Landing Page, utilizando el repositorio recién creado como punto de partida. Este enfoque nos proporcionará una base sólida y organizada desde la cual avanzar en el desarrollo de nuestra solución.

###### Figura 60
*Imagenes de muestra y presentación sobre la construcción del repositorio designado para la Landing Page de Roademics.*
<img src="/assets/img/set-repository-name.png" alt="Set Repository Name">
<img src="/assets/img/repository.png" alt="Repository">

2. El segundo paso implica dirigirse a la sección de ajustes en GitHub y seleccionar la pestaña Pages. Una vez allí, podremos acceder a las configuraciones relacionadas con la publicación de páginas web directamente desde nuestro repositorio. Esta acción nos permitirá habilitar la funcionalidad de GitHub Pages para nuestro repositorio, lo que nos permitirá alojar y publicar nuestro Landing Page de forma rápida y sencilla. La pestaña Pages ofrece una interfaz intuitiva que nos guiará a través del proceso de configuración, permitiéndonos personalizar diversos aspectos de nuestra página web, como la rama a utilizar para el despliegue y el dominio personalizado, si así lo deseamos. Al acceder a esta sección y realizar las configuraciones necesarias, estaremos un paso más cerca de hacer que nuestro Landing Page esté disponible públicamente para su visualización y acceso por parte de los usuarios finales

3. El tercer paso implica dirigirnos al apartado de configuración específico para GitHub Pages en nuestro repositorio. Una vez en esta sección, podremos ajustar diferentes aspectos relacionados con la publicación de nuestro sitio web, como la rama a utilizar, el directorio desde el que se servirán los archivos, y otras opciones de configuración avanzadas. Esta parte del proceso nos brinda la oportunidad de personalizar aún más la forma en que nuestra página web será desplegada y accesible para los usuarios finales. Por ejemplo, podemos seleccionar la rama específica que contiene los archivos de nuestro Landing Page y especificar el directorio raíz desde el cual se servirán los archivos HTML, CSS y JavaScript.

4. El cuarto paso implica dirigirse al apartado de "branch" dentro de la configuración de GitHub Pages y seleccionar el branch "main" donde se realizará el despliegue del Landing Page. Es importante asegurarse de elegir el branch correcto donde se encuentran los archivos actualizados de nuestra página web para garantizar que la versión más reciente se despliegue correctamente. Durante este proceso, es recomendable dejar las demás configuraciones con sus valores predeterminados, a menos que tengamos necesidades específicas que requieran ajustes adicionales. Mantener estas configuraciones en sus valores predeterminados ayuda a simplificar el proceso y reduce la posibilidad de errores durante el despliegue.

###### Figura 61
*Imagen de muestra y presentación sobre el despliegue de la Landing Page y el ajuste de las ramas integradas.*
<img src="/assets/img/pagedeployed.png" alt="github page">

5. Una vez seleccionada la rama correspondiente, se generará un enlace que permitirá acceder al Landing Page desplegado. Este enlace proporciona una forma rápida y sencilla para que los usuarios accedan a nuestra página web y puedan interactuar con su contenido. Es importante tener en cuenta que cualquier modificación realizada en el branch "main" se actualizará automáticamente en el Landing Page desplegado. Esto significa que cualquier cambio que realicemos en nuestros archivos HTML, CSS o JavaScript se reflejará de inmediato en la versión en vivo de nuestra página web. Este proceso de actualización automática garantiza que nuestro Landing Page esté siempre sincronizado con las últimas modificaciones realizadas en el código fuente, lo que proporciona una experiencia consistente y actualizada para los usuarios que acceden a nuestra página web."

###### Figura 62
*Imagen de muestra y presentación sobre la obtención del enlace de ingreso a la Landing Page de Roademics.*
<img src="/assets/img/github-link.png" alt="github link">

6. Una vez completados los pasos anteriores, el Landing Page estará desplegado y listo para ser visualizado y utilizado. Los usuarios podrán acceder al enlace generado y explorar el contenido de nuestra página web. Es importante realizar pruebas adicionales después del despliegue para asegurarse de que la página web se vea y funcione correctamente en diferentes dispositivos y navegadores. Esto garantizará una experiencia de usuario óptima para todos los visitantes de nuestro sitio. En caso los lectores quieran revisar el link desplegado de la Landing Page de Roademics de forma directa y rápida, pueden usar el siguiente enlace: https://grupo-3-moviles.github.io/upc-pre-202402-cc-238-WV61-WeHaveAnIdea-landingPage/ 

###### Figura 63
*Imagen de muestra y presentación sobre la Landing Page de Roademics ya desplegada.*
<img src="/assets/img/landing_deployed.png" alt="Landing deployed">

#### 5.2.1.8 Team Collaboration Insights during Sprint.

Durante el Sprint 1 de la sección Product Software Development & Implementation, nos enfocamos en el desarrollo colaborativo del FrontEnd de la aplicación móvil de Roademics, además de la Landing Page, donde cada miembro del equipo contribuyó con sus habilidades y conocimientos. Esta colaboración se refleja en los numerosos commits realizados en nuestro repositorio de código, los cuales están respaldados por capturas de pantalla adjuntas para una documentación detallada.

Nuestro equipo se reunió tanto en persona como virtualmente para asignar tareas y discutir la estrategia de desarrollo del proyecto. Estas reuniones fueron cruciales para clarificar nuestras responsabilidades individuales y asegurar un desempeño óptimo. Para maximizar la eficiencia, decidimos asignar a cada miembro del equipo una sección específica del FrontEnd para desarrollar, lo que nos permitió avanzar rápidamente y cumplir con los plazos establecidos.

Además, programamos sesiones regulares de brainstorming y resolución de problemas, donde compartimos ideas y abordamos cualquier duda o dificultad que surgiera durante el proceso de desarrollo. Estas reuniones fueron fundamentales para resolver obstáculos de manera efectiva y garantizar un progreso constante en la elaboración del FrontEnd de la Web Application.

###### Figura 88
*Reporte completo de contribuciones para el desarrollo del FrontEnd de la Aplicación Móvil de Roademics durante el Sprint 1 de Software Development & Implementation.*

<img src="/assets/img/Pulse-backend-for-main-sprint1.png" alt="Pulse for the Main Branch in Software Development and Implementation">
<img src="/assets/img/Contributions-backend-for-main-sprint1.png" alt=Contributions for the Main Branch in Software Development and Implementation ">
<img src="/assets/img/Individual-contributions-for-main-sprint1.png" alt="Individual Contributions for the Main Branch in Software Development and Implementation">

---

### 5.2.2. Sprint 2

En esta sección, se registrará y explicará el avance en términos de producto y trabajo colaborativo correspondiente al Sprint número 2 de la Implementación del FrontEnd. Este registro detallado documentará cada aspecto del progreso logrado, incluyendo el desarrollo de la interfaz de usuario en su página de perfil, las principales funcionalidades de Roadmaps e Inteligencia Artificial, todas las secciones referentes al networking, y el avance colectivo aportado por cada integrante del equipo de trabajo en relación con los componentes del FrontEnd y sus respectivas interacciones entre Bounded Context. Se hará hincapié en la importancia de la colaboración y la comunicación efectiva entre los miembros del equipo para alcanzar los objetivos del sprint, destacando cómo cada aportación individual contribuye al éxito colectivo del proyecto.

Todas las especificaciones y resultados presentados en esta sección se derivan del Product Backlog establecido en el Capítulo 2, en la sección de requerimientos. Este alineamiento garantiza que los desarrollos realizados durante el sprint sean consistentes con las expectativas del proyecto y contribuyan a la visión general del producto, asegurando que la interfaz cumpla con los estándares de calidad y usabilidad deseados.

#### 5.2.2.1 Sprint Planning 2.

Aqui se detallarán los puntos discutidos y analizados durante la reunión de Sprint Planning para el segundo sprint enfocado en la implementación del FrontEnd. El objetivo principal de dicha reunión fue establecer un plan estratégico y alcanzable que guíe el desarrollo de la interfaz de usuario, garantizando la incorporación de todas las funcionalidades esenciales para los usuarios. Durante el encuentro, se identificaron las tareas específicas a ejecutar, comprometiéndose a entregar un conjunto de resultados tangibles que contribuyan al progreso del proyecto, particularmente en las funcionalidades clave como la generación y edición de roadmaps, las funciones relacionadas con la gestión del perfil y datos de usuario, así como las características principales de la sección de networking.

Este enfoque asegura que todos los miembros del equipo compartan una visión común respecto a los objetivos y expectativas del sprint, lo cual es fundamental para mantener una adecuada coordinación y efectividad en el trabajo colaborativo. A lo largo de la reunión, se establecieron las características que serán desarrolladas, se definieron los plazos para cada tarea y se acordaron los criterios de aceptación correspondientes. Además, se promovió un diálogo abierto entre los integrantes del equipo, con el fin de identificar posibles desafíos y áreas de mejora, asegurando que todos los aspectos del desarrollo del FrontEnd estén alineados con las metas generales del proyecto. Esta metodología contribuye a una planificación estructurada y a una ejecución eficiente de las tareas, reforzando el compromiso del equipo con los objetivos del sprint.

###### Tabla 23
*Tabla del planeamiento a profundidad del Sprint 1*
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
            <td>2024-10-12</td>
        </tr>
          <tr>
            <td>Time</td>
            <td>17:16</td>
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
            <td>Sprint 2 Review Summary</td>
            <td>Al finalizar el Sprint 2, se concretó la reunión del Sprint Review para evaluar el avance en el desarrollo del FrontEnd de nuestra aplicación. En este sprint, el objetivo principal fue el desarrollo de funciones clave en la aplicación, tales como la generación y edición de roadmaps mediante el asesor que funciona a base de inteligencia artificial, y la implementación de secciones como el perfil de usuario y mejoras en el diseño de las pantallas de networking. <br><br>La reunión fue exitosa, tanto por los avances logrados en los productos de software como por la efectiva colaboración del equipo. Se expusieron las nuevas funcionalidades, se realizaron demostraciones de la interfaz de usuario, y se recibieron comentarios útiles de los miembros del equipo y otros interesados. Este valioso intercambio de ideas permitió identificar oportunidades de mejora y ajustar las prioridades para el siguiente sprint. La colaboración y comunicación fluida durante esta revisión contribuyeron significativamente a la cohesión del equipo y aseguraron que el desarrollo del FrontEnd siguiera en línea con los objetivos generales del proyecto.</td> 
        </tr>
            <tr>
            <td>Sprint 2 Retrospective Summary</td>
            <td>Durante la Sprint Retrospective del Sprint 2, el equipo se enfocó en analizar en detalle toda la retroalimentación obtenida tras la finalización de este ciclo de proyecto. Esta evaluación profunda, tanto del desempeño colectivo como del individual, nos permitió identificar áreas críticas de mejora que resultarán esenciales para perfeccionar nuestra aplicación móvil desde la perspectiva del FrontEnd.<br><br> En este ejercicio de reflexión, surgieron diversas propuestas enfocadas en elevar la calidad del trabajo entregado y asegurar que el producto final cumpla con las expectativas de nuestros usuarios. Se abordaron temas como la mejora en el rendimiento de la aplicación y su balance con el diseño de interfaz, el uso de APIs y mejores opciones de librerías, y mejoras en el alcance y la portabilidad que presentara nuestra aplicación. Este intercambio de ideas no solo reforzó la colaboración del equipo, sino que también estableció un camino claro para los próximos sprints, asegurando que el producto final no solo presente un diseño atrayente, intuitivo y atractivo para los clientes, sino también que las funcionalidades sean accesibles, se encuentren adecuadamente organizadas, y presenten un buen rendimiento. </td>
        </tr>
            <tr>
            <td colspan="2">Sprint Goal & User Stories</td>
        </tr>
              <tr>
            <td>Sprint 2 Goal</td>
            <td>Alcanzar una métrica de cumplimiento del 100%, lo que indicará que se ha logrado todos los objetivos del sprint 2 con todas las historias de usuario y otros materiales necesarios.</td>
        </tr>
              <tr>
            <td>Sprint 2 Velocity</td>
            <td>Con el equipo para este sprint 2 decidimos aceptar 8 Story Points</td>
        </tr>
              <tr>
            <td>Sum of Story Points</td>
            <td>La suma de los Story Points para los User Stories que se están incluyendo en este Sprint 2 es 101</td>
        </tr>
    </table>

#### 5.2.2.2 Sprint Backlog 2.

En esta sección se analizará en detalle el proceso del Sprint Backlog 2, en el cual nuestro equipo concentró sus esfuerzos principalmente en el diseño de los bounded contexts de Roadmaps, Gestión de Usuarios, y en avanzar en aspectos clave de Networking. Este enfoque abarcó de manera integral la definición de cada una de las funcionalidades planteadas en las historias de usuario, además del diseño de cada actividad ya asignada y la propia interfaz.

A lo largo de este sprint, se dio prioridad a la usabilidad y a la experiencia del usuario, asegurando que cada elemento de la interfaz no solo cumpliera con los requisitos funcionales, sino que también proporcionara una navegación fluida y atractiva. Además, se realizaron sesiones de revisión y pruebas exhaustivas para verificar que las funcionalidades desarrolladas estuvieran alineadas con las expectativas del Product Backlog. Este enfoque colaborativo, centrado en el usuario, es crucial para garantizar que la solución no solo sea efectiva, sino también capaz de satisfacer las necesidades de nuestros clientes de manera óptima.

###### Tabla 59
*Tabla principal del planeamiento del Sprint Backlog 2*
<table>
        <tr>
            <td colspan="2">Sprint #</td>
            <td colspan="6">Sprint 2</td>
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
            <td>US007</td>
            <td>Agregar una foto o imagen en el perfil de usuario</td>
            <td>T08</td>
            <td>Agregar imagen de perfil de usuario</td>
            <td><strong>Como</strong> un usuario registrado en la aplicación de Roademics, <strong>quiero</strong> ser capaz de agregar una imagen o foto a mi perfil de usuario en la plataforma, siguiendo todos los formatos más adecuados, <strong>para</strong> personalizar mi cuenta y que otros usuarios puedan reconocerme fácilmente al interactuar conmigo.</td>
            <td>1 hora</td>
            <td>###</td>
            <td>Done</td>
        </tr>
          <tr>
            <td>US008</td>
            <td>Gestión de sección de biografía</td>
            <td>T09</td>
            <td>Agregar y gestionar biografía de usuario</td>
            <td><strong>Como</strong> usuario registrado en la aplicación de Roademics, <strong>quiero</strong> poder agregar, editar y eliminar mi biografía en la plataforma, <strong>para</strong> proporcionar información adicional sobre mí y personalizar mi perfil, reflejando datos relevantes para mi red de contactos.</td>
            <td>1 hora</td>
            <td>###</td>
            <td>Done</td>
        </tr>
            <tr>
            <td>US011</td>
            <td>Actualización de información personal</td>
            <td>T10</td>
            <td>Actualización de información de perfil</td>
            <td><strong>Como</strong> usuario registrado en la aplicación de Roademics, <strong>quiero</strong> poder actualizar mi información personal como nombres, apellidos, país y nacionalidad, y detalles de contacto en la plataforma, <strong>para</strong> mantener mi perfil actualizado y asegurarme de que otros usuarios puedan contactar conmigo de manera adecuada.</td>
            <td>2 horas y 30 minutos</td>
            <td>###</td>
            <td>Done</td>
        </tr>
              <tr>
            <td>US012</td>
            <td>Eliminación de una cuenta de usuario</td>
            <td>T11</td>
            <td>Eliminación de cuenta de usuario</td>
            <td><strong>Como</strong> usuario registrado en la aplicación de Roademics, <strong>quiero</strong> ser capaz de eliminar mi cuenta de la plataforma una vez me encuentre autenticado en mi perfil, <strong>para</strong> eliminar todos los datos personales asociados si ya no deseo utilizar el servicio de manera segura y permanente.</td>
            <td>1 hora</td>
            <td>###</td>
            <td>Done</td>
        </tr>
                <tr>
            <td>US013</td>
            <td>Sección de cambio de contraseña</td>
            <td>T12</td>
            <td>Página con sección de cambio de contraseña</td>
            <td><strong>Como</strong> usuario registrado en la aplicación de Roademics, <strong>quiero</strong> poder cambiar mi contraseña desde una sección específica en mi perfil, <strong>para</strong> actualizar mi contraseña de manera segura y mantener la integridad de mi cuenta a corto y largo plazo.</td>
            <td>1 hora</td>
            <td>###</td>
            <td>Done</td>
        </tr>
                  <tr>
            <td>US016</td>
            <td>Creación de roadmap académico básico</td>
            <td>T13</td>
            <td>Creación de un roadmap básico</td>
            <td><strong>Como</strong> usuario de la aplicación de Roademics interesado en planificar mi trayectoria profesional con las funciones ofrecidas, <strong>quiero</strong> crear un roadmap académico básico en la plataforma, <strong>para</strong> visualizar y gestionar mi progreso académico, planificar mis cursos y establecer metas profesionales de manera eficiente y estructurada.</td>
            <td>3 horas y 30 minutos</td>
            <td>###</td>
            <td>Done</td>
        </tr>
                    <tr>
            <td>US017</td>
            <td>Generación automática de roadmap con el uso de Inteligencia Artificial</td>
            <td>T14</td>
            <td>Creación de un roadmap básico con Inteligencia Artificial</td>
            <td><strong>Como</strong> usuario que busca optimizar su trayectoria profesional con la aplicación de Roademics, <strong>quiero</strong> que la plataforma sea capaz de generar un roadmap profesional utilizando las herramientas de inteligencia artificial que dispone, <strong>para</strong> recibir una recomendación personalizada y optimizada de cursos y objetivos que se alineen con mis metas profesionales y educativas.</td>
            <td>3 horas</td>
            <td>###</td>
            <td>Done</td>
        </tr>
                      <tr>
            <td>US018</td>
            <td>Menú de almacenamiento de Roadmaps de un usuario</td>
            <td>T15</td>
            <td>Implementar menú de almacenamiento de roadmaps personales</td>
            <td><strong>Como</strong> usuario que busca optimizar su trayectoria profesional con la aplicación de Roademics, <strong>quiero</strong> que la plataforma tenga un pequeño menú o dashboard donde se muestren todos los roadmaps u hojas de ruta que he generado en la aplicación, <strong>para</strong> tener un acceso directo a cada uno de mis roadmaps y poder almacenarlos de forma más sencilla, cómoda y organizada.</td>
            <td>2 horas</td>
            <td>###</td>
            <td>Done</td>
        </tr>
                        <tr>
            <td>US019</td>
            <td>Acceso a plantillas básicas y avanzadas para la creación de Roadmaps</td>
            <td>T16</td>
            <td>Diseño de plantillas básicas y avanzadas para la creación de Roadmaps</td>
            <td><strong>Como</strong> usuario que desea mejorar su planificación profesional con el uso de la aplicación de Roademics, <strong>quiero</strong> tener acceso a plantillas predeterminadas y avanzadas para mis hojas de rutas y roadmaps, <strong>para</strong> facilitar el desarrollo y diseño de los roadmaps de forma profesional, detallada y personalizada, que se ajuste a mis necesidades y objetivos específicos.</td>
            <td>1 hora y 30 minutos</td>
            <td>###</td>
            <td>Done</td>
        </tr>
                          <tr>
            <td>US020</td>
            <td>Edición de roadmaps básicos</td>
            <td>T17</td>
            <td>Edición de un roadmap básico</td>
            <td><strong>Como</strong> usuario que ha creado un roadmap básico en la plataforma de Roademics, <strong>quiero</strong> poder editar el roadmap existente con el uso de herramientas variadas de edición y modificación, <strong>para</strong> actualizar la información relevante, ajustar mis objetivos profesionales o académicos, y modificar mis planes según mis necesidades actuales.</td>
            <td>4 horas y 30 minutos</td>
            <td>###</td>
            <td>Done</td>
        </tr>
                            <tr>
            <td>US021</td>
            <td>Acceso a herramientas de edición avanzada de roadmaps para usuarios premium</td>
            <td>T18</td>
            <td>Desarrollo de herramientas de edición avanzada de roadmaps (Para usuarios premium)</td>
            <td><strong>Como</strong> usuario con suscripción Premium en la plataforma Roademics, <strong>quiero</strong> tener acceso a herramientas de edición avanzada para la modificación de mis roadmaps profesionales, <strong>para</strong> aprovechar funcionalidades adicionales que me permitan optimizar la planificación y gestión de mis metas, brindándome mayor flexibilidad y precisión en la creación y ajuste de mis objetivos.</td>
            <td>2 horas y 30 minutos</td>
            <td>###</td>
            <td>Done</td>
        </tr>
                              <tr>
            <td>US022</td>
            <td>Eliminación de Roadmaps</td>
            <td>T19</td>
            <td>Eliminación de Roadmaps</td>
            <td><strong>Como</strong> usuario registrado en la plataforma Roademics, <strong>quiero</strong> poder eliminar roadmaps que ya no necesito, <strong>para</strong> mantener mi perfil organizado, optimizar el uso de la plataforma y evitar la acumulación de información obsoleta o irrelevante.</td>
            <td>1 hora y 30 minutos</td>
            <td>###</td>
            <td>Done</td>
        </tr>
                                <tr>
            <td>US023</td>
            <td>Visualizar limitaciones respecto a la cantidad de roadmaps que el usuario podrá gestionar</td>
            <td>T20</td>
            <td>Visualización de limitaciones de la cantidad de roadmaps que cada usuario puede gestionar</td>
            <td><strong>Como</strong> usuario registrado de Roademics, <strong>quiero</strong> visualizar las limitaciones respecto a la cantidad de roadmaps que puedo gestionar dentro de la sección de organización de roadmaps, <strong>para</strong> tener un control claro y transparente sobre el número de roadmaps que puedo crear y editar, asegurándome de no sobrepasar los límites establecidos por mi plan de suscripción o la configuración de la misma plataforma.</td>
            <td>1 hora y 30 minutos</td>
            <td>###</td>
            <td>Done</td>
        </tr>
                                  <tr>
            <td>US024</td>
            <td>Recibir análisis avanzados sobre un Roadmap en específico para los usuarios premium</td>
            <td>T21</td>
            <td>Análisis avanzado sobre un Roadmap en específico para los usuarios premium</td>
            <td><strong>Como</strong> usuario Premium de la plataforma Roademics, <strong>quiero</strong> recibir análisis avanzados y detallados sobre el progreso y la estructura de mi roadmap profesional, <strong>para</strong> obtener información valiosa que me permita identificar áreas de mejora, optimizar mi planificación, y tomar decisiones informadas que me ayuden a alcanzar mis objetivos profesionales de manera más efectiva y eficiente.</td>
            <td>3 horas</td>
            <td>###</td>
            <td>Done</td>
        </tr>
                                    <tr>
            <td>US025</td>
            <td>Poder exportar mi roadmaps en formato como PDF o PNG</td>
            <td>T22</td>
            <td>Exportar roadmaps en formato PDF o PNG</td>
            <td><strong>Como</strong> usuario premium de la plataforma Roademics, <strong>quiero</strong> poder exportar mis roadmaps generados y editados mediante formatos de archivo como PDF o PNG, <strong>para</strong> disponer de una copia accesible, portable y presentable de mis planes profesionales, que pueda ser utilizada para compartir, almacenar o imprimir con facilidad y conservar la integridad del diseño visual y la información estructurada en la plataforma.</td>
            <td>2 horas</td>
            <td>###</td>
            <td>Done</td>
        </tr>
                                    <tr>
            <td>US026</td>
            <td>Poder crear los nodos de mi roadmap</td>
            <td>T23</td>
            <td>Creación de nodos de un roadmap</td>
            <td><strong>Como</strong> usuario registrado de la plataforma Roademics, <strong>quiero</strong> poder crear los nodos de mi roadmap de forma manual, <strong>para</strong> estructurar y definir claramente las etapas, actividades y acciones necesarias para alcanzar mis objetivos profesionales de manera organizada y efectiva.</td>
            <td>3 horas</td>
            <td>###</td>
            <td>Done</td>
        </tr>
                                      <tr>
            <td>US027</td>
            <td>Recibir notificación si un nodo en mi grafo se vuelve obsoleto o ya no está disponible</td>
            <td>T24</td>
            <td>Notificar si un nodo en un grafo se vuelve obsoleto o ya no se encuentra disponible</td>
            <td><strong>Como</strong> usuario registrado en la plataforma Roademics, <strong>quiero</strong> recibir una notificación si un nodo en mi grafo se vuelve obsoleto o ya no está disponible, <strong>para</strong> estar al tanto de cualquier cambio que pueda afectar la estructura y el progreso de mi roadmap, y tomar las medidas necesarias para actualizar o ajustar mi plan según sea necesario.</td>
            <td>2 horas</td>
            <td>###</td>
            <td>Done</td>
        </tr>
                                        <tr>
            <td>US028</td>
            <td>Guardar versiones de mi roadmap</td>
            <td>T25</td>
            <td>Historial de versiones de un roadmap</td>
            <td><strong>Como</strong> usuario registrado en la plataforma Roademics, <strong>quiero</strong> ser capaz de guardar distintas versiones de mi roadmap, <strong>para</strong> tener un historial de cambios y poder revertir a versiones anteriores si es necesario, asegurando así que pueda realizar ajustes sin perder progresos importantes.</td>
            <td>2 horas y 30 minutos</td>
            <td>###</td>
            <td>Done</td>
        </tr>
    </table>

#### 5.2.2.3 Development Evidence for Sprint Review.

En esta sección se explicarán y presentarán los avances obtenidos en la implementación, relacionados con los productos de la solución según el alcance definido para el Sprint 2 de la sección de Product Implementation. El enfoque de este apartado será documentar cada uno de los commits ya implementados dentro del repositorio de GitHub, proporcionando detalles técnicos de los cambios realizados y su impacto en el desarrollo de la aplicación móvil junto a todas sus funcionalidades por parte de la interfaz.

###### Tabla XX
*Tabla de los commits realizados y relacionados con el desarrollo de todas las secciones del Sprint Backlog 2*
| Repository | Branch| Commit Id| Commit Message| Commit Message Body|Commited on (Date) |
|------------|-------|----------|---------------|--------------------|-------------------|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-Roademics|profile-feature|fcd14b9127bccf8dce545dfaff8e439c2dde91c7|chore: create clean architecture folder structure and add app_constants|committed :)| 25/10/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-Roademics|profile-feature|11e89700dd38ae8f9b45e8f598a3278a1e746222|chore: add placeholder for team collaboration|committed :)| 26/10/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-Roademics|profile-feature|f3e95111ef5f8264cb4c28fbbc2ee7adb46545a0|chore: add more placeholders |committed :)| 26/10/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-Roademics|profile-feature|5d323f549767b421e31f61af7bddf5f281371054|feat: add profile page, edit profile, settings page |committed :)| 26/10/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-Roademics|profile-feature|fbb9f26790c7ee08a44aae50b4e9de868ab08fba|feat: add update email settings page |committed :)| 26/10/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-Roademics|profile-feature|65bf6314c46c88c58692c652b8e5e4d69078278d|feat: add update phone number page |committed :)| 26/10/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-Roademics|profile-feature|1dd12af8610363edb885b11be93bf78585066d2f|feat: add change password page|committed :)| 26/10/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-Roademics|profile-feature|d4dc95c6b813259b32fba6ab146dbc2a8aaa7f21|feat: add delete account function|committed :)| 26/10/24|

#### 5.2.2.4 Testing Suite Evidence for Sprint Review. 

En esta sección presentaremos una evidencia detallada de las rigurosas pruebas realizadas durante el sprint, con el fin de garantizar la calidad y la funcionalidad del producto en desarrollo. Hemos implementado la metodología Gherkin, que permite definir escenarios de prueba de manera clara y concisa, facilitando la comprensión tanto para los desarrolladores como para los interesados no técnicos.

Cada uno de estos escenarios de prueba ha sido meticulosamente registrado en commits específicos dentro de nuestro repositorio de código, lo que asegura un historial completo, detallado y transparente del proceso de prueba. Este enfoque no solo permite rastrear fácilmente los cambios y correcciones asociados a las pruebas, sino que también garantiza que las funcionalidades clave del sistema cumplan con los criterios de aceptación definidos. La metodología adoptada refuerza la integridad del código y la entrega de un producto final robusto y confiable.

###### Tabla 26
*Tabla de los modelos de pruebas realizados y relacionados con el desarrollo de todas las secciones del Sprint Backlog 1*
| Repository                        | Branch              | Commit Id                          | Commit Message                   | Commit Message Body           |Commited on (Date) |
|-----------------------------------|---------------------|------------------------------------|----------------------------------|-------------------------------|-------------------|
| upc-pre-202402-cc-238-WV61-WeHaveAnIdea-AcceptanceTests | Sprint-1 | 5198ddb8114acf692f93d46e0224c8652529b5dc | feat: add US_Sprint1.feature | En esta sección se implementaron todos los Acceptance Test para el Sprint 1 del backend de Roademics | 28/09/24 |
| upc-pre-202402-cc-238-WV61-WeHaveAnIdea-AcceptanceTests | Sprint-1 | 7990a48a9b476d87cdcd98de0535f2b07b2644d1 | feat: add TS013-TS017 y TS27-TS040 |En esta sección se implementaron todos los Acceptance Test para el Sprint 1 del backend de Roademics | 28/09/24 |
| upc-pre-202402-cc-238-WV61-WeHaveAnIdea-AcceptanceTests | Sprint-1 | e7e7f030e2b31007d0f9daf82fecc1889569c491 | feat: add US_Sprint1_Frontend |En esta sección se implementaron todos los Acceptance Test para el Sprint 1 del Frontend de Roademics | 28/09/24 |

#### 5.2.2.5 Execution Evidence for Sprint Review. 

Durante el desarrollo de este Sprint 2, en el área de Product Implementation y FrontEnd, nuestro equipo se enfocó en implementar las funcionalidades centrales de los bounded contexts de IAM (Identity and Access Management), Profiles y Roadmaps. Este esfuerzo fue fundamental para asegurar que la aplicación cumpla con los principales requisitos funcionales, siguiendo prácticas avanzadas de desarrollo y una estructura sólida que facilite el crecimiento y la escalabilidad del proyecto en sprints futuros. La implementación de estas funcionalidades no solo marca un hito en la creación de una base estable para la aplicación, sino que también nos permite seguir avanzando con las características adicionales que enriquecerán la experiencia del usuario.

En términos de arquitectura de desarrollo, optamos por un modelo Bloc para gestionar el estado en cada bounded context de manera independiente, permitiendo un control más efectivo del flujo de datos y la reactividad en cada componente de la aplicación. Además, adoptamos un patrón de repositorio, lo que facilita la conexión fluida con el Backend de Roademics y asegura que las solicitudes a los Endpoints se manejen de forma eficiente y segura. Al mismo tiempo, logramos implementar un modelo de Clean Architecture, lo cual asegura una organización óptima y una clara separación de archivos, funcionalidades, modelos, servicios, constantes y widgets. Esta estructura modular es esencial para un mantenimiento más ágil, permitiendo que los desarrolladores trabajen en diferentes áreas sin interferir en otras, mejorando así la productividad y reduciendo posibles conflictos en el código.

Dentro del contexto de Profiles, diseñamos una página de perfil que permite a los usuarios visualizar y gestionar sus atributos y datos personales. Los usuarios pueden acceder a un botón de edición de perfil que les otorga la capacidad de modificar sus datos de manera dinámica, facilitando la actualización de su información en cualquier momento según sus necesidades. Además, se añadió un menú de ajustes completo que permite al usuario personalizar su experiencia, incluyendo opciones para editar datos personales importantes, como correos electrónicos y números de teléfono. También se incluyen ajustes avanzados de privacidad y preferencias de visualización, ofreciendo al usuario un control detallado sobre cómo se muestra y maneja su información. Para brindar una experiencia completa, esta sección también cuenta con opciones que permiten cerrar sesión o, si el usuario así lo desea, eliminar su cuenta de forma segura y definitiva.

En cuanto a IAM, se realizaron optimizaciones significativas en el rendimiento de las funciones de autenticación y autorización, lo cual es esencial para una experiencia de usuario fluida y segura. Además, se añadieron estados específicos que gestionan cada etapa del proceso de inicio de sesión, registro y recuperación de cuenta, garantizando que las interacciones del usuario sean rápidas y seguras. Se incluyó una pantalla de términos y condiciones, y se habilitó la opción de inicio de sesión mediante cuentas externas, permitiendo una integración con servicios de autenticación populares que facilitan el acceso y reducen la fricción en el proceso de registro. Estas mejoras no solo fortalecen la seguridad del sistema, sino que también amplían la accesibilidad para usuarios que prefieren utilizar sus cuentas existentes.

En el contexto de Roadmaps, se añadió la funcionalidad para que el usuario pueda crear y personalizar manualmente un roadmap. Esta creación es facilitada mediante prompts que guían al usuario a lo largo del proceso, permitiéndole estructurar sus metas y pasos a seguir de manera clara y precisa. Adicionalmente, se integró un asesor de inteligencia artificial que proporciona recomendaciones inteligentes para la planificación de los roadmaps, ofreciendo sugerencias adaptativas que ayudan al usuario a optimizar su plan de acuerdo con sus necesidades y objetivos específicos. Otras mejoras incluyeron la posibilidad de modificar nodos individuales en un roadmap, lo cual brinda flexibilidad al usuario para realizar cambios específicos sin necesidad de reconstruir el roadmap completo. Asimismo, se habilitó la opción de eliminar roadmaps y se implementó una pantalla donde el usuario puede acceder a todos los roadmaps generados, permitiéndole seleccionar y gestionar fácilmente aquellos que están almacenados en su cuenta.

Este conjunto de desarrollos en el Sprint 2 proporciona una base sólida, versátil y escalable para los siguientes sprints, asegurando que la aplicación no solo cumpla con los requisitos actuales, sino que esté preparada para incorporar nuevas funcionalidades y adaptarse a las necesidades cambiantes de los usuarios. Cada uno de estos avances contribuye a mejorar la cohesión del sistema, maximizar la eficiencia del código y garantizar una experiencia de usuario enriquecedora, intuitiva y confiable.

#### 5.2.2.6 Services Documentation Evidence for Sprint Review. 

En esta sección se detalla la relación de los Endpoints documentados mediante la especificación OpenAPI, los cuales están directamente relacionados con el alcance del Sprint y su implementación en el proyecto Roademics, específicamente por las áreas del BackEnd. Estos Endpoints son fundamentales para el funcionamiento de las funcionalidades desarrolladas durante el Sprint 2 del FrontEnd y describen la interacción entre el BackEnd y la aplicación móvil.

Se incluirán aquellos Endpoints que están directamente conectados con las funcionalidades incorporadas en la aplicación móvil durante este Sprint 2.

A continuación, se presenta una tabla exhaustiva que especifica las acciones soportadas por cada Endpoint, destacando el verbo HTTP correspondiente (GET, POST, PUT, DELETE, PATCH) y proporcionando la sintaxis exacta para realizar las llamadas. También se detallan los parámetros que pueden ser incluidos, junto con ejemplos prácticos de cada solicitud. Además, se ofrece una explicación clara y precisa del response asociado, asegurando que el equipo de desarrollo y los interesados comprendan el procesamiento de las peticiones y respuestas dentro del sistema. Esta documentación es esencial para garantizar una integración fluida y efectiva entre los distintos componentes del sistema, facilitando la comunicación entre el BackEnd y el FrontEnd.

###### Tabla 27
*Tabla del modelo de escritura para el Bounded Context de ####*
| Método  | Descripción                                  | Ejemplo de llamada         | Parámetros                                     | Respuesta                                                                                 |
|---------|----------------------------------------------|----------------------------|------------------------------------------------|-------------------------------------------------------------------------------------------|
| PUT     | Actualizar la información de un usuario      | PUT /usuarios/{id}          | `username`, `email`, `password`                | Usuario actualizado con los nuevos datos proporcionados.                                  |
| DELETE  | Eliminar un usuario                          | DELETE /usuarios/{id}       | `id` del usuario                               | Mensaje de confirmación de eliminación del usuario.                                        |
| GET     | Obtener detalles de un usuario específico    | GET /usuarios/{id}          | `id` del usuario                               | Detalles del usuario solicitado, incluyendo roles, fecha de registro, y demás datos.       |
| GET     | Obtener detalles de un usuario específico    | GET /usuarios/{id}          | `id` del usuario                               | Detalles del usuario solicitado, incluyendo roles, fecha de registro, y demás datos.       |
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

En esta sección detallaremos exhaustivamente el proceso de despliegue de los sistemas planificados para este Sprint, abarcando tanto la aplicación móvil como otras plataformas web asociadas. Presentaremos el proceso paso a paso, proporcionando evidencia clara en cada fase del despliegue, y explicando las características técnicas de cada plataforma utilizada para asegurar un despliegue exitoso.

Sin embargo, durante este Sprint 2, no se llegó a realizar ningún modelo de despliegue dentro de la aplicación móvil o dentro de algunos de sus componentes. Esto es debido a que la aplicación aún no presenta un estado que este lo suficientemente completado como para considerar presentarlo en un ambiente de producción. Ante la carencia de funcionalidades clave, como las secciones de networking y mejoras en la seguridad e inicio de sesión,  decidimos no realizar ningún despliegue hasta otro sprint próximo.

#### 5.2.2.8 Team Collaboration Insights during Sprint.

Durante el Sprint 2 de la sección Product Software Development & Implementation, nos enfocamos en el desarrollo colaborativo del FrontEnd de la aplicación móvil de Roademics, principalmente en los bounded context de Roadmaps y Gestión de Usuarios, donde cada miembro del equipo contribuyó con sus habilidades y conocimientos. Esta colaboración se refleja en los numerosos commits realizados en nuestro repositorio de código, los cuales están respaldados por capturas de pantalla adjuntas para una documentación detallada.

Nuestro equipo se reunió tanto en persona como virtualmente para asignar tareas y discutir la estrategia de desarrollo del proyecto. Estas reuniones fueron cruciales para clarificar nuestras responsabilidades individuales y asegurar un desempeño óptimo. Para maximizar la eficiencia, decidimos asignar a cada miembro del equipo una sección específica del FrontEnd para desarrollar, lo que nos permitió avanzar rápidamente y cumplir con los plazos establecidos.

Además, programamos sesiones regulares de brainstorming y resolución de problemas, donde compartimos ideas y abordamos cualquier duda o dificultad que surgiera durante el proceso de desarrollo. Estas reuniones fueron fundamentales para resolver obstáculos de manera efectiva y garantizar un progreso constante en la elaboración del FrontEnd de la Web Application.

###### Figura 88
*Reporte completo de contribuciones para el desarrollo del FrontEnd de la Aplicación Móvil de Roademics durante el Sprint 2 de Software Development & Implementation.*

<img src="/assets/Pulse-frontend-for-main-sprint2.png" alt="Pulse for the Main Branch in Software Development and Implementation">
<img src="/assets/img/Contributions-frontend-for-main-sprint2.png" alt=Contributions for the Main Branch in Software Development and Implementation ">
<img src="/assets/img/Individual-contributions-frontend-for-main-sprint2.png" alt="Individual Contributions for the Main Branch in Software Development and Implementation">

---

### 5.2.2. Sprint 3

En esta sección, se registrará y explicará el avance en términos de producto y trabajo colaborativo correspondiente al Sprint número 2 de la Implementación del FrontEnd. Este registro detallado documentará cada aspecto del progreso logrado, incluyendo el desarrollo de la interfaz de usuario en su página de perfil, las principales funcionalidades de Roadmaps e Inteligencia Artificial, todas las secciones referentes al networking, y el avance colectivo aportado por cada integrante del equipo de trabajo en relación con los componentes del FrontEnd y sus respectivas interacciones entre Bounded Context. Se hará hincapié en la importancia de la colaboración y la comunicación efectiva entre los miembros del equipo para alcanzar los objetivos del sprint, destacando cómo cada aportación individual contribuye al éxito colectivo del proyecto.

Todas las especificaciones y resultados presentados en esta sección se derivan del Product Backlog establecido en el Capítulo 2, en la sección de requerimientos. Este alineamiento garantiza que los desarrollos realizados durante el sprint sean consistentes con las expectativas del proyecto y contribuyan a la visión general del producto, asegurando que la interfaz cumpla con los estándares de calidad y usabilidad deseados.

#### 5.2.2.1 Sprint Planning 3.

Aqui se detallarán los puntos discutidos y analizados durante la reunión de Sprint Planning para el segundo sprint enfocado en la implementación del FrontEnd. El objetivo principal de dicha reunión fue establecer un plan estratégico y alcanzable que guíe el desarrollo de la interfaz de usuario, garantizando la incorporación de todas las funcionalidades esenciales para los usuarios. Durante el encuentro, se identificaron las tareas específicas a ejecutar, comprometiéndose a entregar un conjunto de resultados tangibles que contribuyan al progreso del proyecto, particularmente en las funcionalidades clave como la generación y edición de roadmaps, las funciones relacionadas con la gestión del perfil y datos de usuario, así como las características principales de la sección de networking.

Este enfoque asegura que todos los miembros del equipo compartan una visión común respecto a los objetivos y expectativas del sprint, lo cual es fundamental para mantener una adecuada coordinación y efectividad en el trabajo colaborativo. A lo largo de la reunión, se establecieron las características que serán desarrolladas, se definieron los plazos para cada tarea y se acordaron los criterios de aceptación correspondientes. Además, se promovió un diálogo abierto entre los integrantes del equipo, con el fin de identificar posibles desafíos y áreas de mejora, asegurando que todos los aspectos del desarrollo del FrontEnd estén alineados con las metas generales del proyecto. Esta metodología contribuye a una planificación estructurada y a una ejecución eficiente de las tareas, reforzando el compromiso del equipo con los objetivos del sprint.

###### Tabla 
*Tabla del planeamiento a profundidad del Sprint 3*
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
            <td>2024-10-12</td>
        </tr>
          <tr>
            <td>Time</td>
            <td>17:16</td>
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
            <td>Sprint 2 Review Summary</td>
            <td>Al finalizar el Sprint 2, se concretó la reunión del Sprint Review para evaluar el avance en el desarrollo del FrontEnd de nuestra aplicación. En este sprint, el objetivo principal fue el desarrollo de funciones clave en la aplicación, tales como la generación y edición de roadmaps mediante el asesor que funciona a base de inteligencia artificial, y la implementación de secciones como el perfil de usuario y mejoras en el diseño de las pantallas de networking. <br><br>La reunión fue exitosa, tanto por los avances logrados en los productos de software como por la efectiva colaboración del equipo. Se expusieron las nuevas funcionalidades, se realizaron demostraciones de la interfaz de usuario, y se recibieron comentarios útiles de los miembros del equipo y otros interesados. Este valioso intercambio de ideas permitió identificar oportunidades de mejora y ajustar las prioridades para el siguiente sprint. La colaboración y comunicación fluida durante esta revisión contribuyeron significativamente a la cohesión del equipo y aseguraron que el desarrollo del FrontEnd siguiera en línea con los objetivos generales del proyecto.</td> 
        </tr>
            <tr>
            <td>Sprint 2 Retrospective Summary</td>
            <td>Durante la Sprint Retrospective del Sprint 2, el equipo se enfocó en analizar en detalle toda la retroalimentación obtenida tras la finalización de este ciclo de proyecto. Esta evaluación profunda, tanto del desempeño colectivo como del individual, nos permitió identificar áreas críticas de mejora que resultarán esenciales para perfeccionar nuestra aplicación móvil desde la perspectiva del FrontEnd.<br><br> En este ejercicio de reflexión, surgieron diversas propuestas enfocadas en elevar la calidad del trabajo entregado y asegurar que el producto final cumpla con las expectativas de nuestros usuarios. Se abordaron temas como la mejora en el rendimiento de la aplicación y su balance con el diseño de interfaz, el uso de APIs y mejores opciones de librerías, y mejoras en el alcance y la portabilidad que presentara nuestra aplicación. Este intercambio de ideas no solo reforzó la colaboración del equipo, sino que también estableció un camino claro para los próximos sprints, asegurando que el producto final no solo presente un diseño atrayente, intuitivo y atractivo para los clientes, sino también que las funcionalidades sean accesibles, se encuentren adecuadamente organizadas, y presenten un buen rendimiento. </td>
        </tr>
            <tr>
            <td colspan="2">Sprint Goal & User Stories</td>
        </tr>
              <tr>
            <td>Sprint 2 Goal</td>
            <td>Alcanzar una métrica de cumplimiento del 100%, lo que indicará que se ha logrado todos los objetivos del sprint 2 con todas las historias de usuario y otros materiales necesarios.</td>
        </tr>
              <tr>
            <td>Sprint 2 Velocity</td>
            <td>Con el equipo para este sprint 2 decidimos aceptar 8 Story Points</td>
        </tr>
              <tr>
            <td>Sum of Story Points</td>
            <td>La suma de los Story Points para los User Stories que se están incluyendo en este Sprint 2 es 101</td>
        </tr>
    </table>

#### 5.2.2.2 Sprint Backlog 3.

En esta sección se analizará en detalle el proceso del Sprint Backlog 2, en el cual nuestro equipo concentró sus esfuerzos principalmente en el diseño de los bounded contexts de Roadmaps, Gestión de Usuarios, y en avanzar en aspectos clave de Networking. Este enfoque abarcó de manera integral la definición de cada una de las funcionalidades planteadas en las historias de usuario, además del diseño de cada actividad ya asignada y la propia interfaz.

A lo largo de este sprint, se dio prioridad a la usabilidad y a la experiencia del usuario, asegurando que cada elemento de la interfaz no solo cumpliera con los requisitos funcionales, sino que también proporcionara una navegación fluida y atractiva. Además, se realizaron sesiones de revisión y pruebas exhaustivas para verificar que las funcionalidades desarrolladas estuvieran alineadas con las expectativas del Product Backlog. Este enfoque colaborativo, centrado en el usuario, es crucial para garantizar que la solución no solo sea efectiva, sino también capaz de satisfacer las necesidades de nuestros clientes de manera óptima.

###### Tabla 59
*Tabla principal del planeamiento del Sprint Backlog 3*
<table>
        <tr>
            <td colspan="2">Sprint #</td>
            <td colspan="6">Sprint 3</td>
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
            <td>US007</td>
            <td>Agregar una foto o imagen en el perfil de usuario</td>
            <td>T08</td>
            <td>Agregar imagen de perfil de usuario</td>
            <td><strong>Como</strong> un usuario registrado en la aplicación de Roademics, <strong>quiero</strong> ser capaz de agregar una imagen o foto a mi perfil de usuario en la plataforma, siguiendo todos los formatos más adecuados, <strong>para</strong> personalizar mi cuenta y que otros usuarios puedan reconocerme fácilmente al interactuar conmigo.</td>
            <td>1 hora</td>
            <td>###</td>
            <td>Done</td>
        </tr>
          <tr>
            <td>US008</td>
            <td>Gestión de sección de biografía</td>
            <td>T09</td>
            <td>Agregar y gestionar biografía de usuario</td>
            <td><strong>Como</strong> usuario registrado en la aplicación de Roademics, <strong>quiero</strong> poder agregar, editar y eliminar mi biografía en la plataforma, <strong>para</strong> proporcionar información adicional sobre mí y personalizar mi perfil, reflejando datos relevantes para mi red de contactos.</td>
            <td>1 hora</td>
            <td>###</td>
            <td>Done</td>
        </tr>
            <tr>
            <td>US011</td>
            <td>Actualización de información personal</td>
            <td>T10</td>
            <td>Actualización de información de perfil</td>
            <td><strong>Como</strong> usuario registrado en la aplicación de Roademics, <strong>quiero</strong> poder actualizar mi información personal como nombres, apellidos, país y nacionalidad, y detalles de contacto en la plataforma, <strong>para</strong> mantener mi perfil actualizado y asegurarme de que otros usuarios puedan contactar conmigo de manera adecuada.</td>
            <td>2 horas y 30 minutos</td>
            <td>###</td>
            <td>Done</td>
        </tr>
              <tr>
            <td>US012</td>
            <td>Eliminación de una cuenta de usuario</td>
            <td>T11</td>
            <td>Eliminación de cuenta de usuario</td>
            <td><strong>Como</strong> usuario registrado en la aplicación de Roademics, <strong>quiero</strong> ser capaz de eliminar mi cuenta de la plataforma una vez me encuentre autenticado en mi perfil, <strong>para</strong> eliminar todos los datos personales asociados si ya no deseo utilizar el servicio de manera segura y permanente.</td>
            <td>1 hora</td>
            <td>###</td>
            <td>Done</td>
        </tr>
                <tr>
            <td>US013</td>
            <td>Sección de cambio de contraseña</td>
            <td>T12</td>
            <td>Página con sección de cambio de contraseña</td>
            <td><strong>Como</strong> usuario registrado en la aplicación de Roademics, <strong>quiero</strong> poder cambiar mi contraseña desde una sección específica en mi perfil, <strong>para</strong> actualizar mi contraseña de manera segura y mantener la integridad de mi cuenta a corto y largo plazo.</td>
            <td>1 hora</td>
            <td>###</td>
            <td>Done</td>
        </tr>
                  <tr>
            <td>US016</td>
            <td>Creación de roadmap académico básico</td>
            <td>T13</td>
            <td>Creación de un roadmap básico</td>
            <td><strong>Como</strong> usuario de la aplicación de Roademics interesado en planificar mi trayectoria profesional con las funciones ofrecidas, <strong>quiero</strong> crear un roadmap académico básico en la plataforma, <strong>para</strong> visualizar y gestionar mi progreso académico, planificar mis cursos y establecer metas profesionales de manera eficiente y estructurada.</td>
            <td>3 horas y 30 minutos</td>
            <td>###</td>
            <td>Done</td>
        </tr>
                    <tr>
            <td>US017</td>
            <td>Generación automática de roadmap con el uso de Inteligencia Artificial</td>
            <td>T14</td>
            <td>Creación de un roadmap básico con Inteligencia Artificial</td>
            <td><strong>Como</strong> usuario que busca optimizar su trayectoria profesional con la aplicación de Roademics, <strong>quiero</strong> que la plataforma sea capaz de generar un roadmap profesional utilizando las herramientas de inteligencia artificial que dispone, <strong>para</strong> recibir una recomendación personalizada y optimizada de cursos y objetivos que se alineen con mis metas profesionales y educativas.</td>
            <td>3 horas</td>
            <td>###</td>
            <td>Done</td>
        </tr>
                      <tr>
            <td>US018</td>
            <td>Menú de almacenamiento de Roadmaps de un usuario</td>
            <td>T15</td>
            <td>Implementar menú de almacenamiento de roadmaps personales</td>
            <td><strong>Como</strong> usuario que busca optimizar su trayectoria profesional con la aplicación de Roademics, <strong>quiero</strong> que la plataforma tenga un pequeño menú o dashboard donde se muestren todos los roadmaps u hojas de ruta que he generado en la aplicación, <strong>para</strong> tener un acceso directo a cada uno de mis roadmaps y poder almacenarlos de forma más sencilla, cómoda y organizada.</td>
            <td>2 horas</td>
            <td>###</td>
            <td>Done</td>
        </tr>
                        <tr>
            <td>US019</td>
            <td>Acceso a plantillas básicas y avanzadas para la creación de Roadmaps</td>
            <td>T16</td>
            <td>Diseño de plantillas básicas y avanzadas para la creación de Roadmaps</td>
            <td><strong>Como</strong> usuario que desea mejorar su planificación profesional con el uso de la aplicación de Roademics, <strong>quiero</strong> tener acceso a plantillas predeterminadas y avanzadas para mis hojas de rutas y roadmaps, <strong>para</strong> facilitar el desarrollo y diseño de los roadmaps de forma profesional, detallada y personalizada, que se ajuste a mis necesidades y objetivos específicos.</td>
            <td>1 hora y 30 minutos</td>
            <td>###</td>
            <td>Done</td>
        </tr>
                          <tr>
            <td>US020</td>
            <td>Edición de roadmaps básicos</td>
            <td>T17</td>
            <td>Edición de un roadmap básico</td>
            <td><strong>Como</strong> usuario que ha creado un roadmap básico en la plataforma de Roademics, <strong>quiero</strong> poder editar el roadmap existente con el uso de herramientas variadas de edición y modificación, <strong>para</strong> actualizar la información relevante, ajustar mis objetivos profesionales o académicos, y modificar mis planes según mis necesidades actuales.</td>
            <td>4 horas y 30 minutos</td>
            <td>###</td>
            <td>Done</td>
        </tr>
                            <tr>
            <td>US021</td>
            <td>Acceso a herramientas de edición avanzada de roadmaps para usuarios premium</td>
            <td>T18</td>
            <td>Desarrollo de herramientas de edición avanzada de roadmaps (Para usuarios premium)</td>
            <td><strong>Como</strong> usuario con suscripción Premium en la plataforma Roademics, <strong>quiero</strong> tener acceso a herramientas de edición avanzada para la modificación de mis roadmaps profesionales, <strong>para</strong> aprovechar funcionalidades adicionales que me permitan optimizar la planificación y gestión de mis metas, brindándome mayor flexibilidad y precisión en la creación y ajuste de mis objetivos.</td>
            <td>2 horas y 30 minutos</td>
            <td>###</td>
            <td>Done</td>
        </tr>
                              <tr>
            <td>US022</td>
            <td>Eliminación de Roadmaps</td>
            <td>T19</td>
            <td>Eliminación de Roadmaps</td>
            <td><strong>Como</strong> usuario registrado en la plataforma Roademics, <strong>quiero</strong> poder eliminar roadmaps que ya no necesito, <strong>para</strong> mantener mi perfil organizado, optimizar el uso de la plataforma y evitar la acumulación de información obsoleta o irrelevante.</td>
            <td>1 hora y 30 minutos</td>
            <td>###</td>
            <td>Done</td>
        </tr>
                                <tr>
            <td>US023</td>
            <td>Visualizar limitaciones respecto a la cantidad de roadmaps que el usuario podrá gestionar</td>
            <td>T20</td>
            <td>Visualización de limitaciones de la cantidad de roadmaps que cada usuario puede gestionar</td>
            <td><strong>Como</strong> usuario registrado de Roademics, <strong>quiero</strong> visualizar las limitaciones respecto a la cantidad de roadmaps que puedo gestionar dentro de la sección de organización de roadmaps, <strong>para</strong> tener un control claro y transparente sobre el número de roadmaps que puedo crear y editar, asegurándome de no sobrepasar los límites establecidos por mi plan de suscripción o la configuración de la misma plataforma.</td>
            <td>1 hora y 30 minutos</td>
            <td>###</td>
            <td>Done</td>
        </tr>
                                  <tr>
            <td>US024</td>
            <td>Recibir análisis avanzados sobre un Roadmap en específico para los usuarios premium</td>
            <td>T21</td>
            <td>Análisis avanzado sobre un Roadmap en específico para los usuarios premium</td>
            <td><strong>Como</strong> usuario Premium de la plataforma Roademics, <strong>quiero</strong> recibir análisis avanzados y detallados sobre el progreso y la estructura de mi roadmap profesional, <strong>para</strong> obtener información valiosa que me permita identificar áreas de mejora, optimizar mi planificación, y tomar decisiones informadas que me ayuden a alcanzar mis objetivos profesionales de manera más efectiva y eficiente.</td>
            <td>3 horas</td>
            <td>###</td>
            <td>Done</td>
        </tr>
                                    <tr>
            <td>US025</td>
            <td>Poder exportar mi roadmaps en formato como PDF o PNG</td>
            <td>T22</td>
            <td>Exportar roadmaps en formato PDF o PNG</td>
            <td><strong>Como</strong> usuario premium de la plataforma Roademics, <strong>quiero</strong> poder exportar mis roadmaps generados y editados mediante formatos de archivo como PDF o PNG, <strong>para</strong> disponer de una copia accesible, portable y presentable de mis planes profesionales, que pueda ser utilizada para compartir, almacenar o imprimir con facilidad y conservar la integridad del diseño visual y la información estructurada en la plataforma.</td>
            <td>2 horas</td>
            <td>###</td>
            <td>Done</td>
        </tr>
                                    <tr>
            <td>US026</td>
            <td>Poder crear los nodos de mi roadmap</td>
            <td>T23</td>
            <td>Creación de nodos de un roadmap</td>
            <td><strong>Como</strong> usuario registrado de la plataforma Roademics, <strong>quiero</strong> poder crear los nodos de mi roadmap de forma manual, <strong>para</strong> estructurar y definir claramente las etapas, actividades y acciones necesarias para alcanzar mis objetivos profesionales de manera organizada y efectiva.</td>
            <td>3 horas</td>
            <td>###</td>
            <td>Done</td>
        </tr>
                                      <tr>
            <td>US027</td>
            <td>Recibir notificación si un nodo en mi grafo se vuelve obsoleto o ya no está disponible</td>
            <td>T24</td>
            <td>Notificar si un nodo en un grafo se vuelve obsoleto o ya no se encuentra disponible</td>
            <td><strong>Como</strong> usuario registrado en la plataforma Roademics, <strong>quiero</strong> recibir una notificación si un nodo en mi grafo se vuelve obsoleto o ya no está disponible, <strong>para</strong> estar al tanto de cualquier cambio que pueda afectar la estructura y el progreso de mi roadmap, y tomar las medidas necesarias para actualizar o ajustar mi plan según sea necesario.</td>
            <td>2 horas</td>
            <td>###</td>
            <td>Done</td>
        </tr>
                                        <tr>
            <td>US028</td>
            <td>Guardar versiones de mi roadmap</td>
            <td>T25</td>
            <td>Historial de versiones de un roadmap</td>
            <td><strong>Como</strong> usuario registrado en la plataforma Roademics, <strong>quiero</strong> ser capaz de guardar distintas versiones de mi roadmap, <strong>para</strong> tener un historial de cambios y poder revertir a versiones anteriores si es necesario, asegurando así que pueda realizar ajustes sin perder progresos importantes.</td>
            <td>2 horas y 30 minutos</td>
            <td>###</td>
            <td>Done</td>
        </tr>
    </table>

#### 5.2.2.3 Development Evidence for Sprint Review.

En esta sección se explicarán y presentarán los avances obtenidos en la implementación, relacionados con los productos de la solución según el alcance definido para el Sprint 2 de la sección de Product Implementation. El enfoque de este apartado será documentar cada uno de los commits ya implementados dentro del repositorio de GitHub, proporcionando detalles técnicos de los cambios realizados y su impacto en el desarrollo de la aplicación móvil junto a todas sus funcionalidades por parte de la interfaz.

###### Tabla XX
*Tabla de los commits realizados y relacionados con el desarrollo de todas las secciones del Sprint Backlog 2*
| Repository | Branch| Commit Id| Commit Message| Commit Message Body|Commited on (Date) |
|------------|-------|----------|---------------|--------------------|-------------------|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-Roademics|profile-feature|fcd14b9127bccf8dce545dfaff8e439c2dde91c7|chore: create clean architecture folder structure and add app_constants|committed :)| 25/10/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-Roademics|profile-feature|11e89700dd38ae8f9b45e8f598a3278a1e746222|chore: add placeholder for team collaboration|committed :)| 26/10/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-Roademics|profile-feature|f3e95111ef5f8264cb4c28fbbc2ee7adb46545a0|chore: add more placeholders |committed :)| 26/10/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-Roademics|profile-feature|5d323f549767b421e31f61af7bddf5f281371054|feat: add profile page, edit profile, settings page |committed :)| 26/10/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-Roademics|profile-feature|fbb9f26790c7ee08a44aae50b4e9de868ab08fba|feat: add update email settings page |committed :)| 26/10/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-Roademics|profile-feature|65bf6314c46c88c58692c652b8e5e4d69078278d|feat: add update phone number page |committed :)| 26/10/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-Roademics|profile-feature|1dd12af8610363edb885b11be93bf78585066d2f|feat: add change password page|committed :)| 26/10/24|
|upc-pre-202402-cc-238-WV61-WeHaveAnIdea-Roademics|profile-feature|d4dc95c6b813259b32fba6ab146dbc2a8aaa7f21|feat: add delete account function|committed :)| 26/10/24|

#### 5.2.2.4 Testing Suite Evidence for Sprint Review. 

En esta sección presentaremos una evidencia detallada de las rigurosas pruebas realizadas durante el sprint, con el fin de garantizar la calidad y la funcionalidad del producto en desarrollo. Hemos implementado la metodología Gherkin, que permite definir escenarios de prueba de manera clara y concisa, facilitando la comprensión tanto para los desarrolladores como para los interesados no técnicos.

Cada uno de estos escenarios de prueba ha sido meticulosamente registrado en commits específicos dentro de nuestro repositorio de código, lo que asegura un historial completo, detallado y transparente del proceso de prueba. Este enfoque no solo permite rastrear fácilmente los cambios y correcciones asociados a las pruebas, sino que también garantiza que las funcionalidades clave del sistema cumplan con los criterios de aceptación definidos. La metodología adoptada refuerza la integridad del código y la entrega de un producto final robusto y confiable.

###### Tabla 26
*Tabla de los modelos de pruebas realizados y relacionados con el desarrollo de todas las secciones del Sprint Backlog 1*
| Repository                        | Branch              | Commit Id                          | Commit Message                   | Commit Message Body           |Commited on (Date) |
|-----------------------------------|---------------------|------------------------------------|----------------------------------|-------------------------------|-------------------|
| upc-pre-202402-cc-238-WV61-WeHaveAnIdea-AcceptanceTests | Sprint-1 | 5198ddb8114acf692f93d46e0224c8652529b5dc | feat: add US_Sprint1.feature | En esta sección se implementaron todos los Acceptance Test para el Sprint 1 del backend de Roademics | 28/09/24 |
| upc-pre-202402-cc-238-WV61-WeHaveAnIdea-AcceptanceTests | Sprint-1 | 7990a48a9b476d87cdcd98de0535f2b07b2644d1 | feat: add TS013-TS017 y TS27-TS040 |En esta sección se implementaron todos los Acceptance Test para el Sprint 1 del backend de Roademics | 28/09/24 |
| upc-pre-202402-cc-238-WV61-WeHaveAnIdea-AcceptanceTests | Sprint-1 | e7e7f030e2b31007d0f9daf82fecc1889569c491 | feat: add US_Sprint1_Frontend |En esta sección se implementaron todos los Acceptance Test para el Sprint 1 del Frontend de Roademics | 28/09/24 |

#### 5.2.2.5 Execution Evidence for Sprint Review. 

Durante el desarrollo de este Sprint 2, en el área de Product Implementation y FrontEnd, nuestro equipo se enfocó en implementar las funcionalidades centrales de los bounded contexts de IAM (Identity and Access Management), Profiles y Roadmaps. Este esfuerzo fue fundamental para asegurar que la aplicación cumpla con los principales requisitos funcionales, siguiendo prácticas avanzadas de desarrollo y una estructura sólida que facilite el crecimiento y la escalabilidad del proyecto en sprints futuros. La implementación de estas funcionalidades no solo marca un hito en la creación de una base estable para la aplicación, sino que también nos permite seguir avanzando con las características adicionales que enriquecerán la experiencia del usuario.

En términos de arquitectura de desarrollo, optamos por un modelo Bloc para gestionar el estado en cada bounded context de manera independiente, permitiendo un control más efectivo del flujo de datos y la reactividad en cada componente de la aplicación. Además, adoptamos un patrón de repositorio, lo que facilita la conexión fluida con el Backend de Roademics y asegura que las solicitudes a los Endpoints se manejen de forma eficiente y segura. Al mismo tiempo, logramos implementar un modelo de Clean Architecture, lo cual asegura una organización óptima y una clara separación de archivos, funcionalidades, modelos, servicios, constantes y widgets. Esta estructura modular es esencial para un mantenimiento más ágil, permitiendo que los desarrolladores trabajen en diferentes áreas sin interferir en otras, mejorando así la productividad y reduciendo posibles conflictos en el código.

Dentro del contexto de Profiles, diseñamos una página de perfil que permite a los usuarios visualizar y gestionar sus atributos y datos personales. Los usuarios pueden acceder a un botón de edición de perfil que les otorga la capacidad de modificar sus datos de manera dinámica, facilitando la actualización de su información en cualquier momento según sus necesidades. Además, se añadió un menú de ajustes completo que permite al usuario personalizar su experiencia, incluyendo opciones para editar datos personales importantes, como correos electrónicos y números de teléfono. También se incluyen ajustes avanzados de privacidad y preferencias de visualización, ofreciendo al usuario un control detallado sobre cómo se muestra y maneja su información. Para brindar una experiencia completa, esta sección también cuenta con opciones que permiten cerrar sesión o, si el usuario así lo desea, eliminar su cuenta de forma segura y definitiva.

En cuanto a IAM, se realizaron optimizaciones significativas en el rendimiento de las funciones de autenticación y autorización, lo cual es esencial para una experiencia de usuario fluida y segura. Además, se añadieron estados específicos que gestionan cada etapa del proceso de inicio de sesión, registro y recuperación de cuenta, garantizando que las interacciones del usuario sean rápidas y seguras. Se incluyó una pantalla de términos y condiciones, y se habilitó la opción de inicio de sesión mediante cuentas externas, permitiendo una integración con servicios de autenticación populares que facilitan el acceso y reducen la fricción en el proceso de registro. Estas mejoras no solo fortalecen la seguridad del sistema, sino que también amplían la accesibilidad para usuarios que prefieren utilizar sus cuentas existentes.

En el contexto de Roadmaps, se añadió la funcionalidad para que el usuario pueda crear y personalizar manualmente un roadmap. Esta creación es facilitada mediante prompts que guían al usuario a lo largo del proceso, permitiéndole estructurar sus metas y pasos a seguir de manera clara y precisa. Adicionalmente, se integró un asesor de inteligencia artificial que proporciona recomendaciones inteligentes para la planificación de los roadmaps, ofreciendo sugerencias adaptativas que ayudan al usuario a optimizar su plan de acuerdo con sus necesidades y objetivos específicos. Otras mejoras incluyeron la posibilidad de modificar nodos individuales en un roadmap, lo cual brinda flexibilidad al usuario para realizar cambios específicos sin necesidad de reconstruir el roadmap completo. Asimismo, se habilitó la opción de eliminar roadmaps y se implementó una pantalla donde el usuario puede acceder a todos los roadmaps generados, permitiéndole seleccionar y gestionar fácilmente aquellos que están almacenados en su cuenta.

Este conjunto de desarrollos en el Sprint 2 proporciona una base sólida, versátil y escalable para los siguientes sprints, asegurando que la aplicación no solo cumpla con los requisitos actuales, sino que esté preparada para incorporar nuevas funcionalidades y adaptarse a las necesidades cambiantes de los usuarios. Cada uno de estos avances contribuye a mejorar la cohesión del sistema, maximizar la eficiencia del código y garantizar una experiencia de usuario enriquecedora, intuitiva y confiable.

#### 5.2.2.6 Services Documentation Evidence for Sprint Review. 

En esta sección se detalla la relación de los Endpoints documentados mediante la especificación OpenAPI, los cuales están directamente relacionados con el alcance del Sprint y su implementación en el proyecto Roademics, específicamente por las áreas del BackEnd. Estos Endpoints son fundamentales para el funcionamiento de las funcionalidades desarrolladas durante el Sprint 2 del FrontEnd y describen la interacción entre el BackEnd y la aplicación móvil.

Se incluirán aquellos Endpoints que están directamente conectados con las funcionalidades incorporadas en la aplicación móvil durante este Sprint 2.

A continuación, se presenta una tabla exhaustiva que especifica las acciones soportadas por cada Endpoint, destacando el verbo HTTP correspondiente (GET, POST, PUT, DELETE, PATCH) y proporcionando la sintaxis exacta para realizar las llamadas. También se detallan los parámetros que pueden ser incluidos, junto con ejemplos prácticos de cada solicitud. Además, se ofrece una explicación clara y precisa del response asociado, asegurando que el equipo de desarrollo y los interesados comprendan el procesamiento de las peticiones y respuestas dentro del sistema. Esta documentación es esencial para garantizar una integración fluida y efectiva entre los distintos componentes del sistema, facilitando la comunicación entre el BackEnd y el FrontEnd.

###### Tabla 27
*Tabla del modelo de escritura para el Bounded Context de ####*
| Método  | Descripción                                  | Ejemplo de llamada         | Parámetros                                     | Respuesta                                                                                 |
|---------|----------------------------------------------|----------------------------|------------------------------------------------|-------------------------------------------------------------------------------------------|
| PUT     | Actualizar la información de un usuario      | PUT /usuarios/{id}          | `username`, `email`, `password`                | Usuario actualizado con los nuevos datos proporcionados.                                  |
| DELETE  | Eliminar un usuario                          | DELETE /usuarios/{id}       | `id` del usuario                               | Mensaje de confirmación de eliminación del usuario.                                        |
| GET     | Obtener detalles de un usuario específico    | GET /usuarios/{id}          | `id` del usuario                               | Detalles del usuario solicitado, incluyendo roles, fecha de registro, y demás datos.       |
| GET     | Obtener detalles de un usuario específico    | GET /usuarios/{id}          | `id` del usuario                               | Detalles del usuario solicitado, incluyendo roles, fecha de registro, y demás datos.       |
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

En esta sección detallaremos exhaustivamente el proceso de despliegue de los sistemas planificados para este Sprint, abarcando tanto la aplicación móvil como otras plataformas web asociadas. Presentaremos el proceso paso a paso, proporcionando evidencia clara en cada fase del despliegue, y explicando las características técnicas de cada plataforma utilizada para asegurar un despliegue exitoso.

Sin embargo, durante este Sprint 2, no se llegó a realizar ningún modelo de despliegue dentro de la aplicación móvil o dentro de algunos de sus componentes. Esto es debido a que la aplicación aún no presenta un estado que este lo suficientemente completado como para considerar presentarlo en un ambiente de producción. Ante la carencia de funcionalidades clave, como las secciones de networking y mejoras en la seguridad e inicio de sesión,  decidimos no realizar ningún despliegue hasta otro sprint próximo.

#### 5.2.2.8 Team Collaboration Insights during Sprint.

Durante el Sprint 2 de la sección Product Software Development & Implementation, nos enfocamos en el desarrollo colaborativo del FrontEnd de la aplicación móvil de Roademics, principalmente en los bounded context de Roadmaps y Gestión de Usuarios, donde cada miembro del equipo contribuyó con sus habilidades y conocimientos. Esta colaboración se refleja en los numerosos commits realizados en nuestro repositorio de código, los cuales están respaldados por capturas de pantalla adjuntas para una documentación detallada.

Nuestro equipo se reunió tanto en persona como virtualmente para asignar tareas y discutir la estrategia de desarrollo del proyecto. Estas reuniones fueron cruciales para clarificar nuestras responsabilidades individuales y asegurar un desempeño óptimo. Para maximizar la eficiencia, decidimos asignar a cada miembro del equipo una sección específica del FrontEnd para desarrollar, lo que nos permitió avanzar rápidamente y cumplir con los plazos establecidos.

Además, programamos sesiones regulares de brainstorming y resolución de problemas, donde compartimos ideas y abordamos cualquier duda o dificultad que surgiera durante el proceso de desarrollo. Estas reuniones fueron fundamentales para resolver obstáculos de manera efectiva y garantizar un progreso constante en la elaboración del FrontEnd de la Web Application.

###### Figura 88
*Reporte completo de contribuciones para el desarrollo del FrontEnd de la Aplicación Móvil de Roademics durante el Sprint 2 de Software Development & Implementation.*

<img src="/assets/Pulse-frontend-for-main-sprint2.png" alt="Pulse for the Main Branch in Software Development and Implementation">
<img src="/assets/img/Contributions-frontend-for-main-sprint2.png" alt=Contributions for the Main Branch in Software Development and Implementation ">
<img src="/assets/img/Individual-contributions-frontend-for-main-sprint2.png" alt="Individual Contributions for the Main Branch in Software Development and Implementation">

---

## 5.3. Validation Interviews

En esta sección, nuestro equipo documentará y describirá las actividades vinculadas a las entrevistas de validación realizadas durante el proyecto. Las entrevistas de validación son esenciales, ya que permiten a los usuarios de los segmentos objetivo interactuar tanto con la página web de presentación de la aplicación, así como con la propia aplicación móvil. Estas interacciones brindan información valiosa sobre la experiencia del usuario y la eficacia del diseño. Para asegurar un proceso de validación eficiente, es importante emplear el formato de evaluación heurística desarrollado específicamente para este proyecto. Este formato establece una estructura para analizar la usabilidad y la experiencia del usuario, garantizando que se aborden los aspectos clave para mejorar el diseño y funcionamiento de las aplicaciones (Papalia, 2024).

### 5.3.1. Diseño de Entrevistas

El equipo se encarga de definir, para cada segmento de público identificado, los elementos que deben incluirse en la sesión de validación. Esto incluye tanto el análisis de la página de destino como de las aplicaciones móviles asociadas. Además, se describe el diseño de los flujos de usuario de las aplicaciones, que jugarán un papel fundamental en el proceso de validación. Estos flujos de usuario, que representan la secuencia de acciones que los usuarios realizarán dentro de las aplicaciones, son esenciales para asegurar una experiencia de usuario óptima. De esta forma, se garantiza que cada paso que da el usuario en las aplicaciones sea coherente, intuitivo y esté alineado con los objetivos de diseño establecidos.

Preguntas generales iniciales:

1. ¿Podría indicarnos su nombre completo, por favor?
2. ¿Podría compartir su edad?
3. ¿Había tenido algún contacto previo con nuestra startup antes de esta entrevista?

Preguntas generales sobre la aplicación:

1. ¿Cuál fue su primera impresión al utilizar la aplicación? ¿La encontró intuitiva y fácil de usar?
2. ¿Experimentó algún inconveniente durante su uso? En caso afirmativo, ¿podría describirlo?
3. ¿Recomendaría la aplicación a otros usuarios? ¿Por qué?

Segmento 1: Profesionales formados y en desarrollo que deseen potenciarse planificando su futuro.

1. ¿Considera adecuado el nivel de asesoría proporcionado por la inteligencia artificial de la aplicación?
2. ¿Le parece útil organizar logros, habilidades y metas a través de hojas de ruta? ¿Tiene alguna sugerencia para mejorar esta presentación?
3. ¿Qué tan sencillo fue crear su primer roadmap dentro de la aplicación?
4. ¿Cuáles herramientas del aplicativo fueron las más útiles para sus necesidades profesionales? ¿Por qué?
5. ¿Opina que los modelos de perfiles profesionales ofrecidos en la aplicación reflejan el mercado laboral actual?
6. ¿Cree que la presentación de hojas de ruta es atractiva para las empresas actuales? ¿Consideraría agregar un roadmap adecuado a su curriculum vitae?
7. ¿Piensa que podría lograr una oportunidad laboral estable utilizando solo las funcionalidades de la plataforma?
8. ¿Le parecen efectivas las funciones de networking que ofrece la aplicación? Si estuviera postulando a un empleo, ¿preferiría los medios de comunicación de la aplicación o utilizaría otro canal? ¿Por qué?
9. ¿Cómo compara nuestra plataforma con otras en términos de usabilidad, innovación y calidad en la presentación de información?
10. ¿Qué mejoras o nuevas funcionalidades le gustaría ver en la plataforma y por qué considera que serían relevantes?

Segmento 2: Empresas y Reclutadores en busca de personal capacitado.

1. ¿Considera que el perfil empresarial en la aplicación facilita la búsqueda de candidatos adecuados para sus necesidades de contratación?
2. ¿Cómo evalúa la utilidad de los mapas de ruta profesionales para comunicar los requisitos de habilidades y competencias a los candidatos?
3. ¿Qué tan efectiva considera que es la plataforma para identificar talento que esté alineado con las demandas de su empresa?
4. ¿Encuentra que las herramientas de filtrado de candidatos en la aplicación son precisas y adecuadas? ¿Qué aspectos mejoraría?
5. ¿Le parece útil la visualización de perfiles de candidatos que siguen rutas similares a las requeridas por su organización?
6. ¿Considera que el modelo de networking dentro de la aplicación facilita las conexiones con candidatos relevantes y de alto potencial?
7. ¿La función de creación de perfiles profesionales en Roademics ayuda a su empresa a identificar habilidades y experiencias clave en los candidatos?
8. ¿Qué tan adecuado encuentra el modelo Freemium para su empresa en términos de funcionalidad y acceso a opciones avanzadas de reclutamiento?
9. ¿De qué manera considera que la aplicación podría optimizar el proceso de selección de candidatos en relación con otras herramientas de reclutamiento que haya utilizado?
10. ¿Qué funcionalidades adicionales le gustaría ver en la plataforma para hacer más eficiente la contratación de personal capacitado?

### 5.3.2. Registro de Entrevistas de Validación

#### Segmento 1: Profesionales en Desarrollo y Futuros Profesionales que quieran visualizar su propio roadmap

**Entrevista N°1:**

###### Figura #
*Imagen de presentación de la primera entrevista realizada*

<img src="/assets/img/capitulo-2/interviews/records/entrevista1-segmento1.png" alt="Primera entrevista de validación de nuestro segmento objetivo 1 a Fernando Lizano Coll Cardenas." width="550" height="300">

**Datos principales:**
- Nombre completo del entrevistado: Fernando Lizano Coll Cardenas
- Edad: 19 años
- Distrito: Punta Hermosa
- Link: [Entrevista a Fernando Lizano](https://upcedupe-my.sharepoint.com/:v:/g/personal/u20221c936_upc_edu_pe/EQ3et4X8YHZNhSyy5eJO0UEBT8bMiopqemAQs5_TLl4_eg?e=p6B8JK&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D)
- Inicio de la entrevista: [0:50](https://upcedupe-my.sharepoint.com/:v:/g/personal/u20221c936_upc_edu_pe/EQ3et4X8YHZNhSyy5eJO0UEBPj6r0v3Cyv0xSaHuJNK4Wg?e=5uuGOI&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifSwicGxheWJhY2tPcHRpb25zIjp7InN0YXJ0VGltZUluU2Vjb25kcyI6NTAuNDd9fQ%3D%3D)
- Duración: 7 minutos y 3 segundos
- Entrevistador: Pescorán Angulo, Juan Fabritzzio
- Resumen de Entrevista: Fernando Lizano, un estudiante de 19 años de ingeniería, aún no trabaja pero está en búsqueda de mejorar su perfil académico, el cual considera insuficiente. Aspira a aprender más y planea su ruta de aprendizaje identificando áreas a mejorar y buscando cursos, certificados y proyectos relevantes. Reconoce la importancia de las herramientas digitales y plataformas de aprendizaje para acceder a conocimientos especializados y mantenerse actualizado. Utiliza LinkedIn para compartir logros académicos y construir una red de contactos, y emplea tanto LinkedIn como Computrabajo para informarse sobre vacantes laborales. A la hora de evaluar una vacante, prioriza que sus habilidades coincidan con los requisitos del puesto y valora mucho la claridad de las empresas sobre las aptitudes y características que buscan en los candidatos, lo que le permite prepararse mejor y evaluar su idoneidad para el puesto.

**Entrevista N°2:**

###### Figura 7
*Imagen de presentación de la segunda entrevista de validación realizada*

<img src="/assets/img/capitulo-2/interviews/records/entrevista2-segmento1.png" alt="Segunda entrevista de validación de nuestro segmento objetivo 1 a Jeremías Evangelista Pescorán." width="550" height="300">

**Datos principales:**
- Nombre completo del entrevistado: Jeremías Evangelista Pescorán
- Edad: 24 años
- Distrito: San Juan de Miraflores
- Link: [Entrevista a Jeremías Pescorán](https://upcedupe-my.sharepoint.com/:v:/g/personal/u20221c936_upc_edu_pe/EeXCuqUCgQdLopDzDo2lLDYBJFH9E50qUI9ggXCdqQ34BA?e=wqC7a7&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D)
- Inicio de la entrevista: [0:36](https://upcedupe-my.sharepoint.com/:v:/g/personal/u20221c936_upc_edu_pe/EeXCuqUCgQdLopDzDo2lLDYB2eeMYRKCr-PIywsgNbn1_w?e=pWvjTx&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifSwicGxheWJhY2tPcHRpb25zIjp7InN0YXJ0VGltZUluU2Vjb25kcyI6MzUuNjl9fQ%3D%3D)
- Duración: 7 minutos y 33 segundos
- Entrevistador: Pescorán Angulo, Juan Fabritzzio
- Resumen de Entrevista: Jeremías Evangelista, un ingeniero de software de 24 años, trabaja como analista programador junior especializado en desarrollo backend. Está satisfecho con su formación académica y busca continuamente mejorar aprendiendo nuevas tecnologías como AWS y Azure, utilizando recursos en línea como YouTube y Udemy. Valora mucho las herramientas digitales en su desarrollo profesional y utiliza LinkedIn para compartir logros académicos. Al evaluar vacantes laborales, se enfoca en el salario y los lenguajes de programación requeridos, prefiriendo empresas que sean transparentes sobre sus expectativas para evitar cargas de trabajo inesperadas.

---

#### Segmento 2: Empresas y Reclutadores en busca de personal capacitado

**Entrevista N°3:**

###### Figura #
*Imagen de presentación de la tercera entrevista de validación realizada*

<img src="/assets/img/capitulo-2/interviews/records/entrevista1-segmento2.png" alt="Primera entrevista de nuestro segmento objetivo 2 a Rosa Castro." width="400" height="200">

**Datos principales:**
- Nombre completo del entrevistado: Rosa Castro
- Edad: 32
- Distrito: Ate
- Link: [Entrevista a Rosa Castro](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202213143_upc_edu_pe/Ef9SImimiAlJlFlY3Ok3KX8Bfc6B1rQUYzOfsc8gjdv3yA?e=kFSeXY&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D)
- Inicio de la entrevista: 0:01 
- Duración: 10:56
- Entrevistador: Lucio Yen
- Resumen de Entrevista: Rosa Castro es administradora y coordinadora de Mastercol. Ella da mayor importancia a las habilidades blandas, como la comunicación y la adaptabilidad, en lugar de enfocarse en las habilidades técnicas y la actitud. Para este proceso, Rosa utiliza plataformas como LinkedIn, Facebook, y WhatsApp para obtener información, aunque principalmente confía en referencias laborales obtenidas a través de llamadas telefónicas. En Mastercol, se fomenta el desarrollo continuo de los empleados mediante capacitaciones e incentivos. Cuando un empleado solicita un aumento de sueldo, el impacto que ha tenido en la empresa es un factor determinante en la decisión y también el aprendizaje. Jennifer considera que, si se cuenta con los recursos, es esencial seguir aprendiendo. En su empresa, los despidos son raros y generalmente se deben a bajo rendimiento o al incumplimiento de las normas. 

**Entrevista N°5:**

###### Figura 10
*Imagen de presentación de la quinta entrevista realizada.*

<img src="/assets/img/capitulo-2//interviews/records/entrevista2-segmento2.png" alt="Segunda entrevista de nuestro segmento objetivo 2 a Jennifer Villanueva." width="400" height="200">


**Datos principales:**
- Nombre completo del entrevistado: Jennifer Villanueva
- Edad: 40
- Distrito: Ate
- Link: [Entrevista a Jennifer Villanueva](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202213143_upc_edu_pe/EZTB2EPF2GNNotCvw7IUgUUBly041VIbMyI-vXRE0jOn6g?e=bz4A3v&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D)
- Inicio de la entrevista: 0:02
- Duración: 10:42
- Entrevistador: Lucio Yen
- Resumen de Entrevista: Jennifer Villanueva, gerenta de recursos humanos en Mastercol, es imprescindible en la selección de personal, donde prioriza las habilidades blandas como la comunicación y adaptabilidad sobre las técnicas y la actitud. Para este proceso, utiliza plataformas como LinkedIn, Facebook y WhatsApp para informarse, pero sobre todo, utiliza referencias laborales llamando por teléfono. Por otro lado, la empresa donde trabaja Jennifer fomenta el desarrollo continuo de los empleados a través de capacitaciones e incentivos. Cuando un empleado solicita un aumento, el impacto dentro de la empresa en un factor crucial para decidir. Por último, considera que los profesionales no deberían de dejar de aprender nunca y que los despidos de la empresa van por mal rendimiento y incumplimiento de normas.

**Entrevista N°6:**

###### Figura 11
*Imagen de presentación de la sexta entrevista realizada.*

<img src="/assets/img/capitulo-2/interviews/records/entrevista3-segmento2.png" alt="Tercera entrevista de nuestro segmento objetivo 2 a Ximena Vilchez Paredes." width="400" height="200">

**Datos principales:**
- Nombre completo del entrevistado: Ximena Vilchez Paredes
- Edad: 22
- Distrito: Chorrillos
- Link: [Entrevista](https://upcedupe-my.sharepoint.com/:v:/g/personal/u20201f572_upc_edu_pe/EWm0xNl3QBVHvJNcCJPjZjsBQdiu3tylQ7EwoyLJcHZ9Kg?e=ey6qll&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D)
- Inicio de la entrevista: 0:01
- Duración: 11:19
- Entrevistador: Aldhair Valenzuela
- Resumen de Entrevista: Ximena Vilchez, abogada en un estudio jurídico privado, juega un rol clave en la selección de personal, donde prioriza las habilidades blandas como la comunicación y adaptabilidad sobre las técnicas. Para este proceso, utiliza plataformas como LinkedIn, Facebook y WhatsApp, destacando su adaptación a las herramientas digitales. Además, la empresa donde trabaja Ximena fomenta el desarrollo continuo de los empleados a través de una biblioteca interna y organiza exposiciones sobre cambios legales importantes, promoviendo el aprendizaje colectivo. Cuando un empleado solicita un aumento, la eficiencia en sus labores es un factor crucial en la decisión.

### 5.3.3. Evaluaciones según heurísticas

En esta sección se detalla el proceso minucioso de evaluación de las sesiones de validación, fundamentado en un conjunto de heurísticas diseñadas para cubrir los aspectos más relevantes de la experiencia del usuario. Estas heurísticas se organizan en categorías clave que incluyen criterios de usabilidad, arquitectura de la información y elementos del diseño de experiencia. Cada categoría ha sido cuidadosamente definida para proporcionar un análisis riguroso y profundo de las interacciones y percepciones del usuario.

La evaluación integral tiene como objetivo asegurar que todos los componentes de la interfaz y la experiencia general respondan a altos estándares de calidad, permitiendo identificar no solo las fortalezas en el diseño y la implementación, sino también las áreas que requieren ajustes o mejoras. Este enfoque garantiza una revisión exhaustiva de cada elemento de la aplicación, facilitando el reconocimiento de oportunidades que mejoren la funcionalidad, accesibilidad y satisfacción general del usuario. A través de este proceso continuo de optimización, se busca refinar el producto hasta lograr una plataforma que ofrezca una experiencia de usuario completa, confiable y alineada con los más altos estándares de calidad y eficacia.

## 5.4. Video About-the-Product

En esta sección, se expone y describe en detalle el contenido del video titulado "About-the-Product," diseñado para informar tanto a los visitantes de la Landing Page como a los usuarios de la aplicación móvil. Este recurso audiovisual tiene como propósito brindar una presentación clara y exhaustiva sobre el modelo de negocio y las características distintivas de la aplicación de Roademics, asegurando que tanto los nuevos usuarios como aquellos registrados comprendan el valor que la plataforma ofrece.

Con el fin de alcanzar una comunicación efectiva y alineada con la identidad del producto, se ha adoptado un tono narrativo coherente y uniforme, que refleja tanto la seriedad como la innovación de la solución tecnológica. Este enfoque proyecta una imagen profesional y confiable, facilitando una experiencia de usuario que fomenta el interés y el compromiso con las herramientas y beneficios que el producto proporciona en ámbitos tanto profesionales como personales.

El video "About-the-Product" se ha integrado en la Landing Page y puede visualizarse fácilmente en esta página. Además, para fines de documentación, el video también se incluye en este informe, accesible en el siguiente enlace: (Enlace)
