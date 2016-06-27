# Create a "Hello World" Widget

1. Create a new java class for your widget. For example `HelloWorldWidget`.    This class should extend `org.orienteer.core.widget.AbstractWidget` or one of its child classes.
3. Create an html file with the same name as your class in the same package. For example `HelloWorldWidget.html`. Fill the file as shown below.
4. Annotate your class with `@Widget` annotation and specify required characteristics of the widget.
5. Ensure that package with your widget is enabled for scanning in a module. It should contain something like this: `registerWidgets("com.mycompany.mypackage");`

Finally you should have something like this:

**HelloWorldWidget.html**

```html
<wicket:extend>
<h1>Hello World!</h1>
</wicket:extend>
```

**HelloWorldWidget.java**

```java
package org.orienteer.examples.component.widget;

import org.apache.wicket.model.IModel;
import org.apache.wicket.model.Model;
import org.orienteer.core.component.FAIcon;
import org.orienteer.core.component.FAIconType;
import org.orienteer.core.widget.AbstractWidget;
import org.orienteer.core.widget.Widget;

import com.orientechnologies.orient.core.record.impl.ODocument;

@Widget(domain="schema", tab="hello", id="hello-world", autoEnable=true)
public class HelloWorldWidget extends AbstractWidget<Void> {

	public HelloWorldWidget(String id, IModel<Void> model, IModel<ODocument> widgetDocumentModel) {
		super(id, model, widgetDocumentModel);
	}

	@Override
	protected FAIcon newIcon(String id) {
		return new FAIcon(id, FAIconType.exclamation);
	}

	@Override
	protected IModel<String> getDefaultTitleModel() {
		return Model.of("Hi!");
	}

}
```

To do more complex things you should be familiar with [Apache Wicket](https://ci.apache.org/projects/wicket/guide/7.x/).