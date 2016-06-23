# HTML and JavaScript Widgets

You can add custom HTML / JS widgets to pages. For this add the  *Browse Html Js Pane* widget (steps 1, 2), and on the top right, click **Save** (step 3):

![](adding-a-html-js-widget.png)

After that, on the new widget, click, **Actions > Settings**. On the *widget properties* page, you can edit the widget. 

Disambiguation of properties specific to this widget:

* **Html** and  **Script** add an HTML code and a script to the widget.
* **Resources** ...

Example: you can add a widget with a google map by setting the following HTML code:
`<div>  <iframe width="100%" height="600" frameborder="0" style="border:0" src="https://www.google.com/maps/embed/v1/place?key=AIzaSyC1vj2XnFZv0CpiuOVoJsGl0ZhDtM6rv5c&q=${postalAddress.region} ${postalAddress.city} ${postalAddress.street} ${postalAddress.streetNumber}" allowfullscreen> </iframe>  </div>`