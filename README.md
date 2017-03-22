##JQueryUI (Pluralsight: Scott Allen, 2011)

https://app.pluralsight.com/player?course=jqueryui&author=scott-allen&name=jqueryui-introduction&clip=1 

####Jquery Modules 
- typically, using JQuery UI needs three files:   
- `jquery-ui.css` (default theme)  
- `jquery.js` (core library)  
- `jquery-ui.js` (UI core)  

####Activating JQuery UI Widgets 
- typically, we create an HTML div and give it a specific UI widget id: `<div id="slider"></div>`
- in the script, selecting that UI widget gives access to a function which initializes the widget `$("#slider").slider();`
- we also have access to various configurations in the script: all widgets have **options**, **events**, and **methods**. These are set as parameters to the initialization function 

####Theme Rollers 
- Themes can be created or picked at https://jqueryui.com/themeroller/ 
- This will generate a different `jqueryui.css` style file  

####Options 
- the first parameter passed to a widget's function is an options object: `$('dialog').dialog({*options*})`
- details are in the API docs: http://api.jqueryui.com/category/all/  
- options are used for initialisation of a widget  

####Events 
- all widgets have associated events which are invoked by user interaction  
- these can be used in the script to add functionality    
- events are also added into the options object 
- events generally have two parameters - `event` and `ui`. The event parameter contains DOM information. The ui parameter contains information about the widget  

####Methods 
- JQuery inbuilt methods are usually in the format .css(), .toggle(), .fadeOut() etc
- JQuery UI methods are distinct - they are passed as a string to the widget method: `$('dialog').dialog(open)` - e.g. in response to a user action  
- methods are applied separately after initialization   
- methods are generally used to control the behaviour of a widget after initialization  

####Styles 
- When we attach the UI id to an HTML element, JQuery will attach various classes. These classes enable the styling. 
- We can use these class names to overwrite with our own styles  

####Sprite
- Icons can be selected using a ui.css class. This refers to a single png file which is displayed as a sprite. 

####Most Useful Widgets 
- dialog - replaces the alert box
- tabs - contains related content in a tabbed box, saving space 
- slider - allows user input on a scale 
- progress bar - shows output on a scale; use for timers, progress on a form, etc. 
- autocomplete - supply specific values to search boxes  
- button and buttonset - force consistent styling on inputs, anchors, radios and checkboxes  

####Less Useful 
- Accordian - like tabs, but more annoying 
