# Managing Users and their Access

##Managing perspectives

A perspective defines what page a user sees after logging in and what pages are available for him or her on the navigation pane. Each user role has a [set of available perspectives](https://orienteer.gitbooks.io/orienteer/content/orienteer_user_interface.html) to select from.

> **Warning!** If users don't see a page in their perspective, this doesn't prevent them from accessing a page over its URL. To restrict the access, check that [database security settings](https://orienteer.gitbooks.io/orienteer/content/security.html) are configured properly.

To configure perspectives, on the navigation pane, click **Perspectives** (URL: *&lt;databaseURL&gt; /browse/OPerspective*).

For each perspective, you can add sections to the navigation pane. Sections have following attributes:
* **Perspective item**
* **Name** is the name of the section that will show on the navigation pane.
* **Perspective** is a list of perspectives in which the section will show on the navigation pane.
* **Icon** is the 
* **Url** sets the page that will show when you click the section.
* **Sub items** ...

##Managing roles

The **Roles** page URL: */browse/ORole*.

A role determines what operations a user can perform against a resource. When you create a role, you can make it inherit from another role. To edit all properties of a role, click its name. 

On the **Properties** tab:
* The role's **Name** 
* **Inherited Role** sets the parent role from which the role will inherit its parameters.
* **Rules** and **Mode** regulate rules that apply to a role and how those rules work. 
* **Perspective** defines which perspective will be available for users with this role.
For more details, see [**Security** section of the OrientDB manual](http://orientdb.com/docs/last/Studio-Security.html).

##Managing users

The **Users** page URL: */browse/OUser*.

Users are particular persons that you permit to work with the database. For each user, you can set a name, a password, assign one or many roles, change status.

