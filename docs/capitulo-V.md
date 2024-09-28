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

A continuación, se proporciona una lista con los enlaces a la organización de GitHub de WHAI y a los repositorios específicos relacionados con el desarrollo del frontend dentro de esta organización:

**Repositorios en GitHub:**

- Organización: https://github.com/GRUPO-3-MOVILES 

- Reporte: https://github.com/GRUPO-3-MOVILES/upc-pre-202402-cc-238-WV61-WeHaveAnIdea-report 

- Aplicación Móvil: https://github.com/GRUPO-3-MOVILES/upc-pre-202402-cc-238-WV61-WeHaveAnIdea-MobileApplication

- Landing Page: https://github.com/GRUPO-3-MOVILES/upc-pre-202402-cc-238-WV61-WeHaveAnIdea-landingPage 

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
- Guía de Pautas de Javascript de MDN (Mozilla): https://developer.mozilla.org/en-US/docs/MDN/Writing_guidelines/Writing_style_guide/Code_style_guide/JavaScript}
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


### 4.1.4. Software Deployment Configuration.

En esta sección, se detallará la configuración necesaria para implementar la solución, enfocándose exclusivamente en el despliegue del Backend del proyecto. El backend se desarrollará utilizando Java junto con el framework SpringBoot, lo que proporcionará una arquitectura robusta, escalable y fácil de mantener. Comenzaremos por crear un repositorio en GitHub destinado a almacenar todo el código relacionado con la lógica del servidor, controladores, servicios, y los modelos de datos que interactuarán con la base de datos MongoDB. 

Este repositorio permitirá a los desarrolladores gestionar de manera eficiente la colaboración y el control de versiones, asegurando que cada miembro del equipo trabaje en su propia rama "feature" para desarrollar nuevas funcionalidades del backend, tales como la autenticación de usuarios, el manejo de solicitudes, o la gestión de sesiones. Posteriormente, se llevará a cabo el proceso de merge con la rama principal "develop", lo que asegura que la lógica del backend esté siempre actualizada y optimizada con las últimas mejoras y correcciones.

## 4.2. Software Development & Implementation.

A continuación, describimos en detalle el enfoque técnico que adoptaremos para la implementación, pruebas y despliegue de nuestra infraestructura backend, centrado en la creación y gestión de los servicios web, así como en la integración con la base de datos y el manejo eficiente de las API necesarias para el correcto funcionamiento de la aplicación. Este proceso abarca el desarrollo de servicios backend escalables, la validación exhaustiva mediante pruebas unitarias y de integración, y la optimización del rendimiento antes de cada ciclo de despliegue en el entorno de producción. 

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
