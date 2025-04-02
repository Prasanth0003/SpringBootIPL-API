# Spring Boot IPL API

A RESTful API built with Spring Boot for managing IPL (Indian Premier League) player data.

## Overview

This project is a Spring Boot application that provides endpoints for managing IPL player information. It uses Spring Web, Web Services, and WebFlux for building reactive web applications.

## Prerequisites

- Java 17 or higher
- Maven 3.6 or higher
- Docker (optional, for containerization)

## Tech Stack

- Spring Boot 3.4.4
- Spring Web
- Spring Web Services
- Spring WebFlux
- Maven
- Docker

## Project Structure

```
src/main/java/com/example/demo/
├── Player.java              # Player entity class
├── PlayerController.java    # REST controller for player endpoints
├── PlayerService.java       # Business logic for player operations
└── SpringBootIplApiApplication.java  # Main application class
```

## Getting Started

### Building the Application

```bash
mvn clean install
```

### Running the Application

```bash
mvn spring-boot:run
```

The application will start on `https://ipl-api-i1el.onrender.com`

### Docker Support

To build and run the application using Docker:

```bash
docker-compose up --build
```

## API Endpoints

The API provides the following endpoints:

- `GET /api/players` - Get all players
- `GET /api/players/team/{id}` - Get player by ID (CSK,SRH,RCB...)
- `POST /api/players` - Create a new player
- `PUT /api/players/team/{id}` - Update player information
- `DELETE /api/players/team/{id}` - Delete a player

## Testing

The project includes test dependencies for both Spring Boot and WebFlux testing. Run the tests using:

```bash
mvn test
```

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Author

Prasanth

## Acknowledgments

- Spring Boot team for the excellent framework
- IPL for the inspiration 
