Features 
- Authentication
- Search repo
- Retrieve from graph
- Support for all languages

Tasks to do
	Backend
		Refactor codebase with suggested principles
		Setup postgreSQL connector functions
		Setup arangodb connection
		Authentication
			Sign up - 
				username, password
				Check if username exists
				create user
			Login -
				Get username password, see if user exists
				If user, return jwt
			Handle jwt -
				Access tokens validation for every query
				Refresh tokens handling for new access token
	Frontend
		Signup and login functionality
			Basic POST request for signup and login
			Check access token expiration. If expired, send refresh token for new access token
		UI themes
			Finalise UI themes
			Edit existing frontend to handle new UI
		Landing page 
			Design and content
			Implement this 			
	Graph
		Retrieval
			Choose most appropriate nodes - embedding distance similarity - choose k nearest nodes
			Traverse from those k nodes
			Choose most appropriate nodes while traversing - how?
			Stop traversing - how?
		Building
			Account for all other languages
			
			
				