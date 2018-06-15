# Backend Project

The following project is to build a simple service that leverages some of the technologies that we use as part of our reference architecture.

If any special requirements have been conveyed to you from your interview team, they supercede the following:

## Requirements

- [ ] Create a webservice using Java, Ruby, or Node.js that has a single endpoint.
- [ ] The endpoint should receive a URL as a parameter and return a shortened URL. For example, if the endpoint is given the following URL: "https://facebook.com", it should return "https://hostname/Ux26Yp".
- [ ] When someone accesses the shortened URL ("https://hostname/Ux26Yp"), the server should redirect to the real URL ("https://facebook.com").
- [ ] Add another endpoint to your service that allows for the bulk (hundreds) submission of URLs.
- [ ] Your submission should contain a README file that spells out the exact steps necessary to build and run the project. It should also provide instructions for how to query the webservice.

Design of the API endpoint including paths, structure, and format is up to you. Decisions on how to structure the code and what frameworks to use are up to you as well.

## Bonus

- [ ] Build a frontend for the service in any frontend framework that allows users to submit a URL to shorten it in a form, and see the result.
- [ ] Extend your frontend to allow a text file full of URLs to be submitted to the bulk API. Results can be rendered directly on the page or downloaded as a text file.
- [ ] Add a view to list all the URLs and their short versions.
