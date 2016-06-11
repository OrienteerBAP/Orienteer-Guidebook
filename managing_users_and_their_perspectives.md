# Managing Users and their Perspectives

In this section, we go through managing perspectives and creating users.

A perspective is the user work space that displays only those sections of the data base that this kind of user needs. Perspectives are assigned to roles.

##Creating a Perspective

The users who will use our CRM app and work with clients, need only several sections of the data base. They do not need the tools for creating classes, managing users etc. So, we will create a perspective for them that will show only their part of work.

On the menu on the left, click **Perspectives**, create a perspective with parameters:
   * Name: click **Add**. In the drop box, type *en* (localizaiton). On the right, type *Account manager*.
   * Home URL: /browse/CmsContact. This is the relative URL of the list of contacts, the page that we want this user to see after the logon.

To check the new perspective, select it with the icon on the top right: ![](UI-selecting-perspectives.jpg).

##Creating a User role and a User
On the menu on the left, click **Roles**. Create a role with parameters:
* Name: Account manager
* Perspective: Account manager

On the menu on the left, click **Users**. Create a user with parameters:
* Name: Jane
* Status: Account manager
* Perspective: Account manager
* Password: qwerty

Now when Jane logs in, she will see her default perspective.

>Warning! 
Security
Availability 
