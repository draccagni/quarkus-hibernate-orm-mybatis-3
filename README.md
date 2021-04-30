# Quarkus demo: Hibernate ORM with MyBatis 3

This work has been derived from <https://github.com/quarkusio/quarkus-quickstarts/tree/main/hibernate-orm-quickstart>

## PostgreSQL

```bash
docker-compose up --build
```

### Run Quarkus as a native application on Docker

```bash
mvn clean compile package -Pnative -Dquarkus.native.container-build=true -DskipTests=true

docker build -f src/main/docker/Dockerfile.native -t quarkus-hibernate-orm-mybatis-3 .

docker run -p 8080:8080 quarkus-hibernate-orm-mybatis-3
```

## See the demo in your browser

Navigate to:

<http://localhost:8080/index.html>

Have fun, and join the team of contributors!
