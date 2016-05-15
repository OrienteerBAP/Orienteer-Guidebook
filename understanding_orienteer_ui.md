# Understanding Orienteer UI

The Orienteer UI is based on several basic concepts.

## Pages and perspectives
An Orienteer app is displayed as a set of **pages**. Some pages may be universal for all Orienteer apps, like *Users* or *Classes*. Others will be specific to particular apps. Users can access pages by clicking their links (e.g. on the menu) and [via their URLs](https://orienteer.gitbooks.io/orienteer/content/special_urls.html).

A **perspective** defines what pages are available for the user on the menu and what is the default page that a user sees after logging in. 

Example (the default perspective):

![](Perspectives-small1.png)

For each user role, the Orienteer app administrator allocates a set of available perspectives. To select another perspective, click ![](UI-selecting-perspectives.jpg) on the top right.

## Tabs, dashboards and widgets

What the user sees on a page is a **dashboard**. On a dashboard, there can be several **widgets** that display a variety of data. These may be tables, graphs, custom widgets developed for a particular app. Selecting other **tabs** on the page, user will see other widgets.

Example: the default dashboard of a class contains several widgets *Configuration*, *Properties*, *Indexes*, *Custom properties*. The user can also select between tabs: *Configuration*, *Localization*, *Security*, *Subclasses*.

![](Pages&widgets.png)

To add new widgets, re-size and move them around on the dashboard, click  ![](UI-adding-widgets.jpg) on the top right of the dashboard. 

You can add the pre-defined Orienteer widgets only to particular pages. The set of these pages is a wiget's scope.

|Page|URL|Scope in Orienteer 1.1|
| -- | -- | -- |
|ODocumentPage|/doc/&lt;rid&gt;|Schema class of a document|
|BrowseOClassPage|/browse/&lt;class name&gt;|Schema class|
|SchemaPage|/schema or /classes|Global|
|OClassPage|/classes/&lt;class name&gt;|Global|
|OPropertyPage|/property/&lt;class name&gt;/&lt;property name&gt;|Global|
|OIndexPage|/index/&lt;index name&gt;|Global|
