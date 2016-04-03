# Supplementary. Predefined Classes

**Predefined classes arriving from OrientDB**

* OFunction, хранимые функции

* OIdentity, a parent class for OUser, ORole classes.

* ORIDs, an utitily class.

* ORestricted, a class which you can use for configuring access rights of separate documents (for more [see the Security section](https://orienteer.gitbooks.io/orienteer/content/security.html)).

* ORole, roles.

* OSchedule - планировщик задач - возможность запланировать ту или иную
функцию по расписанию

* OTriggered, deriving your class from this class lets your class's objects 
у объетов могут быть динамически параметры которые определяеют какие
динамические функции вызывать при чтении, при записи и т.д. 
Подробнее тут: http://orientdb.com/docs/last/Dynamic-Hooks.html

* OUser, users.

**Predefined classes specific for Orienteer**

* ODashboard - класс для хранения конфигурации дешбордов
 
* OLocalization - класс для хранения локализации - перевода на разные языки

* OModule - список модулей зарегистрированных в системе

* OPage - возможность иметь динамически страницы - легковестное CMS

* OPerspective - перспективы зарегестрированные в системе

* OPerspectiveItem - меню под перспективы

* OWidget - конфигурация виджетов на дешбордах