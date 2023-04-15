# Springboot-Microservice
Springboot-Microservice


Supported matrix:
=====================

https://github.com/spring-cloud/spring-cloud-release/wiki/Supported-Versions




eureka:
http://localhost:8761/


hystrix:
http://localhost:9295/hystrix 
http://localhost:9295/hystrix/monitor?stream=http%3A%2F%2Flocalhost%3A9191%2Factuator%2Fhystrix.stream


zipkin:
http://127.0.0.1:9411



http://localhost:9191/actuator/hystrix.stream



curl --location --request POST 'http://localhost:9191/departments/' \
--header 'Content-Type: application/json' \
--data-raw '{
    "departmentName": "CSE",
    "departmentAddress": "MIST",
    "departmentCode": "001"
}'


curl --location --request GET 'http://localhost:9191/departments/1' \
--header 'Content-Type: application/json' \
--data-raw '{
    "departmentName": "CSE",
    "departmentAddress": "MIST",
    "departmentCode": "001"
}'





curl --location --request POST 'http://localhost:9191/users/' \
--header 'Content-Type: application/json' \
--data-raw '{
    "firstName": "RAJU",
    "lastName": "SHARKAR",
    "email": "raju@istlbd.com",
    "departmentId": 1
}'


curl --location --request GET 'http://localhost:9191/users/1' \
--header 'Content-Type: application/json' \
--data-raw '{
    "firstName": "RAJU",
    "lastName": "SHARKAR",
    "email": "raju@istlbd.com",
    "departmentId": 1
}'




