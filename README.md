# spring-tips
Spring Tips i've learned over the times



### Show auto-config and other debug stuff in logs
```
// application.yml
debug: true
```

### GUI browser for actuator endpoints
```
// build.gradle
  implementation 'org.springframework.data:spring-data-rest-hal-browser:3.3.8.RELEASE'

// browser url
/servlet/context-path/browser/index.html
```
