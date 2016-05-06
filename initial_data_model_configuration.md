# Initial Data Model Configuration


You implement you data model by creating classes and setting their properties. You can work with classes on the **Schema** page ([..]/schema), on the **Classes** tab.
*  Orienteer supports inheritance between classes, so, a class may have a parent class.
*  Orienteer is a graph + document type of database, so, properties of a class may contain links (references to other documents).

To create a class, click ![+ Create](Create.png). 
To configure a class, go to its page by clicking its name (URL [..]/class/&lt;class name&gt;). 

##Class Configuration

On the **Configuration** tab you can set class parameters. 


* **Name** is the class name that will show on the **Schema** page. When giving a name to a class, follow the [Schema naming convention](https://github.com/OrienteerDW/Orienteer/wiki/Schema-naming-convention).
* **Short Name** is a short alias for the class name used in SQL to simplify wording.
* **Description** is a description of the class.
* **Super Classes** sets the class's parent class.
* **Over Size** is ...
* **Strict Mode**, checking this box will prevent documents of this class having extra properties not defined for the class.
* **Abstract**, ckecking this box makes the class abstract. This prevents the creation on documents of this class. Abstract classes are used only as parents to other classes.
* **Java Class** is the name of the original java class from which this class was generated. For manually created classes, its value is null. 
* **Cluster Selection** defines the [strategy for cluster selection](http://orientdb.com/docs/last/Cluster-Selection.html).
* **Document Name Property** sets the parameter of the class, the value of which will show as a document's name in the list of documents.
* **Parent Document Property** sets the name of a property which refers to logical parent of an instance of this class. Parent hierarchy allows for easier navigation through you data.
* **Default Tab** sets the tab that will show by default when you open a document.
* **Default Sorting** defines property used by default for sorting.
* **Default Sort Order** defines the default sorting order.

##Class Properties

When you create or edit a property, the **property** page opens.
On the **Configuration** tab of a property page, you can set the following:
* **Name** and **Description** are what it says.
* **Tab**:  if you give a name for a tab here, the property will show on a separate tab.
* **Order** sets the order in which this property shows: after other properties with smaller **Order** value and before the rest.
* **Type** sets the data type of the property (for the list of available data types see [OrientDB manual](http://orientdb.com/docs/last/Types.html)).
* **Visualization** defines way the property value is visualized (for the list of available visualisation types, see [supplementary](https://orienteer.gitbooks.io/orienteer/content/supplementary_supported_visualisation_types.html)).
* **Linked Class** lets you connect the class with another class.
* **Inverse** sets inverse property for linkage properties.
* **Mandatory** makes this property mandatory for creating a document.
* **ReadOnly** makes this property read-only in UI on the API level.
* **UI ReadOnly** makes this property read-only in UI.
* **Not Null** sets that value of this property can't be null.
* **Min** and **Max** defines the limits for quantifiable properties.
* **Regexp** sets a pattern for value of this property.
* **Collate** defines collate strategy. Commonly it's default or 'ci' (case insensitive).
* **Displayable** says if a property will be displayed in the list of documents of this class.
* **Hidden** makes this property hidden in UI.
* **Calculable** for making [calculable properties](https://orienteer.gitbooks.io/orienteer/content/adding_calculable_properties.html) (may require experience in coding).
* **Default Value** sets the default value of the property.

You can edit some of these parameters right in the list of class's properties by clicking **Edit**.
On the **Localization** tab on a property page, you can ...

##Class Indexes

With this widget, you can ...
Indexes http://orientdb.com/docs/last/Indexes.html

##Class Custom properties

With this widget, you can set particular custom properties to the whole class.