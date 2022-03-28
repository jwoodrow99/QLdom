# QL-dom

QL-dom is a library apart of the QL-dev framework. This library is designed to help beginner coders get started with DOM manipulation by simplifying the complex vanillaJS syntax. This library allows for beginner developers to create basic interfaces without having to write HTML or CSS. By using QL-dom, beginner developers can focus on creating simple, yet functional user interfaces while only needing to learn browser based JS.

## How to use

This git repo contains the README documenting the functionality of this library as well as the library file itself. You can easily use QL-dom in your project by requiring the script in your HTML file, adding a div tag for QLdom to run inside of and instantiating the QL-dom object in your js file.

```index.html```

```html
<script charset="utf-8" src="QLdom.js" type="text/javascript"></script>
<script defer charset="utf-8" src="app.js" type="text/javascript"></script>

<body>
	<div id="app"></div>
</body>
```

```app.js```

```javascript
const QL = new QLdev('app');
```

Alternatively you can download the full [QL-dev starter project](https://github.com/jwoodrow99/QL-dev/archive/refs/heads/main.zip). All you have to do is unzip it and start coding!

## Commands

**All created elements and fields are added to the bottom of the body.**  
**! = optional parameter.**

### OUTPUT  

```javascript
print(text, !id);
```

creates a "p" element with the content of the text parameter, with or without an id attribute.  

```javascript
break(!id);
```  

Creates a "br" tag with or without an id attribute.  

```javascript
space(!size, !id);
```

This function allows you to make a space in your code to make it look better. You can give it a size in pixels and an id, or just a size, or nothing at all and will create your space with a default size of 25 pixels.  

```javascript
edit(id, text);
```

Changes the display value of a "p" tag with the matching id attribute.

```javascript
clearValue(id);
```

This function will clear the value of an input field.  

```javascript
remove(id);
```

Removed the element with the matching id attribute.  

```javascript
hide(id);
```

Hides the element with the matching id attribute from the user.  

```javascript
show(id);
```

Shows hidden elements to the user after them being hidden with the hide() function matching the id attribute.  

### STYLES  

```javascript
textColor(id, color);
```

changes the text color of the element with the matching id to the specified color.  

```javascript
backgroundColor(id, color);
```

changes the background color of the element with the matching id to the specified color.  

### LOGICAL  

```javascript
exists(id);
```

Returns true if an element with a matching id attribute exists.  

```javascript
valueOf(id);
```

Returns the value of the element with the matching id attribute, or innerHTML vale of p tag.  

### META  

```javascript
changeAttribute(id, attribute, value);
```

This function allows you to add any valid html attribute and its value to an element with a matching id, or change the attribute if it already exists.  

```javascript
removeAttribute(id, attribute, value);
```

This function allows you to remove any html attribute that has previously been assigned to an element.  

```javascript
changeClass(id, newClass);
```

This function will change an existing class or add a class to an element that does not have one, where the id matches the id attribute.  

```javascript
removeClass(id);
```

This function will remove the class attribute from the element where the id matches the id attribute.  

```javascript
changeId(id, newId);
```

This function will change the id of the element with the matching id attribute to the newId.  

```javascript
removeId(id);
```

This function will remove the id attribute from the element where the id matches the id attribute.  

### INPUT  

```javascript
button(text, function, !id);
```

This function allows you to create a button and link a function to it. text being what text is displayed on the button, fcn being the function you are linking, and id being the id attribute you are assigning to the button element.  

```javascript
keyPress(key, function)
```

This function allows you to write a function and have it execute when the specified key is pressed.  

```javascript
textBox(id);
```

This function creates a text box with an id.  

```javascript
textArea(id, !r, !c);
```

This function allows you to create a text area, this area is much larger than a text field, if you only include one parameter (being the id) it will make the text area with the default size of 10X50 characters, but if you include the parameters (r and c) you can specify the number of rows and columns of characters.  

```javascript
radioButton(id, name, value);
```

This function allows you to create a radio button, which is like a checkbox, but you can only select one of the group. In order to specify the group the 'name' parameter must be the same as all of the other radio buttons in the group. Then when you use the QL.value(); function include one id from any of the radio buttons apart of the group.  

```javascript
checkBox(id, value);
```

This function allows you to create a check box giving it an id and a value, if the checkbox is selected the 'value' parameter will be the result, if the box is not checked it will have the value of null.
