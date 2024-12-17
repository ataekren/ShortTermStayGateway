# ShortTermStayGateway

## Video
- [Demo Video Link](https://www.youtube.com/watch?v=exG50SbmNME)


## Overview
The `ShortTermStayGateway` is a .NET 8.0 web application that serves as an API gateway using Ocelot. It is designed to route requests to downstream services and provide a unified entry point for client applications.

## Design
- **Framework**: The project is built on .NET 8.0, leveraging ASP.NET Core for web application development.
- **API Gateway**: Ocelot is used to manage routing, request aggregation, and other gateway functionalities.
- **Configuration**: The application uses JSON configuration files (`appsettings.json`, `ocelot.json`) to manage settings and routing rules.
- **Logging**: Configured to log at the "Information" level by default, with specific settings for ASP.NET Core components.


## Assumptions
- **Local Development**: The application is assumed to be running locally, as indicated by the use of `localhost` in configuration files.
- **Downstream Services**: The downstream services are expected to be running on the specified ports and accessible via the configured hostnames.


## Configuration Files
- **appsettings.json**: Contains general application settings, including logging levels and allowed hosts.
- **ocelot.json**: Defines the routing rules for the API gateway, including upstream and downstream paths and methods.
- **launchSettings.json**: Specifies the launch profiles for the application, including URLs and environment variables.
