# ProG Coder
This project was created by ProG Coder. Visit [ProG Coder](https://www.progcoder.com) and search for the keyword `PG Shop Microservices` to see how to install it.

# PG Shop Microservices

This repository contains a suite of microservices implementing various **e-commerce** modules, including **Identity, Catalog, Basket, Discount, Order, Feedback, Search, Notification, User, Information**, and **Communicate**. These services utilize **NoSQL (DocumentDb, MongoDB, Redis)** and **Relational databases (PostgreSQL, SQL Server, MySQL)**, communicating via **RabbitMQ Event Driven Communication** and leveraging **YARP API Gateway**.

Overall picture of **implementations on microservices with .NET tools** on real-world **PG Shop microservices** project.

![PGShopMicroservices](assets/imgs/PGShopMicroservices.png)

## Technology, Design Patterns, Infrastructure & Architecture

### Infrastructure

- **`Windows 11`** - The OS for developing and building this demo application.
- **[`WSL2 - Ubuntu OS`](https://docs.microsoft.com/en-us/windows/wsl/install-win10)** - The subsystem that helps to run easily the bash shell on Windows OS.
- **[`Docker for Desktop (Kubernetes enabled)`](https://www.docker.com/products/docker-desktop)** - The easiest tool to run Docker, Docker Swarm, and Kubernetes on Mac and Windows.
- **[`Kubernetes`](https://kubernetes.io) / [`AKS`](https://docs.microsoft.com/en-us/azure/aks)** - The app is designed to run on Kubernetes (both locally on "Docker for Desktop" as well as on the cloud with AKS).

### Back-end

- **[`.NET Core 8`](https://dotnet.microsoft.com/download)** - .NET Framework and .NET Core, including ASP.NET and ASP.NET Core.
- **[`Duende IdentityServer 6`](https://duendesoftware.com)** - Identity and Access Control solution for .NET Core.
- **[`YARP`](https://github.com/microsoft/reverse-proxy)** - A toolkit for developing high-performance HTTP reverse proxy applications.
- **[`FluentValidation`](https://github.com/FluentValidation/FluentValidation)** - Popular .NET validation library for building strongly-typed validation rules.
- **[`MediatR`](https://github.com/jbogard/MediatR)** - Simple, unambitious mediator implementation in .NET.
- **[`EF Core`](https://github.com/dotnet/efcore)** - Modern object-database mapper for .NET. It supports LINQ queries, change tracking, updates, and schema migrations.
- **[`Scrutor`](https://github.com/khellang/Scrutor)** - Assembly scanning and decoration extensions for Microsoft.Extensions.DependencyInjection.
- **[`Serilog`](https://github.com/serilog/serilog)** - Simple .NET logging with fully-structured events.
- **[`NEST`](https://github.com/elastic/elasticsearch-net)** - Elasticsearch.Net & NEST.
- **[`Carter`](https://github.com/CarterCommunity/Carter)** - Carter is a library that allows Nancy-esque routing for use with ASP.NET Core.
- **[`Marten`](https://github.com/JasperFx/marten)** - Marten is a .NET document database and event store library that provides a lot of flexibility and power.
- **[`AspNetCore.HealthChecks`](https://github.com/Xabaril/AspNetCore.Diagnostics.HealthChecks)** - Health checks for building services, such as ASP.NET Core.
- **[`Grpc.AspNetCore`](https://github.com/grpc/grpc-dotnet)** - gRPC for .NET, a high-performance RPC framework.
- **[`MassTransit.RabbitMQ`](https://github.com/MassTransit/MassTransit)** - Distributed application framework for .NET, supporting RabbitMQ.
- **[`Mapster`](https://github.com/MapsterMapper/Mapster)** - A high-performance object mapper in .NET.
- **[`MongoDB.Driver`](https://github.com/mongodb/mongo-csharp-driver)** - Official MongoDB .NET Driver.
- **[`Minio`](https://github.com/minio/minio-dotnet)** - MinIO .NET Client SDK for Amazon S3 compatible cloud storage.
- **[`StackExchangeRedis`](https://github.com/StackExchange/StackExchange.Redis)** - General purpose Redis client for .NET.
- **[`Polly`](https://github.com/App-vNext/Polly)** - Polly is a .NET resilience and transient-fault-handling library.
- **[`OpenTelemetry`](https://opentelemetry.io)** - OpenTelemetry provides observability frameworks for cloud-native software, including metrics, logs, and traces.

### Front-end

- **[`nodejs 14.x`](https://nodejs.org/en/download)** - JavaScript runtime built on Chrome's JavaScript engine.
- **[`TypeScript`](https://www.typescriptlang.org)** - Typed superset of JavaScript that compiles to plain JavaScript.
- **[`ReactJS`](https://reactjs.org)** - A JavaScript library for building user interfaces.
- **[`Next.js`](https://nextjs.org)** - The React Framework for Production.

### Design Patterns
- **Decorator** - A structural pattern that allows behavior to be added to individual objects, dynamically, without affecting the behavior of other objects from the same class.
- **Strategy** - A behavioral pattern that enables selecting an algorithm's behavior at runtime.
- **CQRS** - Command Query Responsibility Segregation, a pattern that separates read and write operations.
- **Saga** - A pattern for managing failures, ensuring data consistency across microservices.

### Architecture
- Implementation of **DDD, CQRS, and Clean Architecture** following best practices.

![CleanArchitecture](assets/imgs/CleanArchitecture.png)

## Web UI Screenshots

### Admin
![Admin](assets/imgs/screenshots/admin/home.JPG)

### User
![User](assets/imgs/screenshots/user/home.JPG)

All screenshots are stored in [assets/imgs/screenshots](assets/imgs/screenshots).

## Data Infrastructure

### MinIO
- Object storage solution designed for high performance and scalability.
- Ideal for storing images, files, and other unstructured data.

### Zipkin
- Distributed tracing system for monitoring and troubleshooting microservices.
- Helps in identifying latency issues and tracking the flow of requests across services.

### Seq
- Centralized log management system for aggregating and visualizing service logs.
- Provides powerful querying capabilities and real-time insights into application behavior.

### Airflow
- Workflow automation and scheduling system, with jobs written in Python.
- Navigate to the `airflow` directory to see all DAGs (Directed Acyclic Graphs) and workflows.
- Facilitates complex data engineering and ETL processes.

## Running the Project
For detailed instructions on running and installing the project, visit [ProG Coder](https://www.progcoder.com) and search for the keyword `PG Shop Microservices` to see how to install it.

## Services, Infrastructure, and Web UI Access
For detailed information on all services, infrastructure, and web UI, including port usage and URLs, visit [ProG Coder](https://www.progcoder.com) and search for the keyword `PG Shop Microservices`.

- **Ports and URLs**: Detailed port configurations and URLs for accessing various services are provided in the documentation.
- **User Access**: Instructions on how to access the web UI for both admin and user roles are included.

For more information, please refer to the [ProG Coder](https://www.progcoder.com) website.

## Detailed Service Flow
For an in-depth look at each service, please navigate to the `src/Services` directory and read `Readme.md`.

## Give a Star! :star:
If you liked the project or if it helped you, please **give a star**.

## Bugs, Feature Requests, and Contributing
We welcome community contributions. We use GitHub issues to track bugs and feature requests, and pull requests to manage contributions. See the [contribution information](.github/CONTRIBUTING.md) for more details.

## Donate
Donate me at [Buy Me a Coffee](https://buymeacoffee.com/progcoder).

## Authors

- **Huy Nguyen** - *Initial work* - [huynxtb](https://github.com/huynxtb)

See also the list of [contributors](https://github.com/huynxtb/pg-shop-microservices/contributors) who participated in this project.

## License
Code released under [the MIT License](https://github.com/huynxtb/pg-shop-microservices/blob/main/LICENSE)
