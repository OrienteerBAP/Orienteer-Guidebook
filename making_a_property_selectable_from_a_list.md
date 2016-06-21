# Making a Property Selectable from a List

---
 This part will help you make a property with values selectable from a list.

---

Now we can make several contats for a client. But if we'd like to index them, we will face the fact that the app operators type in the data in a very different style. Just think of how many ways there are to write the work *email*!

So, for each contact, we want the operators to select the contact type (email, skype etc) from a drop box.

For this, we will create yet another class, *CmsContactType*. This class will contain three instances (documents) that will represent the allowed contact types.

1. Create the class *CmsContactType* with just a single STRING type property, *contactTypeName*.
2. In this class, create four documents: 
  * *email* 
  * *skype*
  * *snail mail*
  * *telephone* 
3. In the class *CmsContact*, add a property *ContactType* with following parameters:
  * Type: LINK.
  * Visualization: listbox (this will let the user select the type of contact from a drop box).
  * Linked Class: CmsContactType.

Now you can check any customer's contacts. When you add a new contact or edit an existing one, you will have a drop box to select from a pre-defined set of values.

Let's check the new UML:
![](CMS_UML_step_2.png)
