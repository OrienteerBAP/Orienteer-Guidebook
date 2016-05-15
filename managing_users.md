# Security and User Access Management

##Role-based Security

For each user, you can set a password and assign one or many roles (the **Users** page URL: */browse/OUser*).

A role determines what operations a user can perform against a resource. When you create a role, you can make it inherit from another role. You can manage roles on the **Roles** page (URL: */browse/ORole*). 

On the **Properties** tab of a role, you can set the following:
* The role's **Name**.
* **Inherited Role** sets the parent role from which the role will inherit its parameters.
* **Rules** and **Mode** regulate rules that apply to a role and how those rules work. 
* **Perspective** defines which perspective will be available for users with this role.
For more details, see [**Security** section of the OrientDB manual](http://orientdb.com/docs/last/Studio-Security.html).

##Document-level Security

By using triggers, 