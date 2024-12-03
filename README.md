# Repository Pattern in .NET Core 8

This repository demonstrates the implementation of the Repository Pattern in a .NET Core 8 application. The Repository Pattern is a popular design pattern used to separate the logic that retrieves data from the logic that maps it to the business domain model. It promotes clean code architecture and ensures maintainability and testability.

## Features

- **Separation of Concerns**: Clean separation between data access and business logic.
- **Dependency Injection**: Uses .NET Core's built-in dependency injection framework.
- **Unit of Work**: Ensures atomicity and manages multiple repositories.
- **Asynchronous Programming**: Fully asynchronous data access methods using `async` and `await`.
- **Entity Framework Core Integration**: Supports EF Core for database operations.
- **Clean Code Practices**: Follows SOLID principles and clean architecture.

---

## Table of Contents

- [Getting Started](#getting-started)
- [Project Structure](#project-structure)
- [Setup and Configuration](#setup-and-configuration)
- [Usage](#usage)
- [Unit Testing](#unit-testing)
- [Contributing](#contributing)
- [License](#license)

---

## Getting Started

To get started with this repository, clone it to your local machine and follow the instructions below to set up and run the application.

### Prerequisites

- .NET SDK 8.0 or higher
- SQL Server (or your preferred database)
- Visual Studio 2022+ (or any preferred IDE)

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/reddix-dotnet/RepositoryPattern.git
   cd RepositoryPattern

2. Restore dependencies:
   ```bash
   dotnet restore

3. Apply database migrations:
   ```bash
   dotnet ef database update
   
4. Run the application:
   ```bash
   dotnet run

### Project Structure

Here is an overview of the project structure:

src/
├── Controllers/         # API Controllers
├── Data/                # Database context and seed data
├── Models/              # Domain models
├── Repositories/        # Interfaces and repository implementations
│   ├── IRepository.cs   # Generic repository interface
│   ├── Repository.cs    # Generic repository implementation
│   ├── IUnitOfWork.cs   # Unit of Work interface
│   └── UnitOfWork.cs    # Unit of Work implementation
├── Services/            # Business logic layer
├── Startup.cs           # Application setup and middleware
└── Program.cs           # Main entry point


