# Security

What should we put here?

Orienteer supports different levels of security configuration.
Details from OrientDB: http://orientdb.com/docs/2.1/Database-Security.html

## Class level security

Go to required OClass in schema. Navigate to Security tab. Here you can difine who can read, can write or delete instancies of this class by role basis.

## Roles security rules

Go to role you want to manage. NAvigate to Security tab. Here you can difine specific security rules for the role. 

## Document based security

Details here: http://orientdb.com/docs/2.1/Database-Security.html#record-level-security

But simply saying: if a class extends ORestricted - security can be defined on document by document basis.  For example it's possible to make document visible just for 1 user. 