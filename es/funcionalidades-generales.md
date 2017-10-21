# 5	Funcionalidades generales 

Explicamos a continuación una serie de funcionalidades y características generales de la plataforma que no quedan recogidas en los espacios o componentes ni en las funcionalidades directamente asociadas a participantes.

## 5.1	Instalación y configuración

Decidim **se instala fácilmente** a través de la línea de comandos en cualquier servidor GNU/Linux con los siguientes servicios instalados: PostgreSQL 9.4+, Ruby 2.4.1, NodeJS con yarn (JavaScript dependency manage), ImageMagick y PhantomJS. Un script automático de instalación permite desplegar todo el sistema de dependencias, librerías, bases de datos y otros servicios requeridos de manera automática en Heroku o Docker [funcionalidad prevista para 2018].

La **configuración** del portal permite una **personalización** con los siguientes campos que se rellenan en un formulario desde el panel de administración: Nombre del portal, perfiles de redes sociales (Twitter, Facebook, Instagram, Youtube, Github), breve descripción, texto de bienvenida, idioma por defecto, imagen de portada, logotipo de la organización, favicon, prefijo de referencia (identificador único que se aplicará a los elementos del portal) y URL de la organización.

## 5.2	Integración con otros servicios y compatibilidad/creación de servicios adicionales

Decidim se puede integrar fácilmente con los siguientes  servicios que puede instalarse o configurarse junto con Decidim:

* **OpenStreetMap**: para mostrar eventos y propuestas geolocalizadas

* **Piwik**: analítica de visitas a la web

* **Pad**: pizarras de escritura colaborativa en tiempo real (tecnología por determinar) [Funcionalidad prevista para 2018Q1-3 AjB-Lote1]

* **Identidad y firma digital**: integración con el sistema de gestión de identidad digital OAuth2, sistemas basados en blockchain y sistemas de gestión de identidad y firma digital institucionales reconocidos [Funcionalidad prevista para 2018Q1-3 AjB-Lote1].

* **Sistema distribuido de archivos**: Difusión o réplica de propuestas u otros elementos de la plataforma en sistema distribuidos de archivos (tipo blockchain o IPFS) [Funcionalidad prevista para 2018Q1-3, AjB-Lote1].

* **Microblogging**: integración/compatibilidad con un protocolo/servicio estandarizado y abierto de microblogging tipo GNU Social o StatusNet para la actividad de participantes (propuestas, comentarios y mensajes) [Funcionalidad prevista para 2018Q1-3, AjB-Lote1].

Decidim genera automáticamente los siguientes servicios además de los que pueden navegarse mediante la web o accederse mediante la API: 

* **SMTP**: envío de correos electrónicos.

* **Calendario**: integración o compatibilidad con sistemas de gestión de calendarios y creación y actualización automática de calendarios de eventos, etc.  [Funcionalidad prevista para 2018Q1-3, AjB-Lote1].

## 5.3	Multi-tenencia 

**Múltiples tenencias** de la plataforma pueden servirse en base a una sola instalación. Dicho de otra manera, una sola instalación de Decidim permite desplegar tantos portales como se quiera con una configuración específica para cada una de las instancias. De este modo una organización puede crear portales de participación para sub-organizaciones suyas, o varias organizaciones pueden compartir servidor y reducir los costes de mantenimiento de sus portales.

## 5.4	Multi-idioma

