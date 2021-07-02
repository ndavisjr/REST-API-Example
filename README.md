Simple API endpoints for various code commands (ie CLI commands)
Endpoints developed: Create (POST), Read, Update (PUT), Delete (Json) Patch
Created in VS Code using .NET 3.1 Core MVC standards
Database Management: SQL Server Management Studio (localDb)
Utilizing .NET CLI, EntityFramework, Automapper, DataTransferObjects, Postman




Process:

-- General setup for nearly anything .Net --
1) Set up a Model in Models folder
2( Create a Command Repository interface)
3a) Initially set up a Mock Repository for data, converted to SQLServer later
3b) Set up a DbContext (called CommanderContext in this project)
    - connection string in appsettings.json
    - Create Data folder and add context class inheriting from DbContext
    - Update Startup.cs to register the DbContext in services
4) Migrate to database
5) Create CommandController.cs to handle calls
6) Create DTO's and use Automapper to link DTO to Model
    - CommandsProfile
7) Use JSON for patching


As an example project, .env variables are not set up.
