# 3	Componentes

Los componentes de Decidim son los mecanismos básicos de participación que se activan y configuran para los diferentes espacios de participación o subespacios (fases de un proceso, grupos de trabajo de un órgano, etc.).

## 3.1	Propuestas

Las propuestas son el componente más importante de Decidim. Se entiende por propuesta cualquier elemento de un plan estratégico, una normativa, un plan de inversión, un cambio legislativo o cualquier otra unidad mínima de decisión. Las propuestas pueden tener los siguientes **tipos de creadores**: por la propia organización que gestiona la plataforma  (p.e. un ayuntamiento), por participantes registradas/os, puede originarse en un encuentro como resultado de un debate o deliberación colectiva, o puede generarlos una asamblea u órgano, o una organización registrada en la plataforma. También pueden **crearse de manera directa o colaborativa** y estar sujetas a sistemas de **enmiendas**.

Las propuestas están definidas por un/a autor/a, título y un contenido de texto. Puede también incluir **imágenes**, **geolocalización** y **archivos adjuntos**. 

Una vez publicada una propuesta puede estar sujeta a **moderación** (si alguien la etiqueta como tal y define el motivo de moderación).  

En el panel de **administración** las propuestas pueden **ordenarse** con diferentes criterios, comentarse internamente (sin que los comentarios sean públicos), **descargarse** en formato JSON o CSV (compatible con software de hojas de cálculo), **recategorizarse**, o **moverse** a diferentes espacios [estas dos últimas funcionalidades están prevista para 2017Q4,  AjB-Lote3Mod1]. Además las propuestas se pueden **aceptar**, **rechazar** o mantener en estado de evaluación.

Otras funcionalidades asociadas a las propuestas son:

* **Control de versiones**:** **permite mantener un registro de todos los cambios realizados en una propuesta, así como la generación de códigos de verificación de integridad de la propuesta** **[2017Q3, GenCat].

* **Detección de similares**: Permite a quien realice una nueva propuesta encontrar otras similares realizadas anteriormente en la plataforma y así evitar duplicados [2017Q4, AjB-Lote3Mod1].

* **Relaciones entre propuestas**: las propuestas pueden relacionarse vía enlaces en la sección de comentarios, mostrándose las propuestas relacionadas como tarjetas y notificando sobre la existencia de una nueva relación. [2017Q4,  AjB-Lote3Mod1].

* **Adhesión a propuestas**: las organizaciones pueden adherirse a las propuestas y esta adhesión pública se mostrará en la propuesta y notificará a participantes que sigan la actividad de la organización [2017Q4,  AjB-Lote3Mod1].

* **Modificación y retirada de propuestas**: el/la autor/a de una propuesta puede modificarla y/o retirarla antes de que se abra la fase de recogida de apoyos [2017Q4,  AjB-Lote3Mod1].

* **Enmiendas**: cualquier participante puede editar el texto de una propuesta y se creará una propuesta "hija" a modo de enmienda (tipo Pull Request en Github), esta propuesta hija podrá recoger apoyos, el/la autor/a de la propuesta madre podrá aceptar o rechazar la enmienda (o propuesta hija). En caso de rechazo el/la autor/a de la propuesta hija podrá elevarla a propuesta oficial [2017Q4,  AjB-Lote3Mod1].

* **Creación guiada de propuestas**: Durante la creación de una propuesta se acompaña a la persona participante a través del proceso dividido en pasos, con ayudas contextuales y previsualización antes de enviar la propuesta [2017Q4,  AjB-Lote3Mod1].

* **Incubadora de propuestas**: Decidim permite la co-creación y creación colaborativa de propuestas [funcionalidad prevista para 2018Q1, AjB-Lote3Mod3]. Incorpora las siguientes funcionalidades:

    * Creación de borradores con múltiples autoras/es.

    * Lista de borradores colaborativos

    * Comentarios a borradores

    * Solicitar ayuda de otros colaboradores y aceptar colaboradoras/es

    * Vincular el borrador a una cita presencial 

    * Promoción del borrador a iniciativa, propuesta de proceso o proyecto.

## 3.2	Textos participativos

Entendemos por texto participativo una colección ordenada de propuestas que componen un documento de texto completo. La participación en el texto se deriva de la interacción con las propuestas que la componen. Este componente permite fundamentalmente tres operaciones  [funcionalidad prevista para 2018Q2, AjB-Lote3Mod4]:

