---
title: js-window
---

# JavaScript Window 🪟


### 1. Introduction 
####  what is window?
In JavaScript, a `window` refers to the global object that represents the web browser's window or tab where your web page is displayed. It provides access to various properties and methods for interacting with the browser and the document loaded in it. It's a fundamental part of the JavaScript environment for web development.
    
### 2. BOM & DOM?

#### what is DOM?
  **DOM** Stands for Document Object Model.
    DOM deals with only browser tab `document`. 


#### what is BOM?
  **BOM** Stands for Browser Object Model.
  BOM deals with browser components.
  
##### Properties of BOM with `window` object
   
 ~ `navigator`
 ~ `screen`
 ~ `history`
 ~ `location`
 ~ `frame`
 ~ `XMLHttpRequest`
 


###  Windows.Objects

#### window.screen : 
The `window.screen` is used for interaction with screen.

 The properties `screen` object contain.
 ~ `width`
 ~ `availWidth`
 ~ `height`
 ~ `availHeight`
 ~ `orentation`
 ~ `pixelDepth`
 ~ `colorDepth`
 
 
 HTML

```
<button type="button" onclick="getResolution();">Get Resolution</button>

```


JAVASCRIPT
```js

 function getResolution() {
        alert("Your screen is: " + screen.width + "x" + screen.height);
    }
 
```
 
 
 
 #### window.open :
`window.open` method is used to open a new browser window or tab. It takes parameters such as the URL to open, window name, dimensions, and more.


HTML

```
<button onclick="openWin()">Open "myWindow"</button>

```


JAVASCRIPT
```js

 let myWindow;

function openWin() {
  myWindow = window.open("", "", "width=200,height=100");
}
 
```




#### window.innerWidth & window.innerHeight : 
These properties provide the width and height of the browser window's content area.

```js

let w = window.innerWidth;
let h = window.innerHeight;

let x = "screen width:" + w + "," + "screen height:" + h;

console.log(x);

```


#### window.close: 
Used to programmatically close the current browser window.


HTML

```
<button onclick="closeWin()">Close "myWindow"</button>

```


JAVASCRIPT
```js
 let myWindow;

function closeWin() {
  myWindow.close();
}
 
```

