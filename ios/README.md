# iOS Project

A common feature for most of the mobile applications is a Login. This feature not only requires work with a form but also the logic to decide whether the application sends the user to the main view or the login form when launching the app.

We are Pokemon fans! So the main view must be a list of pokemons taken from the [Pokeapi](https://pokeapi.co/).

Your goal is to create an application that handles the logic to allow the user login and see the main view any time they launch the app.

If any special requirements have been conveyed to you from your interview team, they supercede the following:

## Requirements

- [ ] The application should be built with Swift.
- [ ] The application should be able to run on the iPhone simulator.
- [ ] The application should contain at least two view controllers.

## User Stories

- [ ] The user should authenticate with email and password (you could use static data and a fake endpoint to validate what the user types on the form).
- [ ] The user should be able to log out.
- [ ] The user should be able to view a list of pokemons (this is the main view).
- [ ] The user session should be stored locally.
- [ ] The user should be able to see the main view if they had already logged in.
- [ ] The list of pokemons should be stored locally (you don't need to store all of the pokemons returned by the API, just some of them).

## Bonus points

- [ ] Use an architecure to divide and encapsulate components of a feature (e.g. MVC, MVP, MVVM).
- [ ] Create a set of Unit Tests for the project.
- [ ] Create a set of UI Tests for the project.

## Hint

- [Pokemon API Docs](https://pokeapi.co/docsv2/#).
- The Pokeapi has a limit usage per hour. Consider mocking the requests.
- Review the `offset` and `limit` parameters for the GET request.
