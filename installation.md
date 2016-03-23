# Installing Orienteer
---
**Installation options**

You have two options for installing Orienteer:
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

To install Orienteer in embedded mode, download the latest installation file *orienteer.war* ([link](https://github.com/OrienteerDW/Orienteer/releases), select latest version).

If you want to install Orienteer without using the administration console:
1. Copy the installation file to the  application deployment folder.
2. Create the Orienteer configuration file *orienteer.properties* and edit it according to your environment (see [Editing the Orienteer Configuration File](https://orienteer.gitbooks.io/orienteer/content/editing_the_orienteer_configuration_file.html)).
3. Copy the *orienteer.properties* file to the directory containing *orienteer.properties* file or to any directory above.
4. Run the application server.

If you want to install Orienteer over the administration console of your application server:
1. Deploy the installation file on your application server over administration console.
2. Configure Orienteer by one of the following ways:
  * Create the Orienteer configuration file *orienteer.properties* and edit it according to your environment (see [Editing the Orienteer Configuration File](https://orienteer.gitbooks.io/orienteer/content/editing_the_orienteer_configuration_file.html)) and copy it to...
  * If you don't want to create a configuration file, you can set network parameters of Orienteer in management console and other parameters in system environment variables. 
5. Run the application server.

---
**Installing Orienteer in standalone mode**

In standalone mode, Orienteer runs itself with an embedded jetty server.

To install Orienteer in standalone mode:
1. Download the latest installation file *orienteer-standalone.war* file from ([link](https://github.com/OrienteerDW/Orienteer/releases), select latest version).
2. Put the *orienteer-standalone.war* file into any directory. This will be the Orienteer installation directory.
3. Create the Orienteer configuration file *orienteer.properties* and edit it according to your environment (see [Editing the Orienteer Configuration File](https://orienteer.gitbooks.io/orienteer/content/editing_the_orienteer_configuration_file.html)).
5. Run Orinteer by executing the command  
>java -Xmx512m -Xms512m -jar orienteer-standalone.jar

 With this command, you may specify additional parameters:
 * *--config=&lt;filename&gt;* //the path to the Orienteer configuration file.
 * *--embedded* //to run an embedded OrientDB database. By default Orienteer runs an external OrientDB database. By setting this parameter you make it run an embedded OrientDB database. 
  * *--port=&lt;port number&gt;* //run Orienteer on a specified port (by default: 8080).
 * *--help* //view help.
 
 The Java VM parameters can be adjusted accordingly.
 
 ~~что имеется в виду? что конкретно и в каких случаях нужно сделать?~~
 
