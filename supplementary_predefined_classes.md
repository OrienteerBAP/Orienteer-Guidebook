# Supplementary. Predefined Classes

**Predefined classes arriving from OrientDB**

* OFunction: a parent class for deriving functions.

* OIdentity: a parent class for OUser, ORole classes.

* ORIDs: a utitily class.

* ORestricted: a class which you can use for configuring access rights of separate documents (for more [see the Security section](https://orienteer.gitbooks.io/orienteer/content/managing_users.html).

* ORole: user roles.

* OSchedule: a task sceduler. Allows you to created scheduled tasks.

* OTriggered: a parent class for deriving classes of documents that call dynamic functions at read-write operations. This allows you to implement security at document level. For more details on using triggers (hooks), see the [OrientDB guide](http://orientdb.com/docs/last/Dynamic-Hooks.html).

* OUser, users.

**Predefined classes specific for Orienteer**

* ODashboard stores dashboards configurations.
 
* OLocalization stores localized properties of classes.

* OModule stores a list of modules registered in Orienteer.

* OPage - возможность иметь динамически страницы - легковесное CMS

* OPerspective stores perspectives.

* OPerspectiveItem - меню под перспективы

* OWidget stores configurations of widgets on dashboards.