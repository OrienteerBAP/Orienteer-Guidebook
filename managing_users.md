# Managing Users and their Access

##Managing perspectives

A perspective is the part of the database a user can view. It defines the list of sections on the Navigation pane. A list of available perspectives is defined for each user role. To view the **Perspectives** page, on the navigation pane, click **Perspectives**.
For each perspective, you can add properties, each defining a new section on the navigation pane. Properties have following attributes:
* **Name**
* **Perspective item**
* **Perspective** is a list of perspectives in which a section will show on the navigation pane. You can copy properties between perspectives; for this enter the property editing page and add perspectives to this attribute.
* **Icon** ...
* **Url** sets the page that will show when you click the section on a navigation pane.


##Managing roles

A role determines what operations a user can perform against a resource.
To view the **Roles** page, on the navigation pane, click **Roles**. When you create a role, you can make it inherit from another role.

To edit all properties of a role, click its name. You will see a page of a particular role. 

On the **Properties** tab:
* The role's **Name** 
* **Inherited Role** sets the parent role from which the role will inherit its parameters.
* **Rules** and **Mode** regulate rules that apply to a role and how those rules work. 
* **Perspective** defines which perspective will be available for users with this role.
For more details, see [**Security** section of the OrientDB manual](http://orientdb.com/docs/last/Studio-Security.html).

##Managing users

Users are particular persons that you permit to work with the database. To view **Users** page, on the navigation pane, click **Users**.
For each user, you can set a name, a password, assign one or many roles, change status.

