# msina-disovery-service

Here we are going to conceptulize discovery service, it has following three modules:

1) Discovery-Server - This is being implemented as Eureka discovery server.
2) Service - A simple service applicaiton which will be registered with above discover server, to able discoverable by client applicaion
	When you running you can run multiple servies by passing below parameters:
	
	server.port=8081
	service.instance.name=instance 1 
	
	server.port=8082
	service.instance.name=instance 2
	
3) Client - A simple client application which try to invoke/call service applicaiton via discovery server.
Once started the application access the url: http://localhost:8080/ - You can see the it will be servered by two different instances in round robin fashion.

