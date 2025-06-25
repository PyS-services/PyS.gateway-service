# PyS.gateway-service

[![PyS.gateway-service CI](https://github.com/PyS-services/PyS.gateway-service/actions/workflows/maven.yml/badge.svg?branch=main)](https://github.com/PyS-services/PyS.gateway-service/actions/workflows/maven.yml)

## Overview

PyS.gateway-service is a Spring Cloud Gateway service that acts as the entry point for the PyS microservices ecosystem. It provides routing, load balancing, and API gateway functionality.

## Features

- Dynamic routing configuration
- Service discovery integration with Eureka
- Load balancing
- API gateway capabilities
- Actuator endpoints for monitoring
- Health checks

## Prerequisites

- Java 24
- Maven 3.8+
- Docker (optional)
- Spring Cloud 2025.0.0
- Spring Boot 3.5.3

## Getting Started

### Building the Application

```bash
mvn clean install
```

### Running the Application

```bash
mvn spring-boot:run
```

### Docker

Build the Docker image:
```bash
docker build -t pys-gateway-service .
```

Run the container:
```bash
docker run -p 8080:8080 pys-gateway-service
```

## Configuration

The service can be configured through the following files:
- `application.yml` - Main configuration
- `bootstrap.yml` - Bootstrap configuration

## API Documentation

The API documentation is available at:
- Swagger UI: `http://localhost:8080/swagger-ui.html`
- OpenAPI Documentation: `http://localhost:8080/v3/api-docs`

## Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct and the process for submitting pull requests.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Support

For support, please open an issue in the GitHub repository or contact the development team.

## Acknowledgments

- Spring Cloud Gateway
- Spring Boot
- Spring Cloud Netflix
- Eclipse Temurin
