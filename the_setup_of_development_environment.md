# The Setup of Development Environment

Go to orienteer-core module

##Prerequisites
* java 7+
* git
* maven
* OrientDB, if you want to use OrientDB remotely

##Steps
1. Install of [wicket-orientdb](https://github.com/OrienteerDW/wicket-orientdb) github SNAPSHOT. This step is optional: wicket-orientdb SNAPSHOT is always available on Maven central
  
  >git clone &lt;your fork URL for wicket-orientdb&gt;
  >
  >cd wicket-orientdb
  >
  >mvn clean install


2. Install Orienteer

  >cd ..

  >git clone &lt;your fork URL for Orienteer&gt;

  >cd Orienteer

  >mvn clean install

3. Modify orienteer.properties file (see [configuration section above](https://orienteer.gitbooks.io/orienteer/content/editing_the_orienteer_configuration_file.html)).
4. Compile the code
  >mvn clean install
5. Run jetty server
  >mvn jetty:run
6. To access the application: in your browser, go to http://localhost:8080.