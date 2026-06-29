# Draw-It-or-Lose-It
8-2 Journal Portfolio Submission

## Briefly summarize The Gaming Room client and their software requirements. Who was the client? What type of software did they want you to design?

The client was The Gaming Room. They wanted to expand their existing Android game, Draw It or Lose It, into a web-based application that could run across multiple platforms. The software needed to support games and players at the same time making sure that game names and team names stayed unique. The design also needed to use a centralized server-side structure so the main business logic would not have to be rewritten separately for every device or operating system.

## What did you do particularly well in developing this documentation?

One thing I did well was organizing the system around a clear object-oriented domain model. I used a shared Entity base class for common fields like ID and name, then extended it through Game, Team, and Player classes. I also documented how GameService manages game data and uses the singleton pattern to make sure only one service instance exists during the prototype. This made the design easier to understand and helped connect the software structure back to the client’s requirements.

## What about the process of working through a design document did you find helpful when developing the code?

Working through the design document helped me think through the structure before writing or reviewing the code. Instead of jumping straight into implementation, the document forced me to identify the client’s requirements, define the main classes, and explain how the system should manage games, teams, players, names, and IDs. The UML diagram was especially useful because it showed how the classes connected to each other before the code was finalized.

## If you could choose one part of your work on these documents to revise, what would you pick? How would you improve it?

I would revise the production-level architecture section. The current document explains the recommended operating platform, storage, memory management, networking, and security, but I would make the production design more detailed. I would add more specific information about database tables, API endpoints, authentication flow, and how the system would handle simultaneous users joining or creating games at the same time. That would make the design stronger beyond the prototype stage.

## How did you interpret the user’s needs and implement them into your software design? Why is it so important to consider the user’s needs when designing?

I interpreted the user’s needs by turning the client’s game rules and platform goals into specific software requirements. Since the client needed games, teams, and players, I designed classes that directly represented those parts of the system. Since names needed to be unique, I included lookup logic before new games, teams, or players were created. Since the application needed to support multiple platforms, I recommended keeping the game logic on the server and allowing users to connect through browser-based clients.

Considering user needs is important because software is only successful if it solves the actual problem it was built for. If the design ignores the client’s requirements, the final product may work technically but still fail in real use. Focusing on the user’s needs helps prevent wasted development time, reduces redesign later, and makes the software easier to maintain and expand.

## How did you approach designing software? What techniques or strategies would you use in the future to analyze and design a similar software application?

I approached the software design by first identifying the client’s requirements and constraints, then translating those needs into classes, relationships, and design patterns. I used object-oriented design to separate responsibilities between Entity, Game, Team, Player, and GameService. I also considered platform requirements by comparing Mac, Linux, Windows, and mobile devices before recommending Linux as the best server-side option.

In the future, I would use a similar process for other applications. I would start with requirement analysis, identify the main objects in the system, create a UML diagram, define the relationships between classes, and then evaluate technical constraints such as platform support, storage, networking, security, and scalability. I would also spend more time planning for production concerns earlier, especially database design, concurrency, authentication, and deployment.
