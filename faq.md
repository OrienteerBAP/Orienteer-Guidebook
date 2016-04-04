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

**Q: What do you call a document? 

A: A document is an object of a class. 


> и ещё вопрос, можно ли настраивать видимость (доступ) к объектам, основываясь на значениях филдов например, есть роль "контролёр" и она может видеть только объекты в статусе "На контроле"

Есть 2 варианта это сделать:
1) Использование типа документа (класса) OTriggered для того чтобы
"реагировать" на onAfterRead: проверять значение и возвращать null
2) С помощью java можно написать реализацию ORecordHook, которая бы и
проверяла бы все что надо. Этот подход с точки зрения
производительности более правильный.

> ещё интересует штука с оповещениями
> например, "при определенных значениях полей сделай то-то"

Есть - использование того же OTriggered: на событие onBeforeUpdate

> и есть ли такие вычислимые поля, которые позволят сделать такую штуку: задается пороговое значение и постоянно сравнивается с фактическим, при достижении некоторой дельты -- алярм, или объект раскрасить, или нотифай послать

Не очен понял разницу с предыдущим вопросом. При записи можно
вычислить все что надо и послать аларм.

> ещё вопрос по производительности, на каком количестве объектов и классов начинает ощутимо тормозить? (отклик больше 500мс)

Отклик сильно зависит от самого железа и доступной памяти. Если памяти
не хватает (меньше 512 мегабайт) то даже на небольших объемах могут
быть лаги.
В видео видны проблемы с перформансом при изменении схемы. Это
подтвержденный баг в OrientdB и связан он с тем, что на любое
изменение схемы он вызывает flash для всей операционной памяти. А у
меня там памяти 128 Gb. Баг уже исправили, но он не в стейбл ветке.

> у меня есть такие параметры одного инстанса систмеы пользователи: ~30 лицензии: от 1_000 до 100_000 соискатели\лицензиаты: от 1_000 до 100_000 лицензионные дела: от 1_000 до 100_000 шаблоны документов: ~30 неструктурированные документы: (кол-во шаблонов)*(кол-во лицензий) от 10_000 до 1_000_000

Есть ли предполагаемая дата модель? Пока что числа не сильно большие,
но хотелось бы понять все в совокупности.


