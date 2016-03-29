# Setting Security

Orienteer approach to security is based on [OrientDB security settings](http://orientdb.com/docs/2.1/Database-Security.html) and supports security on several levels.

## Class level security

At the level of each class, you can define which roles can do what. For this, on the class page, select the **Security** tab

![Setting user rights for roles to manage a class](Security.png)
Go to required OClass in schema. Navigate to Security tab. Here you can difine who can read, can write or delete instancies of this class by role basis.

## Roles security rules

Go to role you want to manage. NAvigate to Security tab. Here you can difine specific security rules for the role. 

## Document based security

Details here: http://orientdb.com/docs/2.1/Database-Security.html#record-level-security

But simply saying: if a class extends ORestricted - security can be defined on document by document basis.  For example it's possible to make document visible just for 1 user. 