* **Descomposición de un documento de texto en propuestas ordenadas** a partir de un documento en formatos ODT, XDOC, MarkDown o HTML. Si el texto está estructurado en secciones y subsecciones se crearán propuestas ordenadas a partir de la subsección de nivel más bajo, si el texto no está estructurado se creará una propuesta por cada párrafo de texto. La interfaz permite re-editar las propuestas, fusionarlas, separarlas, añadir títulos, etc.

* **Composición de propuestas en un texto unificado**: a partir de una conjunto de propuestas, éstas se podrán ordenar y generar un texto unificado y descargable.

* **Visualización e interacción** con documentos compuestos de propuestas: Se mostrará la colección de propuestas como un texto unificado y se podrán realizar enmiendas o comentarios al margen.

## 3.3	Resultados

Los resultados son propuestas (o modificaciones de propuestas) que han terminado siendo el resultado de la toma de decisión en el Decidim, ya sea de manera directa (mediante el resultado de la aplicación de un sistema de voto) o mediada por encuentros, asambleas o el equipo técnico o político a cargo de un ámbito de decisión a través de la administración de la plataforma.

El componente de resultados permite gestionar la **respuesta** **oficial **a todas las propuestas realizadas: con el motivo del rechazo o aceptación y en qué resultado ha sido aceptada la propuesta. 

Los resultados recogen los** metadatos de la trazabilidad** de las propuestas incorporadas en el resultado, así como los encuentros en los que se debatió o creó (asistentes a dichos encuentros) y la suma de apoyos recibidos.

## 3.4	Seguimiento de Resultados

El componente de seguimiento de resultados permite realizar la** conversión de resultados a proyectos** o permite descomponerlos en proyectos o subproyectos. Cada uno de dichos proyectos puede describirse en más detalle y permite **definir el estado de ejecución**, en tramos que van desde 0% de ejecución al 100%. El componente de seguimiento permite además a las personas que visitan la plataforma la **visualización del nivel de ejecución** (global,por categorías y/o subcategorías), de los resultados y de los proyectos. Los resultados, proyectos y estados se puede actualizar mediante un CVS y manualmente mediante la interfaz de administración [funcionalidad disponible para decidim.barcelona y pendiente de integración en decidim-core, previsto para 2017Q3, AjB].

## 3.5	Votaciones y/o apoyos

Las personas participantes pueden dar apoyos a propuestas. Dichos apoyos pueden interpretarse como votos, firmas, apoyos, o de cualquier otra manera que demuestre un acuerdo positivo de conformidad con la voluntad política propia. 

Existen **diferentes sistemas de voto y de gestión** del mismo en Decidim. El más sencillo permite activar los apoyos y que las participantes puedan emitir un apoyo único a cada propuesta que quieran, sin límite de propuestas votables. También es posible limitar el número de votos (p.e. 10 por cada participante).

Otra opción es el sistema de voto ponderado por prioridades. Cada participante tiene un número de apoyos disponible con diferentes pesos, por ejemplo 3 apoyos que valen 3, 2 y 1 respectivamente, con la posibilidad de distribuirlos como crea conveniente [funcionalidad prevista para 2017Q4, GenCat].

Desde el panel de administración es posible **configurar la vista de los resultados** de la votación o bien durante el periodo de voto o sólo cuando éste finalice.

Existe una forma de **voto especial para presupuestos participativos** que permite a participantes votar "gastando" una cantidad equivalente al presupuesto objeto de participación entre los proyectos propuestos. El número de votos está aquí limitado por la cantidad de gasto acumulado de los proyectos seleccionados.

## 3.6	Comentarios

Los comentarios son un componente especial que generalmente aparece asociado a otro componente (propuestas, debates, resultados, encuentros, etc.) para permitir un proceso deliberativo sobre un tema o propuesta.

El sistema de comentarios de Decidim ha sido diseñado para favorecer la deliberación. Los comentarios de primer nivel, respecto al objeto de debate, se pueden clasificar como: **a favor, en contra o neutral**. Los comentarios se pueden **anidar** en hilos de subcomentarios y se pueden **votar**. Decidim permite **ordenar comentarios** por aquellos a favor o en contra, en orden cronológico y por cantidad de votos a favor. También permite **visualización en dos columnas** con los comentarios más votados a favor y los más votados en contra [esta última funcionalidad está prevista para 2017Q4, GenCat].

