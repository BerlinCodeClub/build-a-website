# Week 3

Wow, it's week 3 already!

## Week 2 recap

- Using the code editor `Atom`
- More HTML
- Style! Adding some CSS
- Committing code with Git and publishing to GitHub

## A layout for the contact section

### The HTML structure

1. Open `index.html` in `Atom`
1. Find the HTML code for the "Contact me"
1. Wrap it in a HTML `div` element
1. Add a `class` attribute with the value "contact"

A part of your HTML code should now look like this:

```
<div class="contact">
  <h2>Contact me</h2>
  <div>
    <form>
      <input type="text" placeholder="Type your message">
      <input type="submit" value="Send">
    </form>
  </div>
</div>
```

### Add a border and colors

1. Add the following CSS code to your  `style.css`:

```
.contact {
  border-color: darkgray;
  border-width: 2px;
  border-style: solid;
  background-color: lightgray;
}
```

Preview the result in the browser.

### Add some spacing

1. Add margin and padding so the CSS code looks like that:

```
.contact {
  border-color: darkgray;
  border-width: 2px;
  border-style: solid;
  background-color: lightgray;
  margin: 20px;
  padding: 20px;
}
```

Preview again in the browser.

## Hack away

Some HTML elements are "block" elements by default and can have layout. E.g. `<p>`, `<div>`, `<h1>`, `<ul>`, `<li>`, `<body>`.

**Note:** There's also `border-bottom-width`, `margin-top` and other combinations available.

Apply what you learned about layout to your page elements as you wish. Get creative!

## Basic Layout deep dive

Boxes, width and height, margins, paddings, ...

https://internetingishard.com/html-and-css/css-box-model/

## Commit changes

Whenever you're happy with changes and additions you did to your page, use the GitHub desktop app to commit the changes to Git. Give the commit a meaningful summary and description to help future you to understand what you did there and why.

## Developer Tools

Inspect the elements you are adding layout to.

## Publish

Publish (push) your changes to GitHub with the GitHub app.
