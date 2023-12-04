# OnlineShopAPI
Technologies: C#, ASP.NET Core Web API 6.0, Entity Framework Core, MS SQL.

API for handling core functionalities of ecommerce online shop.

I was working on the backend of online shop. Check READ ME.

Backend was developed using ASP.NET Core Web API and Entity Framework Core – Code-first approach. Microsoft SQL Server was used for the database. 

First of all, I created conceptual data model (using PowerDesigner), and defined data schema, along with entities and relationships between them. 

Based on that, then, I created a solution (using Visual Studio), with Web API project, and another project – Core, which was basically used for the core logic of the app – models, abstractions (interfaces), etc. 

My architecture of the API was designed in a very simple and straight-forward manner as: 

- Web API project (Dependency injections – registering dependencies, middlewares – global exception handler middleware, controllers, app configuration - appSettings);

- Application project (business logic  - service layer);

- Core project (models – entities, views, dtos; mapping between models, abstractions – interfaces);

- Common project (constants, password hasher class, exception classes);

- Data project (ef migrations, repository layer, db context).

Business logic of the API contains all core functionalities and CRUD operations for online shop app, as management of  Accounts, Products, Items (in the bill), and Bills.
