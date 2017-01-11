### edit below parameter, then you can switch thymeleaf version.

- build.gradle

```groovy
// thymeleaf3.x
ext['thymeleaf.version'] = '3.0.3.RELEASE'
// thymeleaf2.x
//ext['thymeleaf.version'] = '2.1.5.RELEASE'
```

- src/resources/application.yml

```yaml
spring:
  thymeleaf:
# thymeleaf3.x
    mode: HTML
# thymeleaf2.x
#    mode: HTML5
```

### refresh gradle project and start application 

```bash
./gradlew bootRun
```

### confirm result

```bash
curl http://localhost:8080
```

