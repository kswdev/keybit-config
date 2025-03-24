server:
  port: 8085

spring:
  application.name: tag
  data:
    mongodb:
      host: localhost
      port: 27017
      database: tag
      username: root
      password: root

  jpa:
    defer-datasource-initialization: true
    hibernate.ddl-auto: create
    show-sql: true
    properties:
      hibernate:
        format_sql: true
        default_batch_fetch_size: 100

logging:
  level:
    org.springframework.data.mongodb.repository: DEBUG
    org.mongodb.driver: DEBUG

consumers:
  topic:
    tag:
      group-id: tag
      change: tag_changed

producers:
  bootstrap-servers: localhost:9092
  topic:
    tag:
      register: tag_registered
