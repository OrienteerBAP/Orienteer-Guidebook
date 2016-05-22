# HTML and JavaScript Widgets

You can add a custom HTML / JS widgets to pages. For this, add the  *Browse Html Js Pane* widget, and on the top right, click **Save**.

![](adding-a-html-js-widget.png)

After that, on the new widget, click, **Actions > Settings**. On the widget properties page, you can edit the widget.

* **Title**.
* **Html** and  **Script** add the HTML code and a script to the widget.
* **Dashboard** ...
* **Type id** ...
* **Resources** ...
* **Col** ...
* **Row** ...
* **Size X** and **Size Y** set the size of the widget.
* **Hidden** ...

Example: you can add a widget with a google map by setting the following HTML cole:

> &lt;div&gt;  &lt;iframe width="100%" height="600" frameborder="0" style="border:0" src="https://www.google.com/maps/embed/v1/place?key=AIzaSyC1vj2XnFZv0CpiuOVoJsGl0ZhDtM6rv5c&q=${postalAddress.region} ${postalAddress.city} ${postalAddress.street} ${postalAddress.streetNumber}" allowfullscreen&gt; &lt;/iframe&gt;  &lt;/div&gt;
