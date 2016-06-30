# The Setup of Development Environment

##Prerequisites

* [Java 7+](https://www.oracle.com/java/index.html)
* [git](https://git-scm.com/)
* [maven](https://maven.apache.org/)
* [OrientDB](http://orientdb.com/) (if you want to use an OrientDB database in remote/external mode).

##Steps

1. Fork [Orienteer](https://github.com/OrienteerBAP/Orienteer) on [github](https://github.com)
2. Clone your fork of Orienteer to your computer
```
  cd ..
  git clone <your fork URL for Orienteer>
  cd Orienteer
  mvn clean install
```
3. Modify *orienteer.properties* file if needed(see [configuration section above](https://orienteer.gitbooks.io/orienteer/content/editing_the_orienteer_configuration_file.html)).
4. Go to some specific module you are working on. For example `cd orienteer-core` or `cd orienteer-web`
5. Run jetty server `mvn jetty:run` (or `mvn clean jetty:run` if you changed something in the code)
6. To access the application, in your browser, go to http://localhost:8080.