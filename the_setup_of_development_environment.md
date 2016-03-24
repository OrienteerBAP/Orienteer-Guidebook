# The Setup of Development Environment

https://github.com/OrienteerDW/Orienteer/wiki/How-to-run-Orienteer
Go to orienteer-core module
Run the following command in console mvn jetty:run
If you made some changes in Orienteer consider running mvn clean jetty:run
Go to in your browser to http://localhost:8080



Prerequisites
1.	java 7+
2.	git
3.	maven
4.	OrientDB, if you want to use OrientDB remotely

Steps
1. Install of wicket-orientdb github SNAPSHOT

  This step is optional: [wicket-orientdb](https://github.com/OrienteerDW/wicket-orientdb) SNAPSHOT always available on Maven central
  
  >git clone &lt;your fork URL for wicket-orientdb&gt;
  >cd wicket-orientdb
  >mvn clean install


2. Install Orienteer

  >cd ..
  >
  >git clone &lt;your fork URL for Orienteer&gt;
  >
  >cd Orienteer
  >
  >mvn clean install


Modify orienteer.properties file
See configuration section above
Code compilation
mvn clean install
Run jetty server by command
mvn jetty:run
Goto the application
Open http://localhost:8080 is in your browser

