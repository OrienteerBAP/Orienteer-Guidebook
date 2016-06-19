# Creating the Orienteer Configuration File

orienteer.properties is a text file that stores initial configuration parameters of your Orienteer database. You can download a sample configuration file [here](https://github.com/OrienteerDW/Orienteer/blob/master/orienteer.properties). 

**Configurations**

* Run Orienteer in the production mode (true) or in the development mode (false). The production mode provides broader means for debugging. 

  `orienteer.production=[true|false]` 
*  Run an embedded OrientDB server (true) or an external OrientDB server (false).
  
  `orientdb.embedded=[true|false]`
*  If you are running an external OrientDB server, provide its URL (for example, orientdb.url=remote:localhost/Orienteer).  For details, see [OrientDB manual](http://orientdb.com/docs/last/Concepts.html#database-url).

  `orientdb.url=<URL>`

* Set the name of the default user on the OrientDB server. This name will also be used by guest users. 

  `orientdb.db.username=<user name>` 
* Set password for the default user on the OrientDB server. 
 
 `orientdb.db.password=<user password>`
* Set the name of the user that will perform administrative tasks on the OrientDB server.
   
   `orientdb.db.installator.username=<admin name>` 
*  Set the password of the user that will perform administrative tasks on the OrientDB server.
   
   `orientdb.db.installator.password=<admin password>`

If something missing, Orienteer will use default settings.

**Default settings**

You can check default settings [here](https://github.com/OrienteerDW/Orienteer/blob/master/orienteer-core/src/main/resources/orienteer-default.properties)

```
orienteer.production=false
orientdb.embedded=true
orientdb.url=plocal:Orienteer
orientdb.db.username=reader
orientdb.db.password=reader
orientdb.db.installator.username=admin
orientdb.db.installator.password=admin
orienteer.image.logo=/org/orienteer/core/web/logo.png
orienteer.authenticatelazy=true
```