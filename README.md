# ContosoUniversity.API

RESTful API ContosoUniversity Backend using Microsoft.AspNetCore.Identity and OpenID Connect

- ASP.NET Core 2.0 
- Entity Framework Core
- Code First Migration
- OpenID Connect
- Identity 
- Sql Server
- Automapper

Referenced [Microsoft](https://docs.microsoft.com/en-us/aspnet/core/data/ef-mvc/intro) and [chsakell](https://chsakell.com/2016/06/23/rest-apis-using-asp-net-core-and-entity-framework-core/)'s REST API best practice

## Installation

1. Clone or download this project
2. Click ContosoUniversity.sln and open with Visual Studio 2017
3. Navigate to Build - Rebuild Solution
4. Navigate to Tools - Extensions and Updates..
5. Search for Open Command Line and install (restart Visual Studio)
6. Click on ContosoUniversity.API on the Solution Explorer, and press ALT + SPACE
7. Run this migration command: dotnet ef migrations add InitialDatabase -c ContosoContext
8. Run another command which creates database: dotnet ef database update -c ContosoContext
9. Press F5 to run the project. (Make sure ContosoUniversity.API is set as startup project)

## Best Practice

- Separation of concerns is widely applied so the codes are not tightly coupled. (Ex: repository patterns)
- Used Automapper to prevent from over-posting attacks
- Fluent validation is used
- RESTful HTTP API using JSON as a data format
- JWT(JSON Web Tokens) based security (Authentication, Authorization & API calls)

## Test API

Use Postman or other API testing IDEs

- Ex: GET http://localhost:51089/api/instructors
- Access Apis based on a role (Admin or User):
  
  ![1](https://user-images.githubusercontent.com/7738916/34234638-2e99fad6-e5a1-11e7-86ca-ebea9f7c1eab.png)

  
  
  
    
