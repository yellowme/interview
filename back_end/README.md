# Backend Project

The following project is to build a simple service leveraging API best practices. This should take you about 5 hours to complete, but you are free to spend more time on it.

If any special requirements have been conveyed to you from your interview team, they supersede the following:

## API Specification

We want to create an API that allow us to handle articles that could be shown in many clients like mobile apps, websites, text to speech apps, etc.
 
 For this challenge assume that the writers are already store in the application database. You don't need to create a registration endpoint.
 
## Actors 

### Visitor
Is any person that wants to read the articles published in the API. It doesn't have to authenticate herself to do it. 

### Writer

Is a person that have the permission to create new articles in our API. It has to authenticate herself in order to create, edit and publish articles.

## Entities

This is a list of entities that need to be on the API.  

### Article

An article can be on two possible states. The first one is **drafted** that means that only the writer can see it. The second one is "published" that means that everyone can see it. 

Article attributes: 

- title
- body
- published date
- state (drafted or published)

### Writer

Writer attributes: 

- email 
- password

## User Stories 

1. As a writer I should be able to create an article
2. As a writer I should be able to change an article status from drafted to published or viceversa.
3. As a writer I should be able to edit any article
4. As a writer I should be able to list all articles (published and drafted state)
5. As a writer I should be able to see a list of all drafted articles or all published articles
6. As a writer I should be able to see one article
7. As a writer I should be able to do everything a visitor can do in the API
8. As a visitor I should be able to list all the published articles order by published date in descending order
9. As a visitor I should be able to see a published article 

## Requirements

- [ ] You can select the language you think is the best for this challenge. If you decide to use a functional programming like elixir just let us know first.
- [ ] You are free to decide the high level architecture of the app.
- [ ] You are free to add any library for improving the development experience, like, linters, formatters, etc. Try to emulate the environment that you would like to have when you are working.
- [ ] You should design your API for evolvability. Given that in real life no API stays static for long.
- [ ] The API clients are going to be mobile devices.  
- [ ] You can use any API paradigm. Rest, RPC or GraphQL depending on what you think is best for the challenge. 
- [ ] The app should have the tests that you decide are necessary for maintainability
- [ ] You should handle all success and errors cases the endpoints could have. When there is an error the backend should notify the client about so allows the client side to decide what to do. (Ex. If the client tries to create an article without a title we expect the API to notify the user that the title is a required attribute in order to create an article).
- [ ] There should be a way for client users to discover how to use the API. It can be a document,a postman project, a swagger document or a plain html website. Is up to you, but it should allow the user to discover all your endpoints, and their possible responses both success and errors.
- [ ] Even if you don't implement it you should think of a plan about how you will deploy the application. You don't have to write anything, you can tell us during the interview.

## Bonus Points 

Take 1 or 2, we don't expect for you to do everyone of them. 

1. Make changes on your App, so it complies with these new user stories. Note that these stories have conflicts with the previous stories 2,3,4 and 5.
  1. As a writer I should be able to edit only my articles
  2. As a writer I should be able to only change my articles status from drafted to published or viceversa.
  2. As a writer I should be able to list see only my articles (published and drafted state) 
  3. As a writer I should be able to see a list of my drafted articles, or my published articles.
2. Dockerize the development environment so the database, programming language version, etc lives in a container. The idea is that when a new developer starts on the project she will not have to configure the development environment by hand. 
3. Write down every tool or methodology that you know for improving backend developer happiness explaining why you think they are necessary and how a team would use them on their workflow. 
4. Create a deployment pipeline that runs linters, tests, ect every time any branch is push it to the repository. In addition, when a PR is merged to master(main) branch then the app should be deployed on a Platform as a Service like Heroku, AWS or GCloud.
5. Write down the name of the strategies or, a little paragraph explaining how you would prevent all or some of these security vulnerabilities. 
   - Distributed Denial-of Service attacks
   - Cross Site Request Forgery attacks
   - Man in the middle attacks
   - SQL Injection attacks
   - Lack of Resources & Rate Limiting
   or other possible security considerations. write strategies we could use to prevent it.
6. Write down what you would add for logging and monitoring of the system. What kind of metrics and logs the application could have and what mechanism for notification you could use to let the team now when something happens?  
7. Write down how to handle authentication on multiple types of devices. For example, imagine that this API will be consumed in a mobile application, a web browser, and on a server. How you would handle authentication on each scenario and why?  

