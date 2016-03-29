# The Setup of Development Environment

https://github.com/OrienteerDW/Orienteer/wiki/How-to-run-Orienteer

Go to orienteer-core module

Run the following command in console mvn jetty:run

If you made some changes in Orienteer consider running mvn clean jetty:run

Go to in your browser to http://localhost:8080

##Prerequisites
* java 7+
* git
* maven
* OrientDB, if you want to use OrientDB remotely

Steps
1. Install of [wicket-orientdb](https://github.com/OrienteerDW/wicket-orientdb) github SNAPSHOT

  This step is optional: [wicket-orientdb](https://github.com/OrienteerDW/wicket-orientdb) SNAPSHOT always available on Maven central
  
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

3. Modify orienteer.properties file
  See configuration section above
4. Code compilation
  >mvn clean install
5. Run jetty server by command
  >mvn jetty:run
6. Goto the application
  Open http://localhost:8080 is in your browser

