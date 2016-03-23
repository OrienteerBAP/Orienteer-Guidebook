# Editing the Orienteer Configuration File

*orienteer.properties* is the main file to store initial configuration paramenters for your installation. You can download a sample configuration file [link](https://github.com/OrienteerDW/Orienteer/blob/master/orienteer.propertie).

**Obligatory properties**
* >orienteer.production=[true|false]

  Run Orienteer in the production mode (true) or in the development mode (false).
* >orientdb.embedded=[true|false]

  Run an embedded OrientDB server (true) or an external OrientDB server (false).
* >orientdb.url=remote:localhost/Orienteer

  If you are runneing an external OrientDB server, provide its network access parameters. For details of setting , see [OrientDB manual](http://orientdb.com/docs/last/Concepts.html#database-url).
* >orientdb.db.username=reader

  Set the name of the default user on the OrientDB server (it will be used for guests as well).
* >orientdb.db.password=reader

  Set password for the default user on the OrientDB server.
* >orientdb.db.installator.username=admin

  Set the name of the user that will perform administrative stuff on the OrientDB server.
* >orientdb.db.installator.password=admin

  Set the password of the user that will perform administrative stuff on the OrientDB server.

If something missing, Orienteer will use default settings.