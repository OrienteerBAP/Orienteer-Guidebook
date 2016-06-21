# Creating a Class

---
 This part will guide you through creating a class, setting its properties and creating an instance of the new class (a document) in Orienteer.

---

We will start with the simplest model, with only one class, *Customer*. It will have properties *Customer name*, *Contacts* and *Interaction*.

1. Go to page */schema*.
2. To create a new class, сlick **Create**.
3. On the class page, fill the parameter Name: *CmsCustomer*, then click **Save**.
4. On the widget **Properties** create three properties by clicking **Create**. Set their  parameters and click **Save**. 
  * For the *customerName* property, set the parameters:
    * Name: customerName
    * Type: String
  * For the *contact* property, set the parameters:
    * Name: contact
    * Type: String
  * For the *interaction* property, set the parameters:
    * Name: interaction
    * Type: String

5. Specify which of the parameters will identify a document. In our case each document corresponds to a customer's name. So, in the class *CmsCustomer*, on the widget *Configuration*, set the parameter **Document Name Property**: *customerName*.

Now we can create documents of the class Customer. Each document will correspond to a person.

Once we want to add a new customer or to edit an existing one, we will need to go to the list of class's documents.
1. Go to /browse/Customer (otherwise, you could go to /schema and in the line Customer, on the right, click **Browse Class**).
2. To create a new document, click **Create**.
3. Now you can fill new client's data and save it.

