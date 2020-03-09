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

http://localhost:8881/config-server/dev





{
"name": "config-server",
"profiles": [
"dev"
],
"label": null,
"version": "c3155ee9b6f917bd1d596c59cb636db55bb40b21",
"state": null,
"propertySources": [
{
"name": "https://github.com/saannjaay/insurance-config-server/application-dev.properties",
"source": {
"user.school": "dev",
"user.name": "sanjay dev ",
"user.city": "mirzapur dev"
}
},
{
"name": "https://github.com/saannjaay/insurance-config-server/application.properties",
"source": {
"insurnace.provider.url": "http://localhost:9999/services-proider/plans"
}
}
]
}
