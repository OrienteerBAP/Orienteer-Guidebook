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
1. Download the newest *orienteer.war* file from LOCATION.
>What is the link to download?
2. Put the *orienteer.war* file into the deployment folder of your application server.
>What is deployment folder for your application server? Where is it on Windows, Linux etc?
3. Configure *orienteer.properties* according to your environment and place it in the same directory or above.
4. Run application server.

---
**Installing Orienteer in standalone mode**

In the standalone mode, Orienteer runs itself with an embedded jetty server.

To install Orienteer in standalone mode:
1. Download the newest *orienteer-standalone.war* file from LOCATION.
>What is the link to download?
2. Put the *orienteer-standalone.war* file into any directory.
3. Optionally configure orienteer.properties accordging to your environment and place it in the same directory or above.
 * By default, Orienteer, will run OrientDB database embedded.
4. Run Orinteer as java -Xmx512m -Xms512m -jar orienteer-standalone.jar. JVM parameters can be adjusted accordingly. Additional application parameters can be supplied:
 * --config=<filename> - specification of path to orienteer configuration file
 * --embedded - run embedded OrientDB database
 * --port=<port number> - run Orienteer on specified port (Default: 8080)
 * --help - display help