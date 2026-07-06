# API Gateway

Routes incoming requests to cinema microservices.

## Requirements

- Java 21
- cinema-core-service running on port 8081
- cinema-booking-service running on port 8082

## Running the Application

```bash
./mvnw spring-boot:run
```

Gateway runs on `http://localhost:8080`

## Routing

| Path | Service |
|------|---------|
| `/api/films/**` | cinema-core-service |
| `/api/salons/**` | cinema-core-service |
| `/api/seanslar/**` | cinema-core-service |
| `/api/auth/**` | cinema-booking-service |
| `/api/rezervasyonlar/**` | cinema-booking-service |
| `/api/biletler/**` | cinema-booking-service |

## Tech Stack

- Java 21
- Spring Cloud Gateway
- Spring Security