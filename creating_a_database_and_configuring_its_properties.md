# Configuring Database Properties

Commonly there is no need to configure OrientDB database manually, because Orienteer take care of that, but in specific cases you can configure the database on the **Schema** page (URL */schema*), on the **Database** tab. 

###Parameters:

####General settings
* **Type** - type of the database. It's 'graph' by default
* **Status** - status of a database. Should be ACTIVE.
* **Default Cluster Id** - id of a cluster which should be considered by OrientDB as default

####Date, time and location
* **Date Format**, e.g. *yyyy-MM-dd*
* **Date/Time Format**, e.g. *yyyy-MM-dd HH:mm:ss*
* **Timezone** selected from a droplist
* **Locate Country**, e.g. *US*
* **Locale Language**, e.g. *en*


####Other settings

* **Charset** - sets the character encoding.
* **Custom** - some specific custom settings
* **Cluster Selection** - approach for cluster selection
* **Minimum Clusters**
* **Conflict Strategy** - selected strategy of conflicts resolution
* **Validation*** - should validation be enabled