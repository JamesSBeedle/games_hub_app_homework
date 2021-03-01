1. What is responsible for defining the routes of the games resource?

       The routes are defined by gamesRouter which calls the function createRouter and alters the routes contained within to follow the paths it requires.

2. What do you notice about the folder structure? Whats the client responsible for? Whats the server responsible for?

	The Client is responsible for providing the browser with information and the user experience and user interface. (Front end)

	The server is responsible for the routing of the requests and the database. (Back end)


3. What are the responsibilities of server.js?

	The server is responsible for importing express, parser, mongoclient createrouter and cors. It then uses cars and the parser within the app. Connects to the db and creates a router called gamesRouter.

  
4. What are the responsibilities of gamesRouter?
	
    To set the routes in createRouter to use the /api/games prefix so the user can interact with the game information.  

5. What process does the client (front-end) use to communicate with the server?

	 It uses fetch requests to communicate with the server.

6. What optional second argument does the fetch method take? And what is it used for in this application? 

	It takes an init object to allow you to control different settings. In this app it is allowing us to send POST and DELETE requests rather than just sending GET requests that we would be doing without the init parameter.

7. Which of the games API routes does the front-end application consume (I.e make requests to)?

	GET, POST, DELETE

8. What are we using the MongoDB driver for?

	To perform CRUD operations to the DB.

9. Why do we need to use ObjectID from the MongoDB driver?

	So we can select a specific item in the database and only that item.
