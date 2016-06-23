# Functions

In Orienteer, you can use custom functions to process data. A Function is an executable unit of code that can take parameters and return a result.

OrientDB Functions features (from [OrientDB manual](http://orientdb.com/docs/last/Functions.html)):

* are persistent.
* can be written in SQL or JavaScript.
* can be executed via SQL, Java, REST and Studio.
* can call each other.
* supports recursion.
* have automatic mapping of parameters by position and name.
* plugins can inject new objects to being used by functions.

To create a function, you need to create a document of the class OFunction. With the **Language** parameter, choose if you use SQL or JavaScript.

You can test your function on a widget **Function executor**.

