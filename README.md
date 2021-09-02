# **About ASP.NET Core WebAPI – Clean Architecture**

Modular development was a prime requirement for me when we got started. Adapting to a Microservice architecture was the first choice me had. But given the complexities with the mentioned architecture, me decided to stay away from it atleast for the starting.

For API, ASP.NET Core 5.0 was me obvious choice.

The WebAPI application had to be highly modular to improve development experience. Each of these modules has its own controllers / interfaces / dbContext. As for the DB providers, mssql will be used. One module cannot directly talk to the other module nor modify its table. CrossCutting concerns would use interfaces/ events. And yes, domain events are also included in the project using mediatr Handler. Each of the module follows a clean architecture design / Onion / Hex.

**Technology Stack** 💪
API - ASP.NET Core 5.0 WebAPI
Data Access - Entity Framework Core 5.0
DB Providers - MSSQL

**Project Status**
API - In Progress
Seperate Website to maintain documentation - Coming Soon!
Docker Container - Coming Soon!

Clone this repository to your local machine.

**Prerequisites to run API**
Install the latest .NET 5 SDK
Install the latest DOTNET & EF CLI Tools by using this command dotnet tool install --global dotnet-ef
Install the latest version of Visual Studio IDE 2019 (v16.8 and above) 🚀
It's recommended to use MsSQL as it comes by default with ASP.NET Core WebAPI – Clean Architecture. Install MsSQL.

**Running the API**
Open up NetCoreApiStarterKit.sln in Visual Studio 2019.
Navigate to appSettings.json
Add you PostgreSQL connection string under ConnectionStrings. The default connection string is "DefaultConnection": "Server=.\\HAKAN;Database=NetCoreApiStarterKit;Trusted_Connection=True;"
That's everything you need to setup the API. Just build and run the API project.
By default, the database is migrated and latest changes are applied.
Some default data is also seeded to this database like roles, users, brands, products etc.

**Note**
Since ASP.NET Core WebAPI – Clean Architecture is in it's early development stage, I have not been able to write detailed documentation about the implementation.

**The Team**
Hakan GÜZEL @hakanguzel
