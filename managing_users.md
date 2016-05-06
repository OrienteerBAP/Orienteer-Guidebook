# Managing Users and User Roles

##Managing user roles

The **Roles** page URL: */browse/ORole*.

A role determines what operations a user can perform against a resource. When you create a role, you can make it inherit from another role. To edit all properties of a role, click its name. 

On the **Properties** tab, you can set the following:
* The role's **Name**.
* **Inherited Role** sets the parent role from which the role will inherit its parameters.
* **Rules** and **Mode** regulate rules that apply to a role and how those rules work. 
* **Perspective** defines which perspective will be available for users with this role.
For more details, see [**Security** section of the OrientDB manual](http://orientdb.com/docs/last/Studio-Security.html).

##Managing users

The **Users** page URL: */browse/OUser*.

Users are particular persons that you permit to work with the database. For each user, you can set a name, a password, assign one or many roles, change status.