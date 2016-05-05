# Installing Orienteer in the Embedded Mode

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
