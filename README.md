# GitSmart (Demo)

This repository contains a small demo ASP.NET Core Razor Pages application named "GitSmart". It's intended as an example project to demonstrate a minimal Razor Pages site structure, configuration patterns, and how to build and run the app locally.

## Functional description

- Minimal Razor Pages web application (ASP.NET Core).
- Serves static assets from `wwwroot` (CSS, JS, images) and Razor Pages in the `Pages/` folder.
- Reads optional database credentials from environment variables `DB_USERNAME` and `DB_PASSWORD` (currently unused but shown in `Program.cs` to demonstrate configuration patterns).
- Includes a simple error page and basic layout under `Pages/Shared`.

This project is a demo only and is not intended for production use.

## Architecture

- Framework: .NET 9 (ASP.NET Core)
- Project type: Razor Pages web application (minimal host in `Program.cs`).
- Key components:
  - `Program.cs` — application startup, service registration, middleware configuration, and endpoint mapping.
  - `Pages/` — Razor Pages (views and page models).
  - `wwwroot/` — static assets (CSS, JS, images, libraries).
  - `appsettings.json` / `appsettings.Development.json` — configuration for different environments.

The app uses the minimal hosting model provided by ASP.NET Core. Static assets are mapped and Razor Pages are enabled through the service registration and endpoint mapping calls in `Program.cs`.

## Build and run

Prerequisites:

- .NET 9 SDK installed (verify with `dotnet --version`).

From a command prompt (PowerShell recommended on Windows):

1. Restore and build the project:

```powershell
dotnet restore
dotnet build --configuration Debug
```

2. Run the project:

```powershell
dotnet run --project .
```

3. Open a browser and navigate to https://localhost:5001 or the URL printed by the app.

Environment variables

You can optionally set environment variables to demonstrate configuration usage in `Program.cs`:

```powershell
$env:DB_USERNAME = "yourusername"
$env:DB_PASSWORD = "yourpassword"
dotnet run --project .
```

Notes

- The example includes placeholder code for connecting to a database (commented out). If you add a real database connection, avoid committing secrets to source control.
- The app is intentionally minimal; use it as a starting point for experimenting with Razor Pages, middleware, and configuration patterns.

## Development suggestions

- Add unit/integration tests for page models or services.
- Wire up a real database connection and move credentials to user secrets or a secure store (e.g., Azure Key Vault) before using in non-demo scenarios.
- Add Dockerfile or GitHub Actions workflow for CI if you plan to extend this demo.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
