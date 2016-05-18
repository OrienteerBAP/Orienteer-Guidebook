# Adding Custom Pages

You can add custom pages to your app. Pages may display dynamically generated data from the database and call functions. For example, you can make a page to print a document.

To add a custom page, create a document of the class OPage. The document parameters are the following:
* **Name**.
* **Path** is the path to access the page that will be added to the root path of your web app. As parts of the path, you may add a document's record ID as */${rid}*.
* **Description**.
* **Content** is the HTML code of the page (including CSS and JavaScript). With an Orienteer wicket, you can call properties of the object that you have specified in the path by the */${rid}* record.
* **Script** is a JavaScript run by the server.
* **Embedded**:
  * yes: displays the page as a widget.
  * no: displays the page as a separate web page.
* **Document** is the link to the default document used by the wicket when */${rid}* is lacking.
