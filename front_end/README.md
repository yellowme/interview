# Front-end Project

Most web applications show a list of items on their main view. Usually you can click these items to see more details. Maybe you've heard of this pattern, it's called Master-Detail. Building a Master-Detail application requires handling UI events and loading the necessary data to show it on the details panel.

We are Pokemon fans! So the master view must show a list of pokemons taken from the [Pokeapi](https://pokeapi.co/) 👾

Your goal is to create a web application that lists the first 150 pokemons and show you some details about a pokemon when you click on its name.

If any special requirements have been conveyed to you from your interview team, they supercede the following.

## Requirements

- [ ] The application should be built with JavaScript. You may use frameworks or pre-compile your code if you want.
- [ ] The application should work properly on a desktop computer running Google Chrome.
- [ ] The application should be identical to the design described in the "design/desktop" folder.
- [ ] The application code should be optimized for production.
- [ ] The site should be a [SPA](https://en.wikipedia.org/wiki/Single-page_application). The site should not reload to show a pokemon's details.
- [ ] The project must have a README listing the supported browsers and the technologies and patterns used in development.

## User Stories

- [ ] The user should be able to see and click all first 150 pokemons in the left sidebar.
- [ ] The user should be able to see the pokemon's details when clicking its name.

## Bonus points

- [ ] This is your Pokedex. Add more details to the white spaces in the detail view.
- [ ] Use an architecure to divide and encapsulate components of a feature.
- [ ] Make the site responive 🙌 (You can take some ideas form the "design/mobile" folder).
- [ ] Support other major browsers 🦄 (Firefox, Safari, Opera, Edge).
- [ ] Add a router to your application. Update the site's URL when a pokemon detail panel is shown (without reloading the site). Users should be able to enter this URL and see the pokemon's details without having to click its name.
- [ ] Create a set of Unit Tests for the project.
- [ ] Create a set of E2E (UI) Tests for the project.

## Hints

- [Pokemon API Docs](https://pokeapi.co/docsv2/#).
- The Pokeapi has a limit usage per hour. Consider mocking the requests.
- Review the `offset` and `limit` parameters for the GET request.
 
