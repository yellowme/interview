# Backend Project

The following project is to build a simple service leveraging API best practices.

If any special requirements have been conveyed to you from your interview team, they supersede the following:

## Requirements

- [ ] You can select the language you think is the best for this challenge. If you decide to use a functional programming like elixir just let us know first.
- [ ] You are free to add any library for improving the development experience, like, linters, formatters, etc. Try to emulate the environment that you would like to have when you are working.
- [ ] You should design your APi for evolvability. Given that in real life no API stays static for long.  
- [ ] You can use any API paradigm. Rest, RPC or GraphQL depending on what you think is best for the challenge. 
- [ ] The app should have the tests that you decide are necessary for maintainability
- [ ] You should handle all success and errors cases the endpoints could have. When there is an error the backend should notify the client about it in such a way that allows the client side to decide what to do. (Ex. If the client tries to create an article without a title we expect the API to notify the user that the title is a required attribute in order to create an article) 
- [ ] There should be a way for client users to discover how to use the API. It can be a document, a postman, a swagger document or a plain html website. Is up to you but it should allow the user to discover all your endpoints, and their possible responses both success and errors. 

## API Specification

We want to create an API that allow us to handle articles that could be shown in many clients like mobile apps, websites and text to speech apps, etc.
 
 For this challenge assume that the writers are already store in the application database. You don't need to create a registration endpoint
 

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
- created_at
- state

### Writer

Writer attributes: 

- first name
- last name

## User Stories 

- [ ] As a writer I should be able to create an article
- [ ] As a writer I should be able to change an article status from drafted to published or viceversa.
- [ ] As a writer I should be able to edit any of my articles
- [ ] As a writer I should be able to list all my articles (published and drafted state)
- [ ] As a writer I should be able to see a list of only my drafted articles or only my published articles
- [ ] As a writer I should be able to see one article
- [ ] As a writer I should be able to do everything a visitor can do in the API
- [ ] As a visitor I should be able to list all the published articles order by published date in descending order
- [ ] As a visitor I should be able to see a published article 

## Bonus Points 

Take 1 or 2, we don't expect for you to do everyone of them. 

- [ ] Update the list of user stories, and the API documentation if we add a new actor called Admin that is the only one with the permission to publish articles but only when an article is "ready to review". Think about how that new actor will change your current implementation and what changes you will need to do.
 - [ ] Deploy the API in a Platform as a Service (Heroku, Blue Ocean, AWS, GCloud, etc)
- [ ] Dockerize the development environment so the database, programming language version, etc lives in a container. The idea is that when a new developer starts on the project she will not have to configure the development environment by hand. 
- [ ] Write down every tool or methodology that you know for improving backend developer happiness explaining why you think they are necessary. 
- [ ] Create a deployment pipeline that runs linters, tests, ect every time any branch is push it to the repository. In addition, when a PR is merged to master(main) branch then the app should be deployed.
- [ ] Write down the name of the strategies or, a little paragraph explaining how you would prevent all or some of these security vulnerabilities. 
   - Distributed Denial-of Service attacks
   - Cross Site Request Forgery attacks
   - Man in the middle attacks
   - SQL Injection attacks
   - Lack of Resources & Rate Limiting
   or other possible security considerations. write strategies we could use to prevent it.
  
