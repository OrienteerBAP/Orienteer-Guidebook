# Supplementary. Predefined Classes

**Predefined classes arriving from OrientDB**

* OFunction, хранимые функции

* OIdentity, a parent class for OUser, ORole classes.

* ORIDs, an utitily class.

* ORestricted, a class which you can use for configuring access rights of separate documents (for more [see the Security section](https://orienteer.gitbooks.io/orienteer/content/security.html)).

* ORole, roles.

* OSchedule - планировщик задач - возможность запланировать ту или иную
функцию по расписанию

* OTriggered, deriving your class from this class lets your class's objects have dynamic parameters that define dynamic functions, which are called at reading or writing a document. You can check for more details of using triggrs (hooks) [in OrientDB guide](http://orientdb.com/docs/last/Dynamic-Hooks.html).

* OUser, users.

**Predefined classes specific for Orienteer**

* ODashboard stores dashboards configurations.
 
* OLocalization stores localized properties of classes.

* OModule stores a list of modules registered in the OS.

* OPage - возможность иметь динамически страницы - легковесное CMS

* OPerspective - перспективы зарегестрированные в системе

* OPerspectiveItem - меню под перспективы

* OWidget - конфигурация виджетов на дешбордах