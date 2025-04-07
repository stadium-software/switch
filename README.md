# Switch

A switch is a way to for users to make a boolean selection. Switches imply that they are effective immediately. Use switches when you want users to make a boolean selection that will be applied immediately.

https://github.com/stadium-software/switch/assets/2085324/64812cbc-de58-4e87-8720-9d7bba8c745e

## Version 
v1.1 - Updated CSS for Stadium 6.12;

1.1.1 Updated readme CSS for Stadium 6.12+; Converted px to rem;

# Setup

## Application Setup
1. Check the *Enable Style Sheet* checkbox in the application properties

## Page Setup: Switch only
1. Drag a *Checkbox* control to a page 
2. Add the class "stadium-switch" to the control's class property

## Page Setup: Switch with labels
1. Drag a *Container* control to a page 
2. Add the class "stadium-switch" to the control's class property
3. Drag a *Checkbox* control and place it into the *Container*
4. Drag a *Label* control and place it to the left of the *Checkbox* inside the *Container*
5. Enter text in the *Label's* text property to denote the "Off" state of the switch
6. Optionally, drag another *Label* control and place it on the right-hand side of the *Checkbox*
7. Enter text in the *Label's* text property to denote the "On" state of the switch

![](images/Container-Layout.png)

![](images/Switch-Rendered.png)

## CSS
The CSS below is required for the correct functioning of the module. Variables exposed in the [*css-file-variables.css*](css-file-variables.css) file can be [customised](#customising-css).

### Before v6.12
1. Create a folder called "CSS" inside of your Embedded Files in your application
2. Drag the two CSS files from this repo [*css-file-variables.css*](css-file-variables.css) and [*css-file.css*](css-file.css) into that folder
3. Paste the link tags below into the *head* property of your application
```html
<link rel="stylesheet" href="{EmbeddedFiles}/CSS/css-file.css">
<link rel="stylesheet" href="{EmbeddedFiles}/CSS/css-file-variables.css">
``` 

### v6.12+
1. Create a folder called "CSS" inside of your Embedded Files in your application
2. Drag the CSS files from this repo [*css-file.css*](css-file.css) into that folder
3. Paste the link tag below into the *head* property of your application
```html
<link rel="stylesheet" href="{EmbeddedFiles}/CSS/css-file.css">
``` 

### Customising CSS
1. Open the CSS file called [*css-file-variables.css*](css-file-variables.css) from this repo
2. Adjust the variables in the *:root* element as you see fit
3. Stadium 6.12+ users can comment out any variable they do **not** want to customise
4. Add the [*css-file-variables.css*](css-file-variables.css) to the "CSS" folder in the EmbeddedFiles (overwrite)
5. Paste the link tag below into the *head* property of your application (if you don't already have it there)
```html
<link rel="stylesheet" href="{EmbeddedFiles}/CSS/css-file-variables.css">
``` 
6. Add the file to the "CSS" inside of your Embedded Files in your application

**NOTE: Do not change any of the CSS in the 'css-file.css' file**

## Upgrading Stadium Repos
Stadium Repos are not static. They change as additional features are added and bugs are fixed. Using the right method to work with Stadium Repos allows for upgrading them in a controlled manner. 

How to use and update application repos is described here: [Working with Stadium Repos](https://github.com/stadium-software/samples-upgrading)