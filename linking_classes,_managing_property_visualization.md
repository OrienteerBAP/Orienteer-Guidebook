# Linking Classes, Managing Property Visualization

---
This part will guide you through linking classes in Orienteer. You will also learn how to display properties on separate tabs and how to enable basic UI controls to manage properties of a document.

---

In the app we've just created, we store all contacts in a single plaintext field for skype, telephones, emails etc in bulk. Now we want each customer to have several separate contact records, each containing one contact. We also  want contacts of each customer to show on a separate tab.

Do the following:
1. From the class *CmsCustomer*, delete the property *contact*. We will store contacts in a different way. 
2. Create a new class for storing contacts, *CmsContact*

  We want each customer's contact to be stored as a separate item. This is why we will create a separate class for contacts. We will be able to add as many documents of this class as needed to each customer.
  
3. Link the *CmsContact* and the *CmsCustomer* classes. For this, add special LINK properties to both classes:
  *  To the *CmsCustomer* class, add a property *linkToContacts* with parameters `Type: LINKLIST`. `Linked Class: CmsContact`.
  *  To the *CmsContact* class we add a property *Customer* with parameters:
    *  `Type: LINK`.
    *   `Linked Class: CmsCustomer`.
    *   `Visualization: listbox` (this will let the app user select a linked customer for a contact from a drop box).
    *  `Inverse: linkToContacts` (here you choose a back link from the list of link type parameters of the linked class, *CmsCustomer*).
  *  Go back to the *CmsCustomer* class and edit the parameter *linkToContact*. Set its parameter *Inverse* similarly, by selecting the property *Customer*.

4. We want each customer's contacts to show on a separate tab. For this, in the class *CmsCustomer* edit the link property *linkToContacts*. Set the following parameters:
  * `Tab: Contacts`. Now a separate tab named *Contacts* will show the list of contacts linked to the particular customer.
  * `Visualization: table`. This enables UI elements like **Create** or **Save** buttons etc, that will be handy for creating and managing contacts.

5. In the previous step, we have changed the visualization of a property. Whenever we will look through the list of customers (the documents of the class *CmsCustomer* on the page /browse/CmsCustomer), this property, with its buttons and other elements, is not useful. We want to hide it from the document list.
   
   To do this, for each property of the class *CmsCustomer* set its parameter **Displayable**. Check it for the properties *customerName* and *interaction* and uncheck it for the property *linkToContacts*.

With this, we are done for this part. Now, when you create a customer, you do not give its contacts, only their name and stage of interaction. To add contacts, you will go to each customer's page and on a separate tab **Contacts** add as many contacts as you need.