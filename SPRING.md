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
  implementation 'org.springframework.data:spring-data-rest-hal-explorer'

// application.yml
management:
  endpoints:
    web:
      exposure:
        include: '*'


// browser url
/servlet/context-path/index.html


```

### log sql statements and arguments
```
// application.yml
spring:
  config:
    activate:
      on-profile: default
  jpa:
    show-sql: true
    properties:
      hibernate:
        format_sql: true
        order_inserts: true
        jdbc:
          batch_size: 500

logging:
  level:
    org:
      hibernate:
        type: trace
        stat: debug

```
