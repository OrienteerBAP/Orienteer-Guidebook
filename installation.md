# Installing Orienteer

Initial installation of Orienteer is as easy as double-click on a file. This is the first step towards implementation of a dedicated business app.

Before installing, you may want [to test-drive a deployed Orienteer database](http://demo.orienteer.org/login).

## Installation Options and System Requirements

There are two options for Orienteer installation:
* The embedded mode: on an application server. Orienteer can be installed on all famous compatible web application servers:
  * [WildFly/Jboss](http://wildfly.org/),
  * [Weblogic](https://www.oracle.com/middleware/weblogic/index.html),
  * [IBM WebSphere](http://www-03.ibm.com/software/products/en/appserv-was),
  * [Apache Tomcat](http://tomcat.apache.org/),
  * [Jetty](http://www.eclipse.org/jetty/),
  * and others.


* The standalone mode: on any computer that runs Java environment.

## Installing Orienteer as a Standalone Application

In standalone mode, Orienteer utilizes an embedded [jetty server](http://www.eclipse.org/jetty/) to run itself as a web application.

To install Orienteer in standalone mode:
1. Download the latest installation file *orienteer-standalone.war* file ([link](https://github.com/OrienteerDW/Orienteer/releases), select latest version).
2. Put the *orienteer-standalone.war* file into any directory.
3. [Create the Orienteer configuration file *orienteer.properties*](https://orienteer.gitbooks.io/orienteer/content/editing_the_orienteer_configuration_file.html).
4. Run Orinteer by executing the command  
>java -Xmx512m -Xms512m -jar orienteer-standalone.jar

 Additional parameters:
 * >--config=&lt;filename&gt;
   
    the path to the Orienteer configuration file.
 * >--embedded
   
    By default Orienteer runs an external OrientDB database. If you give this parameter, Orienteer will run an embedded OrientDB database.
  * >--port=&lt;port number&gt;
  
    run Orienteer on a specified port (by default: 8080).
 * >--help
   
    view help.
 
 The Java VM parameters can be adjusted accordingly.
 
## Installing Orienteer in the Embedded Mode

Download the latest installation file *orienteer.war* ([link](https://github.com/OrienteerDW/Orienteer/releases), select latest version).

To install Orienteer without using the administration console:
1. Copy the installation file to the  application deployment folder.
2. [Create the Orienteer configuration file *orienteer.properties*](https://orienteer.gitbooks.io/orienteer/content/editing_the_orienteer_configuration_file.html).
3. Copy the configuration file to the directory containing the *orienteer.war* installation file or to any directory above.
4. Run the application server.

To install Orienteer with the administration console of your application server:
1. Deploy the installation file on your application server over the administration console.
2. Configure Orienteer by one of the following ways:
  * [Create the Orienteer configuration file *orienteer.properties*](https://orienteer.gitbooks.io/orienteer/content/editing_the_orienteer_configuration_file.html) and copy it to...
  * If you don't want to create a configuration file, you can set network parameters of Orienteer in management console, and other parameters in system environment variables. 
5. Run the application server.

