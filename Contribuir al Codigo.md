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



* Review the appropriate project license. To contribute to the MongoDB Server, you must sign the [contributor agreement](http://www.mongodb.com/legal/contributor-agreement).
* Add yourself to the contributors list. Most projects have a [list of contributors](https://github.com/mongodb/mongo-hadoop#contributors)
on their Github READMe. Once your patch as been accepted, add yourself to the list. 
* Read the contributing guidelines for each project. These can be found in each individual driver repo and may differ across project. Also see the [full list of drivers projects](http://docs.mongodb.org/ecosystem/drivers/).
* Show off your accomplishment by [requesting a contributor T-shirt](http://www.mongodb.com/swag) once your first patch has landed.

If you need help or advice, the [MongoDB-user](https://groups.google.com/forum/#!forum/mongodb-user) and [MongoDB-dev](https://groups.google.com/forum/#!forum/mongodb-dev) mailing lists are extremely active, and both are good places to either ask questions or learn from others' experiences. MongoDB-user is for users building applications with MongoDB, whereas MongoDB-dev is best used by those contributing to the database or building third party tools. Also be sure to check out the #mongodb IRC channel on Freenode, or tag your question with mongodb on [Stack Overflow](http://stackoverflow.com/questions/tagged/mongodb). If you can answer another users' question on any of those sites - feel free to jump in! 

Always remember: MongoDB is developed in the open. The source code can often be the best way to understand how it works.
