# Week 4

Let's do some PROGRAMMING with JavaScript! 🎉

## Week 3 recap

- Personal page: basic layout and style with CSS
- What is Git and GitHub really?

## Interactive programming in the browser console

### Open the browser console

In Chrome, press Command+Opt+J and find the input cursor at the bottom.

### Enter code

Type `1 + 1` and press enter.

Next, type `alert("This computer does exactly what I tell it to do")`.

**Explanation:** This part is the essence of the JavaScript console: you get to type in a one-line program, and the browser will run it for you, and tell you what the result was. If you write something that is not a valid program, it will try to tell you what went wrong.

1 + 1 is probably the simplest program possible. Try other calculations.

**Hint:** Use arrow up and down keys to save yourself some typing!

The second program (`alert(…)`) is a function call. The function available under the name "alert" is an operation for showing a little dialog window on the screen. The parentheses are the notation for invoking a function, and the value in between is an argument or paramter to the function as further info. In this case, it told the alert function which text to display.

### Understand expressions

Combine the two programs from the previous step: `alert(1 + 1)`.

Enter "hey" + "ho".

**Explanation:** The kind of program fragment we have been writing so far is called an expression. Expressions are like Lego blocks, in that you can combine them into bigger, more interesting expressions.

### Variables

Enter the following lines at the console:

```javascript
var myvalue = 32 * 32
alert(myvalue)
myvalue = 10
alert(myvalue)
```

**Explanation:** With `var` you declare a variable. This introduces a name and associates a value with it. Afterwards, the name ("myvalue", in this case) can be used to refer to the current value of the variable by that name.

## Applying a JavaScript program to our web page

Open your web page project from last week with the Atom Editor.

### Accessing HTML elements with JavaScript

1. In your HTML file, add an "id" attribute with a unique value (no spaces or special characters allowed) to any HTML element like so: `<div id="myElement">`.
1. Save the file and open the page in the browser.
1. In the browser console, type `document.getElementById("myElement")`

You will see a representation of the HTML element logged to the console.

It is also possible to get more specific information from the element. For instance you can read the ID from it like so: `document.getElementById("myElement").id`. Try it out!

**Explanation:** With the dot you access things deeper in a hierachy, in this case a property of an element of the document (page).

Remember variables can be used to store and read values:

```javascript
var myElement = document.getElementById("myElement")
myElement.id
```

### Manipulating HTML elements

Try entering the following code in the console:

1. `document.getElementById("myElement").style.backgroundColor = "green"`
1. `document.getElementById("myElement").innerHTML = "green"`

😲 We made stuff change and disappear! ✨ But this is not permanent, just refresh the page and we are back where we were.

**Explanation:** With JavaScript we can get and also set styles just like we can apply styles with CSS. We just cannot use "-" for the property names because JavaScript would confuse it for a minus (remember JavaScript can do math). Just write everything together - like German words - but capitalize every new part of the name. You can also get and set text and even HTML content within an element.

## Adding JavaScript to our code project

1. Create a new file next to `index.html` called `script.js` with the following content: `alert("test")`.
1. Open `index.html`, find the closing body tag at the bottom of the file (`</body>`) and add the following in a new line above: `<script src="script.js"></script>`.

The code at the bottom of the HTML should like like that:
```html
...
    <script src="script.js"></script>
  </body>
</html>
```

Refresh the page in the browser. It should open a dialog with "test".

Commit the changes to Git.

## Interaction

1. Anywhere in your HTML between `<body>` and `</body>` add the following code: `<button id="magicButton">Click me!</button>`.
2. Replace the code in `script.js` with the following:

```javascript
document.getElementById("magicButton").addEventListener("click", function() {
  alert("test")
})
```

Refresh the page and click the button. Click "Ok". Click the button again. How do you like your first interactive program?!

**Explanation:** We haven't learned enough, yet, to fully understand how this works. For now it's enough to know that whenever the button is clicked we run some code in a function.

## Exercise

Replace the alert code with some of the style and text manipulations we did earlier in the console. Just add multiple lines.

Add "id" attributes to more elements and do stuff with them when the button is clicked.

Try to add another button with a separate event listener.

**Hint:** You can change the class of elements with JavaScript like this: `document.getElementById("myElement").className = "summary-text"`. If you have nice styles for a class in your CSS file, you can apply them all together with JavaScript like that.
