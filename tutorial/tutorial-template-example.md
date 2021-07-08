# Tutorial example guide

**Structured Metadata for SEO purposes**
``` json
<script type="application/ld+json">
{
    "name": "Octopus library tutorial example",
    "description": "This guide explains how to build a good example Octopus library document for a specific doctype, which aligns with the principles of The Good Docs Project.",
    "version": "0.1",
    "datePublished": "2021-04",
    "license": "http://creativecommons.org/licenses/by/4.0/",
    "audience": "doctype template author"
}
</script>
```

**Version:** 0.1

**Last updated:** 2021-04-05 (YYY-MM-DD) by Ian

---
# Fictional example project

Here's an example of a small open source project that aims to guide developers and users through how to use their library

# An example of a technical project
Octopus library offers a great toolset to build a model of an octopus on web browser, from tentacle movements to the color and textures of an octopus. We want to guide developers and users through how they can use the library to build an octopus using Javascript, CSS and HTML. 

# Goal
This tutorial will guide you through how to use Octopus library, using Javacript to enable Octopus behaviours, CSS class names to enable the correct style of an octopus and HTML to build the base frame. 

# Before you start
Since Octopus library is aimed at web developers' usage, you should have a basic understand of 
- Javascript: DOM manipulation, methods, selecting HTML elements
- CSS: class name rulesets and properties
- HTML: semantic tags and their functions


# Part 1 - Set up + building a frame of the octopus
So you want to build a live model of an octopus that looks like an actual real life one. First, we need to create a base structure of the octopus. 

Download the Octopus library [here](https://octopus.com/download) and save them in your root folder

Create a new `index.html` in your root folder. Then let's create the structure with HTML tags and the below CSS classes:

```html
    <head>
        <title>This is Octopus</title>
        <link to='./octopus/dist/css/main.css' />
    </head>
    <body>
        <section class='octopus-model'>
            <div class='eye'></div>
            <div class='eye'></div>
            <div class='body'></div>
            <div class='tentacle'></div>
        </section>
        <script src='./octopus/dis/js/main.js'></script>
    </body>
```

We have linked to Octopus library, and declared a container to display our octopus, which is the `section` tag with a CSS class name `octopus-model` to input our own styling. 

Take notice of the `eye` and `body` and `tentacle` classes and the `<div>` tag within the section. These are pre-defined CSS classes that applies styling to your HTML tags. We suggest you use `<div>` for best results. 

For more pre-defined CSS classes from Octopus library, we suggest reading [the official doc](https://octopus.com/docs).

# Part 2 - Customizing styling with CSS

Now that we have a basic octopus, you can customize your octopus or add surround environment with CSS classes in your `index.html`, paste these divs with CSS classes

```html
    <head>
        <title>This is Octopus</title>
        <link to='./octopus/dist/css/main.css'>
    </head>
    <body>
        <section class='octopus-model'>
            <div class='eye'></div>
            <div class='eye'></div>
            <div class='body purple'></div>
            <div class='tentacle'></div>
            <div class='water'></div>
        </section>

        <script src='./octopus/dis/js/main.js'></script>
    </body>
```

Open the HTML file in your browser. We just added a new `<div>` tag with a custom class name `water`, and a new CSS class `purple` with the `body` CSS class. We'll add some new colors and sizes using CSS. 

Create a `style.css` file in the same folder with your HTML file

```css
purple {
    background-color: purple;
}

water {
    background-color: blue;
}
```

Remember to add a link to the file in your HTML

```html
<link rel='stylesheet' to='./style.css' />
```

Reload your browser again and you'll see the octopus body has turned purple and there a blue rectangle to represent the water environment

You can add many more classes of your own next to Octopus's pre-defined classes to customize looks and feels. 

# Part 3: Adding interactions with Javascript
Let's add some interactions and behaviours to the octopus we just created, using Javascript. 

Create a `script.js` file in your root folder. Remember to link the file from your HTML: 

```html
<script src='./script.js'></script>
```

In your `script.js`, copy and paste this line:

```javascript
document.getElementsByClassName('.tentacle').swing()
```

Now reload your HTML file on browser. You should see the `<div>` with class name `tentacle` will swing around like a real octopus moving in the water.

In the js file, we have selected the div tag with class name `tentacle` by using `getElementsByClassName()` method. This is the default browser's DOM method that lets us do this.

Then we chained it with another method called `.swing()`. This method comes from Octopus library and it can make an HTML element move around, like the octopus tentacle.

We can also make the octopus body move around as well. Add this line below: 

```javascript
document.getElementsByClassName('.body').upward().circle()
```

Now the body of the octopus will move up and down and swirl in the cirlce. Octopus library's method `.upward()` animate an HTML element to move up, then `.circle()` will make it swirl around. 

# What you've learned

So you have learned how to link and use Octopus library to take advantage of pre-defined CSS styling, use your own style with custom classes, and Javascript animation. Check out [Octopus Docs](https://octopus.com/docs) for many more fun animations and styling. Have fun!