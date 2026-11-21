# Smart Campus Service Portal — Experiment 11
ASP.NET Core MVC + EF Core + SQLite + REST API based on the uploaded reference PDF.

## Run in Visual Studio 2022
1. Extract ZIP and open `SmartCampusServicePortal.csproj`.
2. Wait for NuGet restore.
3. Press F5. The SQLite database `SmartCampus.db` is created automatically.
4. Open `/swagger` for API testing.

## Terminal
`dotnet restore` then `dotnet run`.

## Features
Student registration/list/details/dashboard; campus service request create/list/details/track; admin status and remarks updates; REST API GET/POST/PUT/DELETE `/api/servicerequests` and status update `/api/servicerequests/{id}/status`.

The supplied PDF has an incorrect duplicate Student class under ServiceRequest.cs; this project uses a corrected ServiceRequest model and a combined MVC/API application. SQLite is used to make setup simple without a SQL Server installation.