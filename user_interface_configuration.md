# User Interface Configuration

Orienteer provides adaptive UI, making Orienteer apps available on mobile devices.

##Configuring Perspectives

The administrator allocates perspectives available for each user role.

To configure perspectives, on the navigation pane, click **Perspectives** (URL: *&lt;databaseURL&gt; /browse/OPerspective*).

For a perspective, you can set:
* **Name** - localizable name of a perspective
* **Icon** - name of an icon to be displayed (you can pick any icon name from [Font Awesome project](http://fontawesome.io/icons/))
* **Home Url** - default page of the perspective
* **Footer** - textarea to define html code to be shown on any page footer. 


For each perspective, you can add sections to the navigation pane. Sections have following attributes:

* **Perspective item**
* **Name** is the name of the section that will show on the navigation pane.
* **Perspective**, a list of perspectives in which the section is present.
* **Icon**, the icon that will show on the navigation pane by the section's name. Set it similarly to the icon of the perspective. 
* **Url**, the page that will show when you click the section.
* **Sub items** are the subsections of the secton.


> **Warning!** If users don't see a page in their perspective, this doesn't prevent them from accessing a page over its URL. To restrict the access, configure the [database security settings](https://orienteer.gitbooks.io/orienteer/content/managing_users.html).