## 3.7	Páginas informativas

Se trata de una página con contenido html y un título que aparece en el menú interior de los espacios de participación. Permite incorporar imágenes, vídeos empotrados y texto enriquecido.

## 3.8	Debates

Permite abrir debates sobre preguntas o temas específicos definidos por los administradores o por los participantes. [Esta funcionalidad está activa solamente para decidim.barcelona, se espera la funcionalidad integrada en Decidim-core para 2017Q3, GenCat].

## 3.9	Encuestas

El componente de encuestas permite diseñar, realizar y visualizar los resultados de encuestas que pueden activarse en diferentes espacios de participación.

* **Configurador de encuestas**: permite a administradoras/es crear preguntas y respuestas (abiertas, tipos test, selección múltiple, etc.) y activar la encuesta, así como descargar las respuestas en formato csv.

* **Interfaz de encuestas para participantes**: permite a las participantes responder a las preguntas de la encuesta.

* **Visualizador de resultados**: permite visualizar los resultados de las encuestas de manera gráfica. [funcionalidad prevista para 2017Q3, GenCat].

## 3.10	Encuentros presenciales

Este componente permite convocar encuentros, **calendarizar**, **geolocalizar**, colgar las **actas** del encuentro, **debatir**, crear **propuestas asociadas** al encuentro (indicando el tipo de apoyo colectivo a la propuesta), recoger el **número** de participantes, colgar **fotos** del encuentro y **categorizar** el encuentro dentro de un espacio.

La **configuración** de un encuentro incluye los siguientes **campos básicos**: Título, descripción, dirección, ubicación, detalles de la ubicación, hora de inicio y finalización, ámbito, categoría y aforo máximo. 

