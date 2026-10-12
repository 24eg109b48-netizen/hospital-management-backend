# Hospital Management Backend

Spring Boot 3.3.4 REST API with Java 17 and MySQL.

## Build and run

```sh
./mvnw clean package -DskipTests
java -jar target/backend-0.0.1-SNAPSHOT.jar
```

Set `DB_URL`, `DB_USERNAME`, and `DB_PASSWORD` for MySQL. Set `FRONTEND_URL` to the frontend's exact HTTPS origin for CORS. The application listens on the host-provided `PORT` (default `8080`).

For Railway, deploy this repository root as a Java/Maven service with the build and start commands above, then add the database variables and `FRONTEND_URL`.

**Demo only:** current API authorization is permissive. Do not use real patient information or treat this as a production medical system.