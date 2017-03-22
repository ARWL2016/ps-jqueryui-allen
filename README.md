##JQueryUI (Pluralsight: Scott Allen, 2011)

https://app.pluralsight.com/player?course=jqueryui&author=scott-allen&name=jqueryui-introduction&clip=1 

####Jquery Modules 
- typically, using JQuery UI needs three files:   
- `jquery-ui.css` (default theme)  
- `jquery.js` (core library)  
- `jquery-ui.js` (UI core)  

####Activating JQuery UI Widgets 
- typically, we create an HTML structure and give it the UI class
- in the script, selecting that UI widget gives access to a function which initializes the widget `$( "#accordion" ).accordion();`
- we also have access to various configurations in the script: all widgets have **options**, **events**, and **methods**   

####Theme Rollers 
- Themes can be created or picked at https://jqueryui.com/themeroller/ 
- This will generate a different `jqueryui.css` style file  

####Options 
- the first parameter passed to a widget's function is an options object: `$('dialog').dialog({*options*})`
- details are in the API docs: http://api.jqueryui.com/category/all/ 

####Events 
- all widgets have associated events which are invoked by user interaction
- these can be used to add functionality in the script   
- event are added into the options object

####Methods 
- JQuery inbuilt methods are usually in the format .css(), .toggle(), .fadeOut() etc
- JQuery UI methods are distinct - they are passed as a string to the widget method: `$('dialog').dialog(open)` - e.g. in response to a user action  

