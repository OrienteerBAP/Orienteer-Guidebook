# Creating Your First Business Application

It's time to create your business application. Assuming that you know what you want to have finally, this chapter will walk you through Orienteer basics configuration techniques. You will learn how to manage data model, create new users, configure dashboards, manage security and make many other operations with your app.

> Note. This chapter shows configurations in the default Orienteer perspective.

## Building The Data Model
We will build a simple data model and augment it in a step-by-step manner. 
We will build a basic CRM app that will store client names, contacts and the type of their interaction with the company (interested, purchase, support). We will go through minimal steps to have a viable app.

### Creating a Class
We will start with the simplest model, with only one class, *Customer*. It will have properties *Customer name*, *Contacts* and *Interaction*.

1. Go to page */schema*.
2. To create a new class, сlick **Create**.
3. On the class page, fill the parameter Name: *Customer*, then click **Save**.
4. On the widget **Properties** create three properties by clicking **Create**. Set their  parameters and click **Save**. 
  * For the *Customer name* property, set the parameters:
    * Name: Customer_name
    * Type: String
  * For the *Contact* property, set the parameters:
    * Name: Contact
    * Type: String
  * For the *Interaction* property, set the parameters:
    * Name: Customer_name
    * Type: String

Now we can create documents of the class Customer. Each document will correspond to a person.

Once we want to add a new customer or to edit an existing one, we will need to go to the list of class's documents.
1. Go to /browse/Customer (otherwise, you could go to /schema and in the line Customer, on the right, click **Browse Class**).
2. To create a new document, click **Create**.
3. Now you can fill new client's data and save it.

###

### Links

  * Creating classes, properties
  * Link type properties.
  * UML
  * Creating documents.
## Managing Users
## Configuring the UI
  * Dashboards, tabs
  * Setting perspectives

## Data Visualisation
Pivot table, other custom and configurable widgets.
## Localization

