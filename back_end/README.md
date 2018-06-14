# Backend Project

The following project is build a simple service that leverages some of the 
technologies that we use as part of our reference architecture.

If any special requirements have been conveyed to you from your interview
team, they supercede the following.

## Requirements

- [ ] Create a webservice using Java, Ruby, or Node.js that has a single 
      endpoint.
- [ ] The endpoint should receive as a parameter a url and return that 
      url shorter. For example, if the endpoint is given the url 
      "https://facebook.com" it should return "https://hostname/Ux26Yp".
- [ ] When someone access to the url "https://hostname/Ux26Yp" the server should redirect to the real url that is "https://facebook.com".
- [ ] Add another endpoint to your service that allows for the bulk (hundreds) 
      submission of urls.
- [ ] Your submission should contain a README file that spells out the exact 
      steps necessary to build and run the project. It should also provide 
      instructions for how to query the webservice.

Design of the API endpoint including paths, structure, and format is up to 
you. Decisions on how to structure the code and what frameworks to use are 
up to you as well.

## Bonus

- [ ] Build a frontend for the service in front-end framework that allows users to submit an
      url to short it in a form and see the result.
- [ ] Extend your front end to allow a text file full of urls to be 
      submitted to the bulk API. Results can be rendered directly on the page
      or downloaded as a text file.