También se incluye los siguientes **campos avanzados**: carácter (público, abierto, cerrado), grupo organizador, existencia de espacio de conciliación, adecuación a personas con diversidad funcional, existencia de traducción simultánea, tipo de encuentro (informativo, creativo, deliberativo, decisivo, evaluativo, rendición de cuentas, otros) [funcionalidad prevista para [2017Q4, AjB-Lote2Mod2]

Los encuentros relacionados con una instancia de un espacio (un proceso específico o un órgano) pueden mostrarse en un **mapa** y se pueden **ordenar por fechas o categorías**. También pueden mostrarse todos los encuentros en **modo calendario**, con la posibilidad de exportarlos a calendarios del móvil u otras aplicaciones [funcionalidad prevista para [2017Q4, AjB-Lote2Mod2].

Algunas funciones avanzadas del componente encuentro incluyen:

* **Sistema de inscripción y asistencia** [funcionalidad prevista para 2017Q4, AjB-Lote2Mod2]:

    * Permite administrar el **tipo de inscripción** de un encuentro (abierto y automático, cerrado y accesible sólo a cierto tipo de participantes, etc.), definir el **número de plazas **para asistentes, realizar **reservas** de plazas, la **inscripción manual**, el envío de **invitaciones** y definir tipos de **condiciones** a aceptar para acudir al meeting (p.e. cesión de derechos de imagen) y el** registro de asistencia **de participantes.

    * Permite a las personas participantes la **inscripción** para un encuentro, solicitar **servicio de conciliación**** familiar **(ludoteca, espacio de cuidados) y obtener un **código para acreditarse** al presentarse en el encuentro. 

    * Las personas inscritas que hayan acudido al encuentro tendrán** permisos especiales** para poder evaluar el encuentro o realizar comentarios y otras acciones. 

    * Participantes o administradoras/es podrán recibir **notificaciones** sobre la apertura del periodo de inscripción, el número de plazas que quedan para inscribirse, recordatorios del encuentro, publicación de actas. 

* **Gestión del orden del día**: una sección de orden del día permite definir la duración del encuentro, la creación de  items y sub-items del orden del día, el título, contenido y duración estimada. Las personas participantes pueden proponer puntos para el orden del día. [funcionalidad prevista para 2017Q4, AjB-Lote2Mod2].

* Sistema de** redacción, publicación y validación de actas** de reuniones  [funcionalidad prevista para 2017Q4, AjB-Lote2Mod2]:

    * Las actas se pueden colgar en formato video, audio y texto.

    * Las actas en modo texto van asociadas a una **pizarra de escritura colaborativa** integrada en Decidim.

    * Las actas pasan por 4 **fases de elaboración**: 1. Escritura colaborativa durante el transcurso del encuentro, 2. Elaboración de borrador oficial de las actas, 3. Fase de enmiendas al borrador, 4. Publicación y validación final de las actas.

    * Las actas se pueden **comentar** con el componente de comentarios.

    * Se pueden también añadir **documentos adjuntos** a las actas.

* **Auto-convocatoria**: las personas participantes verificadas podrán convocar reuniones a través de la plataforma de manera directa, con el apoyo de un número determinado de otras personas participantes se activará el encuentro públicamente y las participantes convocantes tendrán acceso al panel de administración [funcionalidad prevista para 2017Q4, AjB-Lote2Mod2]

* **Visualización y exportación de encuentros**: los encuentros se pueden visualizar en modo mapa (por espacios o de manera general en la plataforma), en modo calendario, y se podrán exportar a gestores de agendas y calendarios (en formato iCalendar) [funcionalidad prevista para 2017Q4, AjB-Lote2Mod2].

## 3.11	Jornadas

Entendemos jornadas como un conjunto de encuentros que tienen algunas características específicas (programa interactivo y descargable, sistema de inscripciones, sistema de generación de certificados de asistencia y/o diplomas).

Decidim dispone de un configurador y generador de páginas de jornadas, que permite crear una **web interna para la realización de eventos** relacionados con un proceso participativo u otro espacio de participación. [El componente Jornadas está previsto para 2018Q2, AjB-Lote2Mod5]

Las opciones de configuración incluyen:

* Generación de un **programa interactivo** de las jornadas (en el caso de contar con ponentes invitados, se incluye su nombre, cargo, organización, pequeña bio, enlaces a otras webs).

* Envío de **invitaciones** por correo electrónico.

* **Ge****neración de diplomas** de manera automatizada para las personas que lo soliciten, a través de un panel de asistencia que un administrador pueda verificar.

* Enlaces a plataformas de **vídeo y materiales** de las jornadas en el programa y la documentación.

* Enlaces automáticos a webs de medios digitales que den cobertura a les jornadas.

* Seguimiento de las jornadas por **redes sociales** (p.e. incorporando un feed de Twitter).

## 3.12	Blog

El blog es un componente que permite crear y visualizar **noticias** en orden cronológico. Las entradas de un blog son otro tipo de contenido, deben estar asociadas a una instancia de un espacio de participación. Las entradas del blog están relacionadas con el sistema de clasificación de contenidos de la plataforma. Los **comentarios asociados** a las entradas del blog serán tratados como el resto de comentarios de la plataforma, ya descritos anteriormente  [funcionalidad prevista para 2017Q4, AjB-Lote2Mod1].

## 3.13	Newsletter general y selectivo

Decidim permite enviar un **newsletter** (un correo electrónico) a todas las personas inscritas en la plataforma que hayan aceptado, en las condiciones de uso, recibir dicho correo electrónico a modo de boletín informativo. El envío es personalizado con el nombre de usuaria/o y en varios idiomas (se envía por defecto en el idioma escogido por la/el usuaria/o). 

También pueden enviarse **newsletters ****selectivos** a grupos de usuarios que hayan decidido seguir un proceso, órgano o iniciativa [funcionalidad prevista para 2017Q3, GenCat].

Las personas participantes podrán **darse de baja** automática y directamente desde el propio correo electrónico haciendo click en un enlace y se podrá hacer un **seguimiento de visitas** derivadas de los newsletter [funcionalidad prevista para 2017Q4, AjB-Lote2Mod1]. 

## 3.14	Buscador

El **buscador** permite realizar búsquedas entre todos los contenidos indexables de la plataforma, tanto a nivel general como a nivel específico, realizando la búsqueda dentro de un proceso participativo concreto, o dentro de sus componentes (propuestas, resultados, etc.) mediante la búsqueda avanzada.

La **página navegable y filtrable de resultados de la búsqueda** muestra los contenidos según su tipología y ordenados según la prioridad que se haya definido (p.e. que se muestren primero los términos encontrados dentro de asambleas, y a continuación se muestren los procesos participativos.) [funcionalidad prevista para 2017Q4, AjB-Lote3Mod2]

