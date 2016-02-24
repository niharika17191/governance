The GC-Events project provides a Node.js 
application that renders some amazing charts 
showing InfoSphere event statistics. 
It uses the Message Hub service to communicate with
an Information Server Kafka client. 

Usage:

1. Fork this project into your DevOps Services project and deploy it
2. From the iis folder, copy the gcevents.jar to your Information Server machine and run
   
   java -jar gcevents.jar localhost:52181 http://gc-events.mybluemix
net demo 

 NOTE: specify the URL that routes to your Bluemix application.
3. In a browser open your Bluemix application, for example http://gc-events.mybluemix

The appication shows some charts and you can see how they get updated in real-time as events come in. With the demo parameter, the application creates automatically creates sample events. You can omit the demo parameter to just read the events coming from Information Server. 