1. Проект: REST API с JWT аутентификацией на Spring Boot
  
2. Собрать и запустить
   mvn clean package
   docker run --name postgres-jwt -e POSTGRES_PASSWORD=postgres -e POSTGRES_USER=postgres -e POSTGRES_DB=jwt -p 5433:5432 -d postgres:15
   java -jar target/RESTwithJWT-0.0.1-SNAPSHOT.jar
   Доступ через /api/auth
   
3. Технические особенности
   Реализована JWT аутентификация и авторизация 
   Использован Spring Security для защиты endpoints
   Роли и права доступа пользователей
   Настроена работа с PostgreSQL через Spring Data JPA
