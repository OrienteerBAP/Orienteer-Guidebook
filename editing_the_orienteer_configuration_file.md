# Editing the Orienteer Configuration File

orienteer.properties is the main file to store initial configuration paramenters for your installation. 

There is an example: https://github.com/OrienteerDW/Orienteer/blob/master/orienteer.properties but in any case: if something missing Orienteer will use default settings

Sample properties file can be always found here.

* *orienteer.production=[true|false]* //Run Orienteer in the production mode (true) or in the development mode (false).
* *orientdb.embedded=[true|false]* //Run an embedded OrientDB server (true) or an external OrientDB server (false).
* *orientdb.url=remote:localhost/Orienteer* //If you are runneing an external OrientDB server, provide its network access parameters. For details of setting , see [OrienDB manual](http://orientdb.com/docs/last/Concepts.html#database-url).
* *orientdb.db.username=reader* //Default OrientDB user (will be used for guests as well)

orientdb.db.password=reader               //Password for default OrientDB user

orientdb.db.installator.username=admin    //OrientDB user to user for administrative stuff

orientdb.db.installator.password=admin    //Password for OrientDB user used for administrative stuff

** Optional properties**

orientdb.rest.url=http://localhost:2480

plantuml.url=http://custom-plantuml-url

plantuml.showuml=false;

webjars.readFromCacheTimeout=5 seconds

webjars.useCdnResources=true

webjars.cdnUrl=//maxcdn.bootstrapcdn.com:80
