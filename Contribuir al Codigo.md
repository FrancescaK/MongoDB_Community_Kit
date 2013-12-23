Contribuir al código
===========================================

El software open source es impulsado por la contribución de la comunidad y una de las formas más efectivas de participar es contribuyendo al código, bien del [MongoDB Server Repo](https://github.com/mongodb/mongo) o uno de los [Muchos proyectos relacionados](http://docs.mongodb.org/ecosystem/drivers/) como drivers o librerías.

###Directrices de contribución:

####Pre-Pull Request: Buscando Issues

Antes de enviar un pull request al MongoDB Server o cualquier herramienta open source de MongoDB, por favor revida los [tickets abiertos en Jira](https://jira.mongodb.org/browse/). 

Para contribuciones al Server, sugerimnos revisar la [Hoja de ruta del Server](https://jira.mongodb.org/browse/SERVER#selectedTab=com.atlassian.jira.plugin.system.project%3Aroadmap-panel) en Jira para encontrar issues que se hayan programado pero no asignado. Esto aumentará las oportunidades de que tu parche vaya a la siguiente release.

Para próximas releases, los issues están ordenados por "fixVersion":

- “2.#.#” son cosas que queremos y hemos programado.
- "2.#.w" son cosas para las que creemos que no tenemos tiempo.
- "2.#.x" son cosas que el equipo de Kernel quiere pero para las que  *realmente* no tienen tiempo.

Evita los tickets con la fixVersion "Needs Triage". Es la fixVersion por defecto para los nuevos tickets e indica que nos se ha tomado una decisión en relacion de esa solicitud para la hoja de ruta.

#####Pull Reuqests al MongoDB Server

Antes de enviar un pull request al MongoDB Server, por favor completa los pasos siguientes:

* Lee las [directrices de contribución](http://www.mongodb.org/about/contributors/). En particular, deberías asegurarte de que tus cambios se adhieren a las reglas de Reglas de Desarrollo del Kernel de MongoDB incluyendo estilo de código, manejo de excepciones, loggin y tests.
* Identifica un [Server ticket](https://jira.mongodb.org/browse/SERVER), o crea un nuevo ticket para tu pull request en el proyecto del Server.
Por favor, incluye una referencia al [SERVER ticket](https://jira.mongodb.org/browse/SERVER) en el título del pull request (eg: "SERVER-1234: Add $foo operator to Aggregation framework").
* Asegurate de que tu solicitud de código es específica para los cámbios de un solo issue en Jira. Si has hecho múltiples commits, sería preferible [unificarlos](http://git-scm.com/book/en/Git-Tools-Rewriting-History#Squashing-Commits) en un solo commit antes de enviar la solicitud. Si tu cámbio soluciona varios issues de Jira, divídelos entre múltiples pull requests o incluye algún detalle sobre por qué no ha sido possible.
* Firma el [Acuerdo de contribución de MongoDB](http://www.mongodb.com/legal/contributor-agreement).


#####Ciclo de vida de un Pull Request

Esto es lo que sucede cuando envías un pull request:

* El equipo de ingeniería revisará la solicitud para asegurarse de que has incluido el SERVER ticket en tu solicitud y firmado el acuerdo de contribución.
* Deberías recibir una respuesta de uno de nuestros ingenieros con preguntas adicionales sobre tus contribuciones.
* Si tu solicitud concuerda con un ticket y está alineado con la Hoja de Ruta del Server, le será asignada una prioridad y será revisada por el equipo del Kernel.
* Las Pull Request que han sido revisadas y aprobadas serán firmadas y fusionadas en una rama de desarrollo y la issue de Jira será resuelta en la fixVersion esperada.

####Buenas prácticas

* Nunca introduzcas cambios que rompan cambios anteriores
* Escribe documentación inline (comentarios) para que los mantenedores del proyecto y otros puedna entender tu código.
* Escribe tests y asegurate de que pasan.
* Asegúrate de que tu código no rompe ninguno de los tests exisentes.
* Revisa la licencia del proyecto. Para contribuir al MongoDB Server, debes firmar el [acuerdo de contribución](http://www.mongodb.com/legal/contributor-agreement).
* Añadete a la lista de contribuidores. La mayoría de los proyectos tiene una [lista de contribuidores](https://github.com/mongodb/mongo-hadoop#contributors) en su README de Github. Una vez que tu parche haya sido aceptado, añadete a la lista.
* Lee las guias de contribución para cada proyecto. Estas se pueden econtrar en el repositorio de cada driver y pueden ser diferentes entre proyectos. Lee también la [lista completa de proyectos de drivers](http://docs.mongodb.org/ecosystem/drivers/).
* Muestra tu logro [solictando una camiseta de contribuidor](http://www.mongodb.com/swag) una vez que tu primer parche haya sido acabado.  

Si necesitas ayuda o consejo, las listas de correo de [MongoDB-user](https://groups.google.com/forum/#!forum/mongodb-user) y [MongoDB-dev](https://groups.google.com/forum/#!forum/mongodb-dev) son extremadamente activas y ambas son un buen lugar para preguntar o aprender de las experiencias de los demás.   MongoDB-user es para usuarios creando aplicaciones con MongoDB, mientras que MongoDB-dev es más utilizada por los que contribuyen a la base de datos o crean herramientas de terceros. Asegúrate también de comprobar el canal de IRC #mongodb en Freenode, o etiqueta tu pregunta con mongodb en [Stack Overflow](http://stackoverflow.com/questions/tagged/mongodb). Si puedes responder preguntas de otros usuarios en alguno de estos sitios, sientete libre de participar.

Recuerda siempre: MonogoDB se desarrolla en apertura. El código fuente puede amenudo ser la mejor manera de entender cómo funciona.
