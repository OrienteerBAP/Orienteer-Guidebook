# Installing as a Web Application

Orienteer can be installed on all famous compatible web application servers:
  * [WildFly/Jboss](http://wildfly.org/),
  * [Weblogic](https://www.oracle.com/middleware/weblogic/index.html),
  * [IBM WebSphere](http://www-03.ibm.com/software/products/en/appserv-was),
  * [Apache Tomcat](http://tomcat.apache.org/),
  * [Jetty](http://www.eclipse.org/jetty/),
  * and others.

Download the latest installation file *orienteer.war* (follow [this link](https://github.com/OrienteerDW/Orienteer/releases), select latest version).

To install Orienteer without using the administration console:
1. Copy the installation file to the  application deployment folder.
2. [Create the Orienteer configuration file *orienteer.properties*](configuration_file.md).
3. Copy the configuration file to the directory containing the installation file or to any directory above.
4. Run the application server.

To install Orienteer with the administration console of your application server:
1. Deploy the installation file on your application server over the administration console.
2. Configure Orienteer in one of the following ways:
  * [Create the Orienteer configuration file *orienteer.properties*](configuration_file.md) and copy it to working directory or one of its parent directories.
  * If you don't want to create a configuration file, you can set network parameters of Orienteer in management console, and other parameters in system environment variables. 
5. Run the application server.


