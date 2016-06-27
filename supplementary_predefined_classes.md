# Supplementary. Predefined Classes

**Predefined classes arriving from OrientDB**

* OFunction: functions.
* OIdentity: a parent class for OUser, ORole classes.
* ORestricted: a class which you can use for configuring access rights of separate documents (for more [see the Security section](https://orienteer.gitbooks.io/orienteer/content/managing_users.html).
* ORIDs: a utitily class.
* ORole: user roles.
* OSchedule: a task sceduler. Allows you to created scheduled tasks.
* OTriggered: a parent class for deriving classes of documents that call dynamic functions at read-write operations. This allows you to implement security at document level. For more details on using triggers (hooks), see the [OrientDB guide](http://orientdb.com/docs/last/Dynamic-Hooks.html).
* OUser: users.

**Predefined classes specific for Orienteer**

* ODashboard: dashboards and their configurations.
* OLocalization: localized properties of classes.
* OModule: modules.
* OPage: dynamic pages.
* OPerspective: perspectives.
* OPerspectiveItem: links on a menu (on the left of the screen) in perspectives.
* OWidget: widgets.