### Spring boot BOM
[On github](https://github.com/spring-projects/spring-boot/blob/master/spring-boot-project/spring-boot-dependencies/build.gradle)

### Show auto-config and other debug stuff in logs
```
// application.yml
debug: true
```

### GUI browser for actuator endpoints
```
// build.gradle
  implementation 'org.springframework.data:spring-data-rest-hal-browser:3.3.8.RELEASE'

// application.yml
management:
  endpoints:
    web:
      exposure:
        include: '*'


// browser url
/servlet/context-path/browser/index.html


```

### log sql statements and arguments
```
// application.yml
spring:
  jpa:
    show-sql: false
    hibernate:
      format_sql: true
    properties:
      hibernate:
        format_sql: true

```
