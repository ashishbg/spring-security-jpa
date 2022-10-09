# spring-security-jpa
Spring Boot + Spring Security with JPA authentication

This project was made following [this tutorial](https://www.youtube.com/watch?v=TNt3GHuayXs) by
[Java Brains](https://www.youtube.com/c/JavaBrainsChannel)

Original source code [link](https://github.com/koushikkothagal/spring-security-jpa)

---

### Prerequisite
1. Existing Postgres DB with teh name `springsecurityjpa` and password `1234` or change te values in `application.properties` accordingly.

2. set the property `spring.jpa.hibernate.ddl-auto` to `create` instead of `update` so that new table are created automatically. 
Revert after first run.

3. Add users with this SQL statement 
```roomsql
INSERT INTO spring_user ("id", user_name, "password", roles, active) 
VALUES (1, 'user', 'pass', 'ROLE_USER', TRUE)
```  

