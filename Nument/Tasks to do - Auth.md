- Wrapper classes
	- Valkey - HIGH PRIORITY
		- Session handling
	- PostgreSQL - HIGH PRIORITY
		- user information CRUD
		- Design schema as well
	- Kafka - LOW PRIORITY
	- ArangoDB - MEDIUM PRIORITY
	- Authentication 
		- will be wrapper around baseHTTP class
		- Validate user for every request from the http headers received
			- Should handle refresh tokens
			- Should set cookies
- Authentication system
	- Option to login with google account - OAuth
		- Store that jwt token
	- Salt, hash password and store them
		- Generate jwt from that
		- use this jwt to validate 
	- Generated jwt tokens - goes within session of valkey

- Schemas to decide on 
	- RelationalDB
	- Session for valkey

- Logging 
	- In JSON format - set a standard code for this

