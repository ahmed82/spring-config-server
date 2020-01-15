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
  
## Test with rest clint 

http://localhost:8191/service1/defaut
http://localhost:8191/service2/defaut

http://localhost:8191/service2/prod
http://localhost:8191/service2/dev