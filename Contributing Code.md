Contributing Code
===========================================

Open source software is driven by community contribution, and one of the most effective ways to participate is by contributing code to either the [MongoDB Server Repo](https://github.com/mongodb/mongo) or one of the [many related projects](http://docs.mongodb.org/ecosystem/drivers/).

###Guidelines for Contributing:

####Pre-Pull Request: Searching for Issues

Before you submit a pull request to the MongoDB Server or any MongoDB open source tool, please review the [open tickets in Jira](https://jira.mongodb.org/browse/). For Server Contributions we suggest reviewing the [Server Roadmap](https://jira.mongodb.org/browse/SERVER#selectedTab=com.atlassian.jira.plugin.system.project%3Aroadmap-panel) on Jira prior to submitting a pull request and find issues that are scheduled but not assigned. These will improve the chances of your patch going into a future release. 

For upcoming releases, issues are ordered by "fixVersion":

- “2.#.#” are things we want and have scheduled.
- "2.#.w" are things we want but don't think we have time for.
- "2.#.x" are things the Kernel team wants but *really* does not have time for.

Avoid tickets with fixVersion "Needs Triage". This is the default fixVersion for new tickets, and it indicates that no decision has been made on the ticket request for the roadmap.

#####Pull Requests to the MongoDB Server

Submitting a Pull Request 

Before you submit a pull request to the MongoDB Server, please complete the following. 

Identify an existing SERVER ticket, or create a new ticket for your pull request in the Server project. It’s helpful to include the name of the Server ticket in the title of the pull request.
Sign the [MongoDB Contributor Agreement](http://www.mongodb.com/legal/contributor-agreement)

#####The Life-cycle of a Pull Request 

When you submit a pull request, here is what happens!

The engineering team will review your pull request to make sure you have included a SERVER ticket in your request and signed the contributor agreement.
You should receive a response from one of our engineers with additional questions about your contributions.
If your pull request matches a ticket and is aligned with the Server Roadmap, it will get triaged and reviewed by the Kernel team. 


####Best Practices

* Never introduce breaking backward changes.
* Write inline documentation (comments) so project maintainers and others can understand your code.
* Write tests and make sure they pass.
* Make sure your code does not break any of the existing tests.
* Review the appropriate project license. To contribute to the MongoDB Server, you must sign the [contributor agreement](http://www.mongodb.com/legal/contributor-agreement).
* Add yourself to the contributors list. Most projects have a [list of contributors](https://github.com/mongodb/mongo-hadoop#contributors)
on their Github READMe. Once your patch as been accepted, add yourself to the list. 
* Read the contributing guidelines for each project. These can be found in each individual driver repo and may differ across project. Also see the [full list of drivers projects](http://docs.mongodb.org/ecosystem/drivers/).
* Show off your accomplishment by [requesting a contributor t-shirt](http://www.mongodb.com/swag) once your first patch has landed.

If you need help or advice, the [MongoDB-user](https://groups.google.com/forum/#!forum/mongodb-user) and [MongoDB-Dev](https://groups.google.com/forum/#!forum/mongodb-dev) mailing lists are extremely active, and both are good places to either ask questions or learn from others' experiences. MongoDB-user is for users building applications with MongoDB, whereas MongoDB-Dev is best used by those contributing to the database or building third party tools. Also be sure to check out the #mongodb IRC channel on Freenode, or tag your question with mongodb (http://stackoverflow.com/questions/tagged/mongodb) on Stack Overflow. If you can answer another users' question on any of those sites - feel free to jump in! 

Always remember: MongoDB is developed in the open. The source code can often be the best way to understand how it works.
