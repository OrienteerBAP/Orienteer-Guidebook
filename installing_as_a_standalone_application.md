# Installing Orienteer as a Standalone Application

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
