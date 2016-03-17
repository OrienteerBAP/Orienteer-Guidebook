# Editing the Orienteer Configuration File

orienteer.properties is the main file to store initial configuration paramenters for your installation. Sample properties file can be always found here.

*orienteer.production=false*  //Run Orienteer in production mode or not

orientdb.embedded=false     //Run embedded OrientDB server?

orientdb.url=remote:localhost/Orienteer   //OrientDB server URL

orientdb.db.username=reader               //Default OrientDB user (will be used for guests as well)

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
