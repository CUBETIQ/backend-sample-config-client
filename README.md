### Sample Config Client

#### Add libras for client config
```groovy
implementation 'org.springframework.boot:spring-boot-starter-actuator'
implementation 'org.springframework.cloud:spring-cloud-starter-config'
```

#### Add config bootstrap
```yml
spring:
  application:
    name: config-client-sample
  cloud:
    config:
      uri: ${CONFIG_URL:https://config-apren.cubetiqs.com}
      profile: config-client-sample
      username: SomboCheaRootAdmin
      password: noRootPassword7891
```