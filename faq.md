# FAQ - Frequently Asked Questions

##About Orienteer

**Q: What is Orienteer? Is it just another data warehouse?**

A: Orienteer is a framework for developing any kinds of applied data warehouses:
* a data warehouse
* a CRM/ERP/BPM solution
* a backend App Platform
* a framework for building web applications 
* a business intelligence tool
* and many others.

**Q: Will Orienteer be always free?**

A: Yes, Orienteer platform will always be free. Our monetization is in:
* building specialized data marts
* customizing solutions
* support

## Data model, configurations etc
**Q: What do you call a document? **

A: A document is an object of a class. 

**Q: Сan I attach an arbitrary file to a document?**

A: Yes. In the class of the document, you need to specify a parameter of type BINARY. You will then be able to attach a file as this parameter to a document. This file will be downloadable from the document.

If this file will be a picture, you can show its thumbnail in the document. For this, in the BINARY parameter's settings specify its visualization: Image.

**Q: Can I implement actions that will work when a document fits to some criteria? For instance, when some property of a document takes a value within some range?**

A: Yes. For this, you will use hooks (triggers), by deriving from the OTriggered class. They may trigger  any automatic actions, from screen notifications or emails to making outomatic records to a log. For details, [see OrientDB guide](http://orientdb.com/docs/last/Dynamic-Hooks.html).

**Q: Similarly, can Orienteer do specific actions on coincidences of data from many properties of many documents? For example, identifying statistical outlyers.**

A: Yes. Similarly, this will require using hooks (triggers) by deriving from the OTriggered class. For details, [see OrientDB guide](http://orientdb.com/docs/last/Dynamic-Hooks.html).

##Users and User Rights

**Q: Can I make rights of users to read / write documents dependent on values of particular properties? E.g. I would like to make documents marked *for audit* visible for the *Auditor* role**

A: Yes. There are two main ways for that:

* If a class extends the *OTriggered* class, you can set it to call the event *onAfterRead* that will check user rights. For details, see [OrientDB guide](http://orientdb.com/docs/last/Dynamic-Hooks.html).
* For providing higher performance, you can implement a java hook with the *ORecordHook* interface, which would check credentials of the user that works with data. For details, see [OrientDB guide](http://orientdb.com/docs/last/Java-Hooks.html).

**Q: How can I add company departments as groups of users to manage them in joint? **

A: It's recommended to use Orienteer roles for modeling company departments. There are few reasons:

1) Person can be within multiple departments: roles do allow that.
2) According to department person is assigned to he can has different rights. Roles do allow to define that

**Q: Сan we establish the common password workflow, when userы can change their passwords themselves? Is there a way for a user for password recovery without involving the admin?**

A: ...

**Q: How can the administrator get user passwords?**

A: ...

##Integrity and Data Control

**Q: What happens if I change parameters of a property so that the existing property values are no more valid?**

A: ... [obligatory correction at next document edit]

**Q: Can I change the type of a property? Are there any limitations?**
 
 A:  You can select any property type during creation, but there are some limitations if you want to change a type of existing property. You can't change type to incompatible/nonconvertible type. For example, it's not possible to change type from STRING to INTEGER just because some values can't be converted.
 
 
 **Q: What happens to documents when I delete their class?**
 
 Unfortunately, you will lost your data.
 
 ##Logging
 
**Q: How can data changes be logged?**

A: See http://orientdb.com/docs/last/Auditing.html

**Q: How can I delete a class but leave its documents in the database for auditing and history logs? Can I hide it and prevent it from being used?**
 
...

##Performance

**Q: What are performance limitations or Orienteer?**

A: This depends on the hardware.
[add testing]




