# Managing Users and their Access

##Managing perspectives

A perspective defines what page a user sees after logging in and what pages are available for him or her on the navigation pane. Each user role has a [set of available perspectives](https://orienteer.gitbooks.io/orienteer/content/orienteer_user_interface.html) to select from.

The **Perspectives** page URL: */browse/OPerspective*.
> **Warning!** If a user doesn't see a page in a set of available perspectives, this doesn't prevent a user from accessing a page over its URL. To restrict the access, check that [database security settings](https://orienteer.gitbooks.io/orienteer/content/security.html) are configured properly.

For each perspective, you can add properties, each defining a new section on the navigation pane. Properties have following attributes:
* **Name**
* **Perspective item**
* **Perspective** is a list of perspectives in which a section will show on the navigation pane. You can copy properties between perspectives; for this enter the property editing page and add perspectives to this attribute.
* **Icon** ...
* **Url** sets the page that will show when you click the section on a navigation pane.
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

