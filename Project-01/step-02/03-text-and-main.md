# Styling: Main section and text

## 🎨 What we will build
Time to do some actual styling. We will be starting on the styling of your index page: 
![end result step 03](https://cd.sseu.re/Museum_Guide_2018-12-11_09-08-51.png)


## 🎯 Learning Goals
By the end of this section, you will learn:

* [ ] how to style specific elements on a page


## 📚 Modules that will be discussed

* [CSS 3]()


## ✏️ Assignments
### Styling the `<main>` section
* Inspect the styling of the `<main>` section and experiment with the values and properties to check what everything does:
![main section in devtools](https://cd.sseu.re/MuseumGuide_2018-12-05_14-54-42.png)

* Do these selectors refer to `element`s, `class`es or `id`s?

* If we want a similar styling in our own app, we don't need to copy all the code. Some styling is done by default by the browser. Can you figure out how to keep them apart?

![which code is done by the browser](https://cd.sseu.re/MuseumGuide_2018-12-05_15-00-48.png)

* Let's start with adding the code of the `main` selector:

```css
  main {
    background: white;
    width: 90%;
    margin: auto;
    border-radius: 5px;
    padding: 2rem 0;
  }
```

> ## 👌 Pro-tip
> Make sure to use indentation! It helps with debugging and makes it easier to see where your declarations start and end.


> ## 😱  Sanity Check
> Your page should now look somewhat like this:
> ![final result 02.03.01](https://cd.sseu.re/Museum_Guide_2018-12-07_09-24-52.png)

## Text
In this assignment, you will be styling the text on the page.

* Inspect the title of your page and apply the margin specified for the `<h1>` element in `index.css`
* Add the `text-align` and `font-family` properties and their values to the `body`-selector in `index.css`

> ## 😱  Sanity Check
> Your `index.css` should have the following content:
>```css
> body {
>    background: #FFBA00;
>    font-family: 'Inconsolata', monospace;
>    text-align: center;
>  }
>
>  main {
>    background: white;
>    width: 90%;
>    margin: auto;
>    border-radius: 5px;
>    padding: 2rem 0;
>  }
>
>  h1 {
>    margin: 3rem 1rem 6rem 1rem;
>  }
>```

* When you compare your application to the example app, you'll notice that the fonts are still slightly different. Do you know why that is the case?

* Add the following line to at the bottom of the `<head>`-section of your HTML file, to load the correct font: 
```html
<link href="https://fonts.googleapis.com/css?family=Inconsolata" rel="stylesheet">
```

* If it all worked out, feel free to go to [fonts.google.com](https://fonts.google.com/) and select a font you like!


### Missing styles
* Check which CSS rules are missing still in your `body`-selector and add them to your `body`-selector in `index.css`. Make sure to check out what each of them is doing in your DevTools!

> ## 😱  Sanity Check
> Your `index.css` should have the following content:
>```css
> body {
>    background: #FFBA00;
>    font-family: 'Inconsolata', monospace;
>    text-align: center;
>    margin: 0;
>    padding: 2rem 0;
>    width : 100%;
>  }
>
>  main {
>    background: white;
>    width: 90%;
>    margin: auto;
>    border-radius: 5px;
>    padding: 2rem 0;
>  }
>
>  h1 {
>    margin: 3rem 1rem 6rem 1rem;
>  }
>```
### Push your changes to GitHub
Check your changes, select the ones you want to commit, commit and push them to your branch.

 ```shell
 $ gst 
 $ git add .
 $ git commit -m 'Style main section and text'
 $ ggpush
 ```

## 🎯 Learning Goal Tracker
In this section, you learned...

* [X] how to use Chrome DevTools to inspect the CSS of a page using different views
* [X] how to create an CSS page in your text editor and link it to your HTML file
* [X] how to style specific elements on a page
* [ ] how to apply some of basic concepts of responsive web development
