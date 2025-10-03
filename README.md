# GiftOfGivers
This project is a web-based application designed to support disaster relief efforts by enabling efficient incident reporting, donation management, volunteer coordination, and administrative oversight. # Gift of Givers – ASP.NET Core MVC

This project implements user registration/login (Identity), profile management, incident reporting, volunteer task management, and admin seeding.

## Quick Start
- .NET 8 SDK (global.json pins 8.0.305)
- Run DB migrations:

- **Seed admin + roles are executed at startup.**
  The app runs EF Core migrations and calls `SeedService.SeedDatabase(...)` on launch, creating roles (`Admin`, `User`) and an admin user (`admin@codehub.com` / `Admin(123)`).

- **Start app:**
  ```bash
  dotnet restore
  dotnet ef database update --project "Gift of Givers/Gift of Givers.csproj"
  dotnet run --project "Gift of Givers/Gift of Givers.csproj"


