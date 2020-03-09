How to Test


http://localhost:8881/config-server/default

config-server = declare in eclips application.properties file 
spring.cloud.config.name=config-server
default means  =by default application.properties file data show in your browser


http://localhost:8881/config-server/prod
default means  =now  application-prod.properties file data show in your browser


Diffrance b/w cloud config and profile 

cloud config - when use cloud config don't need to restart the application (at the run time change reflect)
profile- always need to restart the application 


