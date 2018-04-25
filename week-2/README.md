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

## Preview webpage

1. In Atom, right click on `index.html` and select `Show in Finder`
1. From the window, double click `index.html` to open the file in the default web browser

Nice website! Leave this window open for now, we'll be coming back to it later.

## Add image

The website is pretty plain and boring, let's add an image to spice it up a bit...

1. Open [this image](https://github.com/BerlinCodeClub/BerlinCodeClub.github.io/raw/master/me.jpg) and save it to the root of your repository
1. Switch back to `Atom`, click on `index.html` to open it
1. Above the `h1` tag, copy and paste the following HTML:

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
1. Below the closing tag of the interests list - `</ul>` - insert the following HTML:

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

- Get HTML template
- Add header image
- Add sign up form
- Add cards
- CSS intro
- Playtime

HTTP end to end demo?
