# spring-config-server
Spring Cloud Configuration server - response to give the configuration data to HTTP



## Specify the config to be store localy   
spring:
  profiles:
    active: native
    
## Specify the config to be store on cloud    
spring:
  cloud:
    config:
      server:
        git:
          uri: https://github.com/ahmed82/spring-cloud-config-store    

https://cloud.spring.io/spring-cloud-config/reference/html/
  
## Test with rest clint 

http://localhost:8191/service1/defaut
http://localhost:8191/service2/defaut

http://localhost:8191/service2/prod
http://localhost:8191/service2/dev

## Test Config store server on (Git) with rest clint 
http://localhost:8192/membership/prod
http://localhost:8192/membership-prod.yml
http://localhost:8192/membership-prod.json


http://localhost:8192/membership/qa
Or use commit hash/tag or branch or other repository
http://localhost:8192/membership/qa/9a88216b427f6b43cc86d7901784a019496c7dbf


