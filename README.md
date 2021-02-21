# QA Showcase

The goal of this repo is to showcase manual and automated tests that I've been learning how to do as part of my QA training.

 ## Disclamer
 
Work in progress.

 ## Shopping List - Testing app
 
 In order to practice the manual testing with different scenarios and test cases, I tested a small app called [Shopping List](https://shopping-list-test-1.herokuapp.com/) that @susanaventura developed for me. The app has a bunch of bugs and problems that were meant for me to find. The app's repo is available in [here](https://github.com/susanaventura/shopping-list-public).
 
 - The specs for the app are listed in [Trello](https://trello.com/b/91IwxfVK/shopping-list).
 - The tickets that I considered valid are in the 'Done' column;
 - Bug tickets are listed under the Bugs - FE list
 - The bugs are indicated as comments in the ticket. I used the Gherkin syntax for the tests that failed in order to practice and give some examples using that syntax
 - The complete list of test cases is available in [here](https://docs.google.com/spreadsheets/d/1s93ofgGoDy4cWt9iLHyD99UgH992FZ1096nrQ5ov1w0/edit?usp=sharing).
 
There are some tests missing, the idea of this is just to showcase and not to do a complete test to the app.

__TODO__
- Postman Api tests to the REST api
- Complete the test cases
 
 ## Postman REST API
 
 This project was done by following the exercises of the Udemy course [Postman: The Complete Guide - REST API Testing](https://www.udemy.com/course/postman-the-complete-guide/). 
 
 Here I learned how to use REST requests using Postman and how to make automatic tests using JavaScript with the Chai Assertion Library. Then I made some modifications and improvements to those tests. In this showcase there is a sequence of requests and tests for the Trello API and the GitHub API. The GitHub exercise is simpler and the Trello one is a little bit more complex.
 
 ### Trello
 To use the Trello collection you just have to copy the __Trello.postman_environment.template.json__ file, remove the `template` extension and insert your [Trello Key](https://trello.com/app-key) and [Trello Token](https://trello.com/app-key) in order to run the requests.
 
 ```json
 {
	"id": "6dde355b-7bc9-47be-9532-f73685489b9f",
	"name": "Trello",
	"values": [
		{
			"key": "trelloKey",
			"value": "<YOUR TRELLO KEY>",
			"enabled": true
		},
		{
			"key": "trelloToken",
			"value": "<YOUR TRELLO TOKEN>",
			"enabled": true
		}
	],
	"_postman_variable_scope": "environment",
}
```

### GitHub
 To use the Github collection you just have to copy the __GitHub.postman_environment.template.json__ file, remove the `template` extension and insert your username in the `owner` env var. You also need to setup your OAuth-2.0 authentication.


