 # Setting Security

Orienteer approach to security is based on [OrientDB security settings](http://orientdb.com/docs/2.1/Database-Security.html) and supports security on several levels.

## Class level security

At the level of each class, you can define which roles can do what. For this, [go to the page of a  class](https://orienteer.gitbooks.io/orienteer/content/managing_classes.html), the **Security** tab.

![Setting user rights for roles to manage a class](Security.png)

## Roles security rules

You can define security at the level of roles. For this, [go to the page of a role](https://orienteer.gitbooks.io/orienteer/content/managing_users.html), the **Security** tab, and define specific security rules for the role. To read more about making rules, see [OrientDB guide](http://orientdb.com/docs/2.1/Database-Security.html#working-with-roles).

## Document based security

If a document is an instance of a class, which extends the ORestricted class, you can define security on the document-by-document basis. For example, you can make a document visible for just one particular user.

Details here: http://orientdb.com/docs/2.1/Database-Security.html#record-level-security

 