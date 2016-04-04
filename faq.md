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
**Q: Сan I attach an arbitrary file to a document?**

A: Yes. In the class of the document, you need to specify a parameter of type BINARY. You will then be able to attach a file as this parameter to a document. This file will be downloadable from the document.

If this file will be a picture, you can show its thumbnail in the document. For this, in the BINARY parameter's settings specify its visualization: Image.

**Q: What do you call a document? **

A: A document is an object of a class. 

**Q: Can I implement actions that will work when a document fits to some criteria? For instance, when some property of a document takes a value within some range?**

A: Yes. For this, you will use hooks (triggers), by deriving from the OTriggered class. They may trigger  any automatic actions, from screen notifications or emails to making outomatic records to a log. For details, [see OrientDB guide](http://orientdb.com/docs/last/Dynamic-Hooks.html).

**Q: Similarly, can Orienteer do specific actions on complicated coincidences of data from many properties of many documents? For example, identifying statistical outlyers.**

A: Yes. Similarly, this will require using hooks (triggers) by deriving from the OTriggered class. For details, [see OrientDB guide](http://orientdb.com/docs/last/Dynamic-Hooks.html).

##Performance

**Q: What are performance limitations or Orienteer?**

A: This depends on the hardware.
> > ещё вопрос по производительности, на каком количестве объектов и классов начинает ощутимо тормозить? (отклик больше 500мс)


> у меня есть такие параметры одного инстанса систмеы пользователи: ~30 лицензии: от 1_000 до 100_000 соискатели\лицензиаты: от 1_000 до 100_000 лицензионные дела: от 1_000 до 100_000 шаблоны документов: ~30 неструктурированные документы: (кол-во шаблонов)*(кол-во лицензий) от 10_000 до 1_000_000

Есть ли предполагаемая дата модель? Пока что числа не сильно большие,
но хотелось бы понять все в совокупности.



> и ещё вопрос, можно ли настраивать видимость (доступ) к объектам, основываясь на значениях филдов например, есть роль "контролёр" и она может видеть только объекты в статусе "На контроле"

Есть 2 варианта это сделать:
1) Использование типа документа (класса) OTriggered для того чтобы
"реагировать" на onAfterRead: проверять значение и возвращать null
2) С помощью java можно написать реализацию ORecordHook, которая бы и
проверяла бы все что надо. Этот подход с точки зрения
производительности более правильный.
