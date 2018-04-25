# Week 2

Welcome to week two!

## Week 1 recap

- `GitHub` account setup
- `GitHub Desktop` downloaded
- Logged in to `GitHub Desktop`
- `Atom` downloaded
- Create repository named `username.github.io`

## Add index.html

1. Launch `Atom`
1. Select `Open a Project` from the options on the right hand side welcome screen
1. From the window, navigate to the path of your repository and click `Open`
1. From the file tree view, right click on the repository name and select `New file`
1. Enter `index.html` and hit `Enter`

## Add HTML

1. In `Atom`, click on `index.html` to open it
1. Copy and paste the HTML below into the HTML page

````
<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title>Welcome to Billy Bob's website</title>
  </head>
  <body>
    <h1>Billy Bob</h1>
    <h2>Summary</h2>
    <p>Hi! I'm Billy Bob and this is my website.</p>
    <h2>Interests</h2>
    <ul>
      <li>Sports</li>
      <li>Nintendo</li>
      <li>Nuclear physics</li>
    </ul>
    <h2>Contact me</h2>
    <div>
      <form>
        <input type="text" placeholder="Type your message">
        <input type="submit" value="Send">
      </form>
    </div>
  </body>
</html>
````

## HTML quick dive

https://internetingishard.com/html-and-css/basic-web-pages/ 

## Preview webpage

1. In Atom, right click on `index.html` and select `Show in Finder`
1. From the window, double click `index.html` to open the file in the default web browser

Nice website! Leave this window open for now, we'll be coming back to it later.

## Add image

The website is pretty plain and boring, let's add an image to spice it up a bit...

1. Open [this image](https://github.com/BerlinCodeClub/BerlinCodeClub.github.io/raw/master/me.jpg) and save it to the root of your repository
1. Switch back to `Atom`, click on `index.html` to open it
1. Above the `h1` tag, copy & paste the following HTML:

`<img src="me.jpg">`

The updated HTML should now look like:

````
<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title>Welcome to Billy Bob's website</title>
  </head>
  <body>
    <img src="me.jpg">
    <h1>Billy Bob</h1>
    <h2>Summary</h2>
    <p>Hi! I'm Billy Bob and this is my website.</p>
    <h2>Interests</h2>
    <ul>
      <li>Sports</li>
      <li>Nintendo</li>
      <li>Nuclear physics</li>
    </ul>
  </body>
</html>
````

Switch back to the web browser with the website open and refresh to see the updates - beautiful!

## Add text input

People are going to love this website, we should give them some way of contacting you...

1. Switch back to `Atom`, and open `index.html` once again
1. Below the closing tag of the interests list - `</ul>` - copy & paste the following HTML:

````
<div>
  <form>
    <input type="text" placeholder="Type your message">
    <input type="submit" value="Send">
  </form>
</div>
````

The updated HTML should now look like:

````
<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title>Welcome to Billy Bob's website</title>
  </head>
  <body>
    <img src="me.jpg">
    <h1>Billy Bob</h1>
    <h2>Summary</h2>
    <p>Hi! I'm Billy Bob and this is my website.</p>
    <h2>Interests</h2>
    <ul>
      <li>Sports</li>
      <li>Nintendo</li>
      <li>Nuclear physics</li>
    </ul>
    <div>
      <form>
        <input type="text" placeholder="Type your message">
        <input type="submit" value="Send">
      </form>
    </div>
  </body>
</html>
````

Switch back to the web browser and refresh again.

## Add CSS stylesheet

1. Open `Atom`
1. From the file tree view, right click on the repository name and select `New file`
1. Enter `style.css` and hit `Enter`
1. Open `style.css` and copy & paste the following CSS:

````
h1 { 
  color: darkolivegreen; 
}

.summary-text {
  color: peachpuff;
}
````

Switch back to the web browser and refresh again - nothing happened?

This is because we still need to include this CSS stylesheet in our HTML page.

1. In `Atom`, open `index.html` and copy & paste the following HTML under our `<title>` tag:

`<link rel="stylesheet" href="style.css">`

The updated HTML should now look like:

````
<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title>Welcome to Billy Bob's website</title>
    <link rel="stylesheet" href="style.css">
  </head>
  <body>
    <img src="me.jpg">
    <h1>Billy Bob</h1>
    <h2>Summary</h2>
    <p>Hi! I'm Billy Bob and this is my website.</p>
    <h2>Interests</h2>
    <ul>
      <li>Sports</li>
      <li>Nintendo</li>
      <li>Nuclear physics</li>
    </ul>
    <div>
      <form>
        <input type="text" placeholder="Type your message">
        <input type="submit" value="Send">
      </form>
    </div>
  </body>
</html>
````

Switch back to the web browser and refresh again. The main heading - `<h1>` in our code - is now `dark olive green` but we don't see anything `peach puff` in colour...

This is because `h1` in our CSS will be applied to every `<h1>` element in our HTML but `.summary-text` is targeting the element CSS class. We haven't added any CSS classes to our HTML yet so this means this style won't be applied.

Let's add a class to our `<p>` tag by adding `class="summary-text"` to the opening tag. It should now look like this:

`<p class="summary-text">Hi! I'm Billy Bob and this is my website.</p>`

Switch back to the web browser and refresh again. The heading and summary text are both coloured.

[This page](https://developer.mozilla.org/en-US/docs/Web/CSS/color_value) details using colours in HTML & CSS further.

## Commit and push

1. Switch back to `GitHub Desktop`
1. The file tree view on the left shows `1 changed file` and `index.html` is displayed
1. Below this, enter a `Summary` and `Description` to describe the changes contained in this commit and then click `Commit to master`
1. The file tree view now shows `0 changed files`
1. Click the `Publish repository` button to `push` the committed changes to GitHub
1. In the popup, make sure `Keep this code private` is unselected and click `Publish Repository`

## GitHub pages

Launch a new web browser window and go to https://USERNAME.github.io

Our web page is now online 🤘

## Hack around

So we've added HTML with some styling and deployed this to the cloud.

Spend some time experimenting with different HTML & CSS combinations on your website.

Person with the ugliest website wins.

### HTML elements

Go to examples section, copy and paste HTML into your page.

- [Hyperlink](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/a)
- [Table](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/table)
- [Drop down](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/select)

### CSS

Go to examples section, copy and paste these into your stylesheet.

- [Background colour](https://developer.mozilla.org/en-US/docs/Web/CSS/background-color)
- [Border](https://developer.mozilla.org/en-US/docs/Web/CSS/border)
- [Font size](https://developer.mozilla.org/en-US/docs/Web/CSS/font-size)
- [Font weight](https://developer.mozilla.org/en-US/docs/Web/CSS/font-weight)
- [Text decoration](https://developer.mozilla.org/en-US/docs/Web/CSS/text-decoration)
