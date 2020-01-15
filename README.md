# spring-config-server
Spring Cloud Configuration server - response to give the configuration data to HTTP

# that specifey the config store localy   
spring:
  profiles:
    active: native
  
## Test with rest clint 

http://localhost:8191/service1/defaut
http://localhost:8191/service2/defaut

http://localhost:8191/service2/prod
http://localhost:8191/service2/dev