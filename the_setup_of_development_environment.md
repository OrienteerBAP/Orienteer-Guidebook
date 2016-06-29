# The Setup of Development Environment

##Prerequisites

* java 7+.
* git.
* maven.
* OrientDB (if you want to use an external OrientDB database).

##Steps
1. Install [wicket-orientdb github SNAPSHOT](https://github.com/OrienteerDW/wicket-orientdb). This step is optional: wicket-orientdb SNAPSHOT is always available on Maven central.
```  
  git clone <your fork URL for wicket-orientdb>
  cd wicket-orientdb
  mvn clean install
```
2. Install Orienteer
```
  cd ..
  git clone <your fork URL for Orienteer>
  cd Orienteer
  mvn clean install
```
3. Modify *orienteer.properties* file (see [configuration section above](https://orienteer.gitbooks.io/orienteer/content/editing_the_orienteer_configuration_file.html)).
4. Compile the code `mvn clean install`
5. Run jetty server `mvn jetty:run`
6. To access the application, in your browser, go to http://localhost:8080.