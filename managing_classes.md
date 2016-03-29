# Managing Classes

You can implement you data model by creating classes and setting their properties on the **Schema** page, on the **Classes** tab.
*  Orienteer supports inheritance between classes, so, a class may have a parent class. 
*  Orienteer is a graph+document database, so, properties of a class may contain references to other documents.

When you can create or edit a class, you see this class's page. On the **Configuration** tab you can set class parameters. 
##The Configuration widget

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

##The Properties widget

When you create or edit a property, the **property** page opens.
On the **Configuration** tab on a property page, you can set the following:
* **Name** and **Description** are what it says.
* Determining how the property values show when you view a document:
  * **Tab**:  if you give a name for a tab here, the property will show on a separate tab.
  * **Order** sets the order in which this property shows: after other properties with smaller **Order** value and before the rest.
* **Type** and **Visualization** set the data type of the property and the way it is displayed. For a list of data types see [OrientDB manual](http://orientdb.com/docs/last/Types.html).
* **Linked Class** lets you connect the class with another class.
* **Inverse** ...
* **Mandatory** makes this property mandatory for creating a document.
* **ReadOnly** ...
* **UI ReadOnly** ...
* **Not Null**...
* **Min** and **Max** for quantifiable properties.
* **Regexp**...
* **Collate**...
* **Displayable**...
* **Hidden** ...
* **Calculable**: put a script here to make the property calculable. Write a script in OrientDB format. Examples:
>select sum(a, b) as value from MyClass where @rid = ?
>select sum(e.salary) as value from Employee e where e.department = ? 

  In case of calculation just for a current row you can use short notation:

  > sum(a, b)

  instead of

  > select sum(a, b) as value from MyClass where @rid = ?

* **Default Value** sets the default value of the property.

You can edit some of these parameters right in the list of class's properties by clicking **Edit**.
On the **Localization** tab on a property page, you can ...

##The Indexes widget

On the Indexes widget, you can ...
Indexies http://orientdb.com/docs/last/Indexes.html

##The Custom properties widget
Whatever