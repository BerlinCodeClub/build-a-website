# Week 1

Welcome to the first week!

Today we're going to begin building a website.

Before writing any code, we need somewhere to host our code.

TODO: Talk about what git is here

## Create GitHub account

1. Launch a new web browser window
1. Go to https://github.com/
1. Fill out the signup form and click `Sign up for GitHub`
1. Select the personal (free) plan, leave the two checkboxes unticked and click "Continue"
1. Click the small `Skip this step` link at the bottom of the form
1. Open your email inbox, find the email from GitHub and click the link to verify your email address

## Install GitHub Desktop

When working with git, it's possible to use the command line, a desktop client or even a web browser.

Today we are going to use the `GitHub Desktop` application as it simplifies and hides a lot of the more complex git functionality, cross platform and also works seamlessly with GitHub.

1. Launch a new browser window
1. Go to https://desktop.github.com/
1. Click the download button
1. Once download is complete, extract zip file and install
1. Launch the GitHub Desktop app
1. Click `Sign into GitHub.com`
1. Sign in
1. Configure Git and continue
1. Click `Finish` to complete installation

## Create a repository

Now that we have a GitHub account and the `GitHub Desktop` app installed, our next step is to create a repository to host our website code.

TODO: Info about repository

1. Launch `GitHub Desktop`
1. Click `Create new repository`
1. For `Name` enter `USERNAME.github.io` - replace `USERNAME` with your own GitHub username
1. For `Description` use your imagination
1. Choose the path where this repository will be stored locally on your machine
1. Leave the remaining fields as default
1. Click `Create Repository`

## Download Atom code editor

Now that you have a code repository, we can finally start writing some code.

While it is possible to edit our code using only Notepad, using a code editor or IDE (Integrated Development Environment) will make our lives MUCH more enjoyable.

Some benefits of IDEs:

- Code auto-complete
- Extension packages
- Debugging
- Colour themes

There are many IDEs to choose from - Atom, Sublime, Visual Studio Code, WebStorm. Today we're working with Atom as it's open source, easy to get started with and well suited to frontend development.

1. Go to https://atom.io/
1. Click the download button
1. Once download is complete, extract zip file and install

## Create web page

Now we have our IDE setup, it's time to create our first web page and write some HTML.

`HTML (Hypertext Markup Language)` is the code used to structure a web page and content and is composed using `elements.`

`Elements` can consist of:

- Opening tag
- Closing tag
- Attributes
- Content

Taking the following paragraph element as an example:

`<p class="big">HTML is fun</p>`

- `<p>` is the element opening tag
- `</p>` is the element closing tag
- The element contains a single `class` attribute with a value of `big`
- `HTML is fun` is the element content

Next let's start populating `index.html` with some content.

1. Launch `Atom`
1. From the list of options on the right hand side select `Open a Project`
1. From the Finder window, navigate to the path of your repository and click `Open`
1. In the file tree view on the left you will see your repository already contains `.git` files - you can ignore these for now
1. From the file tree view, right click on the repository name and select `New file`
1. Enter `index.html` and hit `Enter`
1. Now you COULD type all all your HTML by hand or alternatively use [Atom Snippets](https://flight-manual.atom.io/using-atom/sections/snippets/) by typing `html` and hitting `Enter`

The snippet has generated the outline for a HTML document:

```html
<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title></title>
  </head>
  <body>
  </body>
</html>
```

- `<!DOCTYPE html>` always needs to be included - for now that's all you need to know
- `<html>` wraps the entire HTML content and is sometimes known as the root element
- `<head>` contains web page elements which won't be be visible to users such as CSS styles, Javascript and meta information
- `<body>` contains the website content visible to users
- `<meta charset="utf-8">` tells your browser the web page is written using UTF-8 encoding
- `<title>` sets the title of the web page

## Preview web page

Now that we have our first web page created, let's preview it in a web browser.

1. In Atom, right click on `index.html` and select `Show in Finder` - this will be different if you're not using a Mac
1. From the Finder window, double click `index.html` to open the file in the default web browser

The browser window is empty - don't panic! We haven't added any content yet, once we do this, our browser window will start to look more interesting. Let's start with adding a title to our web page.

## Add a page title

The web page title will be used to populate the browser tab title and also by search engines in search result titles.

1. In Atom, open `index.html`
1. Enter some content in the `title` element

For example, before:

`<title></title>`

And after:

`<title>My webpage title</title>`

Switch back to your web browser and refresh the page. The browser tab title will now match the title content.

## Add web page content

TODO: Add Wendi's content here

## Browser dev tools

All modern browsers offer a collection of inbuilt developer tools which assist in helping frontend developers in building, testing and debugging web pages.

This section assumes you are using Google Chrome however Firefox, Safari, Opera, and Edge contain similar functionality. Please avoid Internet Explorer at all costs.

1. Switch back to your web browser
1. Right click anywhere on the page select `Inspect` or alternatively from the file menu select `View` > `Developer` > `Developer tools`
1. From the developer tools overlay, select the `Elements` tab
1. The `Elements` tab displays the web page HTML
1. Try hovering over HTML elements in the `Elements` tab to see the corresponding elements highlighted on the page
1. Try adding, editing or deleting HTML elements in the `Elements` tab to see the corresponding elements updated in real time on the page

This is a very small part of what the the developer tools can do and we will continue digging deeper into these as the course progresses.

## Commit and push

Now `index.html` has been created and some content added, but it still doesn't exist in our GitHub repository yet.

For this to happen we need to `commit` our changes to the repository and `push` these to GitHub.

1. Switch back to `GitHub Desktop`
1. The file tree view on the left shows `1 changed file` with `index.html` being displayed
1. Below this, enter a `Summary` and `Description` to describe the changes contained in this commit and then click `Commit to master`
1. The file tree view now shows `0 changed files`
1. Click the `Publish repository` button to publish the committed changes to GitHub
1. In the popup, make sure `Keep this code private` is unselected and click `Publish Repository`

## View repository on GitHub website

The repository has been successfully published meaning you can now view the files on the GitHub website.

1. Launch a new web browser window
1. Go to https://github.com/
1. Click `Sign in`
1. Enter your username and password and click `Sign in`
1. From the right hand menu under `Your repositories` select the published repository
1. The repository contents are now visible, select `index.html` to view the file content online

## GitHub pages

An added feature when using GitHub is [GitHub Pages.](https://pages.github.com/)

By naming our repository `USERNAME.github.io` it is automatically hosted by GitHub Pages.

Launch a new web browser window and go to https://USERNAME.github.io

## End

We've setup our dev environment, added some basic HTML and published this to a live website people can view online.

Not bad for (hopefully) an hour or so effort!