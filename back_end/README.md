# Backend Project

The following project is to build a simple service that leverages some of the technologies that we use as part of our reference architecture.

If any special requirements have been conveyed to you from your interview team, they supercede the following:

## Technical Requirements

- [ ] You can select the language you think is the best for this challenge. If you decide to use a functional programming like elixir just let us know first.
- [ ] You are free to add any library that improve the development experience. Like, linters, formatters, etc.Try to emulate the environment that you would like to have when you are working.
- [ ] You should design your APi for evolvability. Given that in real life no API stays static for long.  
- [ ] You can use any API paradigm. Rest, RPC or GraphQL depending on what you think is best for the challenge. 
- [ ] The app should have the tests that you decide are necessary for maintainability
- [ ] You should handle all success and errors the endpoints could have. When there is an error the backend should notify the client about it in such a way that allows the client side to decide what to do. (Ex. If the client tries to create an article without a title we expect the API to notify the user that the title is a required attribute in order to create an article) 
- [ ] There should be a way for your user to discover how to use the API. It can be a document, postman, swagger or a plain html website. Is up to you but it should allow the user to discover all your endpoints, and their possible responses (success and error) 

## API Specification

We want to create an API that allow us to handle articles that could be shown in many clients like mobile apps, websites and text to speech apps, etc.
 
 An article commonly follows this process.

-> draft -> published 

## Actors 

### Visitor
Is any person that wants to read the articles published in the API. It doesn't have to authenticate herself to do it. 

### Writer
Is a person that have the permission to create new articles in our API. It has to authenticate herself in order to create, edit and publish articles.

## User Stories 

- [ ] As a writer I should be able to create an article in draft state
- [ ] As a writer I should be able to publish a draft article
- [ ] As a writer I should be able to move an article from publish state to draft state 
- [ ] As a writer I should be able to edit any of my articles
- [ ] As a writer I should be able to list all my articles (published and in draft state)
- [ ] As a writer I should be able to see only my draft articles or only my published articles
- [ ] As a writer I should be able to see one of my draft articles
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
   

### Writer 
- [ ] A writer should be able to create an article in a draft state
- [ ] A writer should be able to publish a draft
- [ ] A writer should be able to list all her draft articles
- [ ] A writer should be able to see her draft article
- [ ] A writer should be able to delete any of her draft articles
### Visitor
- [ ] A visitor should be able to see a list of all published articles ordered in descending order by published date
- [ ] A visitor should be able to list a published article
### Admin
- [ ] An admin should be able to publish an article
- [ ] An admin should be able to list all draft articles
- [ ] An admin should be able to see any article in the platform
- [ ] An admin should be able to delete an article


## Bonus

- [ ] Build a frontend for the service in any frontend framework that allows users to submit a URL to shorten it in a form, and see the result.
- [ ] Extend your frontend to allow a text file full of URLs to be submitted to the bulk API. Results can be rendered directly on the page or downloaded as a text file.
- [ ] Add a view to list all the URLs and their short versions.

## Things to grade

- Extensibility of the API
- How easy is for your clients to implement the API
- Error handling
- Api Design
