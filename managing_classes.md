# Managing Classes

You can implement you data model by creating classes and setting their properties on the **Schema** page, on the **Classes** tab.
*  Orienteer supports inheritance between classes, so, a class may have a parent class. 
*   Orienteer is a graph+document database, so, properties of a class may contain references to other documents.

You can create or edit a class, you see this class's page. On the **Configuration** tab you can set class parameters. 
##Configuration area

* **Name** is the class name that will show on the **Schema** page. When giving a name to a class, follow the [Schema naming convention](https://github.com/OrienteerDW/Orienteer/wiki/Schema-naming-convention).
* **Short Name** is ...
* **Description** is a whatever description you give to the class.
* **Super Classes** sets the class's parent class.
* **Over Size** is ...
* **Strict Mode** is ...
* **Abstract** makes the class abstract, meaning there can be no instances of it (documents) in the database. Abstract classes can only be parent to other classes.
* **Java Class** is ...
* **Cluster Selection** ...
* **Document Name Property** sets the parameter, the value of which will show as a document's name in the list of documents.
* **Parent Document Property** ... 
* **Default Tab** sets the tab that will show by default when you open a document.
* **Default Sorting** ...
* **Default Sort Order** ...

##Properties

When you create or edit a property, 

Creating and editing properties.

Properties order and other attributes

Configuring properties

Types of parameters: https://github.com/OrienteerDW/Orienteer/wiki/Property-types-support 
http://orientdb.com/docs/last/Types.html
В Orienteer есть еще возможность указать тип визуализации. Типы эти расширяемы. Пока что список вот такой:
https://github.com/OrienteerDW/Orienteer/wiki/Property-types-support


Calculable properties https://github.com/OrienteerDW/Orienteer/wiki/How-to-make-calculable-property


##Indexies

Indexies http://orientdb.com/docs/last/Indexes.html

##Custom properties 