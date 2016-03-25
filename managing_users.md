# Managing Users and their Access

You can manage roles and assign them to particular users.

##Managing roles

A role determines what operations a user can perform against a resource.
To view the **Roles** page, on the navigation pane, click **Roles**. When you create a role, you can make it inherit from another role.

To edit all properties of a role, click its name. You will see a page of a particular role. 

On the **Properties** tab:
* The role's **Name** 
* **Inherited Role** sets the parent role from which the role will inherit its parameters.
* **Rules** and **Mode** regulate rules that apply to a role and how those rules work. 
For more details, see [**Security** section of the OrientDB manual](http://orientdb.com/docs/last/Studio-Security.html).

##Managing users

Users are particular persons that you permit to work with the database. To view **Users** page, on the navigation pane, click **Users**.
For each user, you can set a name, a password, assign one or many roles, change status.

##Managing perspectives

A perspective is a 