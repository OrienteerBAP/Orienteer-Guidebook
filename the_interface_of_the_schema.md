# The Interface of the Schema Page

You can access the Schema page by clicking **Schema** on the navigation page (URL: &lt;databaseURL&gt; /schema)

## The Class tab

On this tab you can view all existing classes in your database and some of their attributes. Some are predefined ([see supplementary](https://orienteer.gitbooks.io/orienteer/content/supplementary_predefined_classes.html)).
Class management buttons:
* **Cleate**, **Delete**  for creating and deleting classes
* **Edit**  for editing the parameters Super Classes, Abstract and Strict mode (the ones you can see in list of classes)
* **Reload**  for re-reading of schema from database
* **Export** for exporting the whole schema to a file 
* **Import** for importing the whole schema from a local file
* **View in UML** for viewing the classes that you select on a UML diagram

To edit properties of a class, click its name.
To view documents belonging to a class, click its **Browse class** button (on the right of the screen).

## The Indexes tab

Lets you configure indexes. The indexing approach follows [that of OrientDB](http://orientdb.com/docs/2.1/Indexes.html).

On this page you can view and configure the following attributes of indexes:
* **Type**, a type of the index according to OrientDB approach.
* **Fields** a list of fields which included into an index.
* **Collate** a rule of comparison: either default of CI (case insensitive)
* **Is null values ignored** flag to mark indexes which should ignore null values during index

## The Database tab

Lets you [configure general database settings](https://orienteer.gitbooks.io/orienteer/content/creating_a_database_and_configuring_its_properties.html).
## The Clusters tab

Lets you work with clusters (as [defined in OrientDB](http://orientdb.com/docs/2.0/orientdb.wiki/Tutorial-Clusters.html)). 
> **Note.** In the current Orienteer vesion, each class corresponds to a single cluser. 
