# User Interface Configuration

[Including info about using Orienteer on mobile devices]
Perspectives

##Managing perspectives

A perspective defines what page a user sees after logging in and what pages are available for him or her on the navigation pane. Each user role has a [set of available perspectives](https://orienteer.gitbooks.io/orienteer/content/orienteer_user_interface.html) to select from.

> **Warning!** If users don't see a page in their perspective, this doesn't prevent them from accessing a page over its URL. To restrict the access, check that [database security settings](https://orienteer.gitbooks.io/orienteer/content/security.html) are configured properly.

To configure perspectives, on the navigation pane, click **Perspectives** (URL: *&lt;databaseURL&gt; /browse/OPerspective*).

For each perspective, you can add sections to the navigation pane. Sections have following attributes:
* **Perspective item**
* **Name** is the name of the section that will show on the navigation pane.
* **Perspective** is a list of perspectives in which the section will show on the navigation pane.
* **Icon** is the icon that will show on the navigation pane by the section's name. You can set the icon by ...
* **Url** sets the page that will show when you click the section.
* **Sub items** ...