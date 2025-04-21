
# Nument: Project Update

## Current Progress

- Authentication system is live – users can sign up and log in.
- Users can chat with the AI bot and ask questions about code(with partial augmentation).
- Public GitHub repository search is functional and integrated.
- Core chatbot interface is built and working as expected.
- All backend services are up and communicating through a microservice setup.
- Graph system is building the graph with embeddings across multiple programming languages.
- Chat history is stored and accessible for each user session.
- Database systems (PostgreSQL, Supabase, ArangoDB) are fully operational and containerized.

## Next Milestone (Finalizing MVP)

- Add secure access control to all services using JWT tokens. 
- Set up consistent logging and monitoring across services.
- Enable private repository access by integrating with GitHub, GitLab, and Bitbucket.
- Implement graph retrieval — this will power in-depth codebase understanding.
- Connect graph insights directly into the chatbot flow.
- Conduct final UI polish and bug fixes for a seamless experience.
- Caching of 
	- Models
	- Sessions
	- Graphs accessed

## Timeline (Next 7 Days)
# Nument: 7-Day Task Timeline by Team

| Day       | Graph Team                            | Backend Team                                       | Frontend Team                                      |
| --------- | ------------------------------------- | -------------------------------------------------- | -------------------------------------------------- |
| **Day 1** | Start graph retrieval logic           | Implement JWT-based authorization across services  | Polish chat UI and improve user flow               |
| **Day 2** | Define graph query structure          | Begin standard logging setup                       | Add UI feedback/loaders for chat and repo search   |
| **Day 3** | Continue graph retrieval development  | Integrate GitHub, GitLab, Bitbucket authentication | Start frontend integration for repo authentication |
| **Day 4** | Integrate retrieval with backend APIs | Finalize logging across services                   | Connect frontend to updated backend endpoints      |
| **Day 5** | Finalize graph retrieval endpoints    | Connect graph retrieval with chatbot handler       | Integrate graph results into chat responses        |
| **Day 6** | Test and tune graph retrieval         | Final microservice testing and cleanup             | UI polish and cross-browser testing                |
| **Day 7** | Internal testing with real codebases  | Security audit and config finalization             | End-to-end testing and packaging for demo          |


### Long term tasks


- Payment method 
- Refactor code
- User dashboard

### Concerns to raise
- Landing page with pre-registration/Waiting list