Decidim es una plataforma **multi-idioma**. Durante la instalación se configuran los idiomas disponibles. Los menús, formularios de administración y, en general, los textos fijos de la plataforma están disponibles en varios idiomas (Castellano, Catalán, Euskera, Italiano, Francés, Holandés y Suomi). Un sistema de **traducción colaborativa** en [https://crowdin.com/project/decidim](https://crowdin.com/project/decidim), facilita la incorporación de nuevos idiomas a la plataforma. 

A nivel de contenido, una vez fijados los idiomas oficiales de la instancia durante la instalación, todos los contenidos que se crean desde el panel de administración tienen la opción de generarse en dichos idiomas. El panel de administración permite la **gestión de contenidos en diferentes idiomas** a través de pestañas. El contenido generado por las personas usuarias se muestra en la plataforma en un sólo idioma (el escogido por la persona participante a través del selector de idiomas en la parte superior de los menús o automáticamente a través de la configuración lingüística de su navegador).

## 5.5	Estadísticas, datos abiertos y descargas

Además de la  interfaz de programación de aplicaciones (API) que proporciona acceso a datos públicos de manera  automática, en la portada de Decidim puede encontrarse un **cuadro de estadísticas generales**, con los siguientes campos: número de participantes, procesos, propuestas, resultados, encuentros, comentarios y votos.

Otro **cuadro de estadísticas de cada proceso participativo **muestra el número de encuentros, propuestas, votos y resultados de un proceso determinado.

Desde el panel de administración se pueden **exportar las propuestas, resultados y comentarios **de un proceso de participación a formato CSV y JSON y respuestas a las encuestas para su tratamiento y/o integración con otros sistemas de gestión. Las personas participantes pueden **descargar los resultados de un proceso participativo y su grado de ejecución** mediante un fichero CSV.

Decidim dispone también de un **módulo de visualización de datos**, tanto a nivel general de la plataforma como de manera específica (mostrando datos de un determinado Espacio Participativo) [funcionalidad prevista para 2018Q1, AjB-Lote2Mod4]. Entre los gráficos que se muestran están los siguientes:

* **Gráfico interactivo** de línea temporal con la evolución de los contadores de los diferentes componentes.

* **Mapa de calor** del total de encuentros, propuestas u otros contenidos geolocalizables.

* **Diagramas interactivos **(de barras, circulares o de sectores) con los resultados de un proceso (importe de cada uno de los proyectos de presupuestos participativos, filtro por categorías y estado de las propuestas - seleccionadas sí o no, etc.).

Todas estas visualizaciones vienen acompañadas de una **opción de descarga de los datos** en formato CSV [funcionalidad prevista para 2018Q1, AjB-Lote2Mod4]. 

## 5.6	API, Diseño web adaptable y aplicación móvil

Decidim dispone de un interfaz de programación de aplicaciones o API que es un conjunto de llamadas a servicios y datos de forma independiente de la interfaz web de Decidim. Esto permite a terceros desarrollar servicios sobre la plataforma, liberar datos de manera automática o desarrollar nuevas interfaces o integración de otros servicios con decidim.

La API viene acompañada de una **documentación** y una **ontología formal** de participación [funcionalidad prevista para 2018Q1-3, AjB-Lote1]

El **diseño** web de Decidim es completamente **adaptable** (*responsive*), siguiendo la filosofía de diseño *mobile-first* (primero se diseña para el móvil, luego se expande para sistemas de escritorio y tablets).

Tanto el diseño web como la API facilitan el desarrollo de aplicaciones móviles para Decidim, está previsto el desarrollo de una **App Móvil** para finales de 2018 [AjB].

## 5.7	Sistemas de clasificación de contenidos

A nivel de clasificación de contenidos Decidim permite diferenciar y configurar: ámbitos, categorías y etiquetas (o tags).

Los **ámbitos** son generales a toda la plataforma y se dividen en los de tipo **territorial** y **temático**. Los ámbitos territoriales, una vez definidos, permiten clasificar elementos de los espacios territorialmente (p.e. si un proceso, o un órgano o una iniciativa afecta a un distrito o dos, a toda la ciudad, a una región o a un país, dependiendo de la organización). Igualmente los ámbitos temáticos se definen para toda la plataforma y permiten clasificar los diferentes elementos de los espacios de participación [funcionalidad prevista para 2017Q4, Gencat].

Las **categorías y subcategorías** sirven para clasificar contenidos dentro de los diferentes espacios y se definen para cada una de las instancias de los espacios. Así por ejemplo, un proceso de participación puede incluir diversas categorías y subcategorías (las define el/la administrador/a del proceso) y los encuentros, encuestas, propuestas u otros componentes del proceso se pueden clasificar bajo estas categorías.

A diferencia de los ámbitos y las categorías, las **etiquetas** o tags son transversales, son libremente definidas por las personas participantes y se pueden aplicar a cualquier instancia o componente. Desde el panel de administración se pueden crear etiquetas, anidarlas y definirlas. Un sistema de sugerencia de etiquetas permite a las personas que participan escoger etiquetas similares a las que están proponiendo para etiquetar cualquier elemento de la plataforma. Se podrán navegar los elementos por etiquetas y mostrar las etiquetas más populares [funcionalidad prevista para 2017Q4, AjB-Lote2Mod1].

## 5.8	Sistema de ayuda contextual, tests de usabilidad  y valoración

Decidim incluye un sistema de **ayudas contextuales editables** para guiar a personas participantes y administrativas en el uso de la plataforma. Igualmente incluye  un sistema que permite realizar **experimentos de usabilidad** con tests y estadísticas de uso, así como realizar **encuestas de valoración automáticas** a las participantes de cara a identificar errores de usabilidad, de procedimientos de participación y mejorar la calidad democrática y de experiencia del software [Funcionalidad prevista para 2018Q1-3, AjB-Lote1].


