# Adding Custom Pages

You can add custom pages to your app. Pages may display dynamically generated data from the database and call functions. For example, you can make a page to print a document.

To add a custom page, create a document of the class OPage. The document parameters are the following:
* **Name**.
* **Path** is the path to access the page that will be added to the root path of your web app. As parts of the path, you may add a document's record ID as */${rid}*.
* **Description**.
* **Content** is the HTML code of the page (including CSS and JavaScript). 
  
  With a *wicket:property* wicket, you can call properties of objects that are linked (one or many links) to the object that you have specified in the path by the */${rid}* record. The wicket has the following syntax:
  
  > wicket:property wicket:id="<attribute>" object="<link>", 
  
  where *link* is the path to the target object and *attribute* is its target attribute. For example:
  > wicket:property wicket:id="name" object="first.second.third"
   
  works if the current object (/${rid}) has the link property "first" to another object having the link property "second" to yet another object having the link property "third". The wicket will return the name of the object *third*, 
  
* **Script** is a JavaScript run by the server.
* **Embedded**:
  * yes: displays the page as a widget.
  * no: displays the page as a separate web page.
* **Document** is the link to the default document used by the wicket when */${rid}* is lacking.