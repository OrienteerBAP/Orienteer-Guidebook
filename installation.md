# Installing Orienteer
---
**Installation options**

Orienteer is a Java Servlet 3.1 web application. You have two options for installing Orienteer:
* in embedded mode (on an application server)
* in standalone mode (on any computer that runs Java environment)
---
**Installing Orienteer in embedded mode**

Orienteer can be installed on all famous compatible web containers:
* Jboss
* Weblogic
* IBM WebSphere
* Apache Tomcat
* Jetty
* and others

To install Orienteer in embedded mode:
1. Download the latest *orienteer.war* file from LOCATION.
>What is the link to download?
2. Copy the *orienteer.war* file into the application deployment folder of your application server.
>Можно ли устанавливать его через консоль администрирования сервера приложений, а не через копирование?
3. Create the Orienteer configuration file *orienteer.properties* and edit it according to your environment ().
4. Copy the *orienteer.properties* file to the same directory or above.
>Какая директория имеется в виду?
4. Run application server.

---
**Installing Orienteer in standalone mode**

In the standalone mode, Orienteer runs itself with an embedded jetty server.

To install Orienteer in standalone mode:
1. Download the latest *orienteer-standalone.war* file from LOCATION.
>What is the link to download?
2. Put the *orienteer-standalone.war* file into any directory.
3. Optionally configure orienteer.properties accordging to your environment and place it in the same directory or above.
 * By default, Orienteer, will run OrientDB database embedded.
4. Run Orinteer as java -Xmx512m -Xms512m -jar orienteer-standalone.jar. JVM parameters can be adjusted accordingly. Additional application parameters can be supplied:
 * --config=<filename> - specification of path to orienteer configuration file
 * --embedded - run embedded OrientDB database
 * --port=<port number> - run Orienteer on specified port (Default: 8080)
 * --help - display help