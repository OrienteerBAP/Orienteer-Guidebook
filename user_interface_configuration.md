# User Interface Configuration

Orienteer provides adaptive UI, making Orienteer apps suitable for mobile devices.

##Configuring Perspectives

The administrator allocates [perspectives available for each user role](https://orienteer.gitbooks.io/orienteer/content/understanding_orienteer_ui.html). To configure perspectives, in the menu on the left, click **Perspectives** (or go to URL */browse/OPerspective*).

For a perspective, you can set:
* **Name**: a localizable name of a perspective.
* **Icon**: the name of an icon to be displayed (pick an icon name from [Font Awesome project](http://fontawesome.io/icons/)).
* **Home Url**: the default page of the perspective.
* **Footer**: a text area for html code that defines a common footer for all pages in a perspective. 

For each perspective, you can add and delete sections to the menu on the left. Sections have following attributes:

* **Perspective item**
* **Name**: the name of the section that will show on the menu.
* **Perspective**: a list of perspectives in which the section is present.
* **Icon**: the icon that will show on the navigation pane along with the section's name. Set it similarly to the icon of the perspective. 
* **Url**: the page that shows when you click the section.
* **Sub items**: subsections of the section.


> **Warning!** If users don't see a page in their perspective, this doesn't prevent them from accessing a page over its URL. To restrict the access, configure the [database security settings](https://orienteer.gitbooks.io/orienteer/content/managing_users.html).