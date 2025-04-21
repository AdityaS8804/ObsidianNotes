

|          | Not started                        | In Progress                                    | Completed                                                  |
| -------- | ---------------------------------- | ---------------------------------------------- | ---------------------------------------------------------- |
| Backend  | Integration with Bitbucket, Gitlab | Authorization(80% done)                        | Authentication - with email                                |
|          | Caching with valkey                | Authentication - with google account(20% done) | Integration with Github - Public repos                     |
|          | Kafka support                      |                                                | HTTP SSE based chat with mistralAI                         |
|          |                                    |                                                | CRUD to PostgreSQL                                         |
| Frontend | User dashboard                     | UI implementation(60% done)                    | Authentication - signup and login- with email              |
|          | Landing page                       | Authorization(80% done)                        | Handle chat with http sse to chatbot                       |
|          |                                    |                                                | Render received chunks from http sse( supporting markdown) |
| Graph    |                                    | Graph retrieval(40% done)                      | Graph building for 6 language support                      |
|          |                                    |                                                | Read/write graph to arangoDB                               |
| LLM      | Wrapping it as a microservice      |                                                | Finalised LLM - Deepseek-Coder                             |
* All services have been built out with a good foundation.
* All their integrations haven't been quite built out yet. It will be the next weeks goal.