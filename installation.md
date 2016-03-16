# Installation
---
**Installation options**

There are two options for Orienteer database installation:
* embedded (on application server)
* standalone (no need for application server)
---
**Installing Orienteer in embedded mode**

Orienteer is Java Servlet 3.1 web application and can be installed on all famous compatible containers:
* Jboss
* Weblogic
* IBM WebSphere
* Tomcat
* Jetty
* and others

To install Orienteer in embedded mode:
1. Download latest *orienteer.war* file from LOCATION.
>What is the link to download?
2. Put *orienteer.war* into deployment folder for your application server.
>What is deployment folder for your application server? Where is it on Windows, Linux etc?
3. Configure *orienteer.properties* according to your environment and place it in the same directory or above.
4. Run application server.

---
**Installing Orienteer in standalone mode**

In the standalone mode, Orienteer uses embedded jetty server to run itself.

To install Orienteer in standalone mode:
•	Download latest orienteer-standalone.jar
•	Put orienteer-standalone.war into any directory
•	Optionally configure orienteer.properties accordging to your environment and place it in the same directory or above
o	By default, Orienteer, will run OrientDB database embedded
•	Run Orinteer as java -Xmx512m -Xms512m -jar orienteer-standalone.jar. JVM parameters can be adjusted accordingly. Additional application parameters can be supplied:
o	--config=<filename> - specification of path to orienteer configuration file
o	--embedded - run embedded OrientDB database
o	--port=<port number> - run Orienteer on specified port (Default: 8080)
o	--help - display help
