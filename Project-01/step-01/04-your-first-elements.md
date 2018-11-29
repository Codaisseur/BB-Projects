# Building All The Boxes

## 🎨 What we will build
By then end of this section, your page will look like this one: 
![final result](https://cd.sseu.re/Museum_Guide_2018-11-28_18-03-17.png)

## 🎯 Learning Goals
By the end of this section, you will learn:

* [ ] some important HTML tags, and when/why you should use them

## 📚 Modules that will be discussed

  * [HTML 1](or2?)
  * [Git 2](orGitHub?)

## ✏️ Exercises
### Adding `<main>`, `<footer>`, `<h1>` and `<section>` elements
Let's make sure our page has something to show!

1. Thinking in 'boxes', we could split up the page as like the image below. The different level of boxes are color coded. The outer box has a blue border, the boxes inside the blue border are grey, the boxes inside the grey border are black and the boxes inside the black border are orange. Using the elements in your DevTools, can you assign each elements in the list below to the right color?
    * `<body></body>`
    * `<main></main>`
    * `<footer></footer>`
    * `<h1></h1>`
    * `<section id="gallery"></section>`
    * `<p></p>`
    * `<a href="..."></a>`

![Page in boxes](https://cd.sseu.re/MuseumGuide_2018-11-28_18-50-13.png)

2. Now that we have an overview of all elements on our page, let's start building one. The first two elements we encounter inside our body, are the elements with a black border. Checking our DevTools, we can see these are a `<main>` and a `<footer>` element. Add those elements inside the `<body>` element on your page!

![main and footer in devtools](https://cd.sseu.re/MuseumGuide_2018-11-28_19-03-30.png)

3. We'll continue working on the main section. Opening your DevTools, can you see which elements should be inside your `<main>` element? Make sure to also add the attributes. If there are no nested elements anymore, also add the content, change "Mimi"  to your own name!

> ## 😱  Sanity Check
> Your code should now look like this:
>```html
><!DOCTYPE html>
><html>
>  <head>
>    <title>Museum Guide</title>
>  </head>
>  <body>
>   <main>
>     <h1> _YOUR_NAME_ Mobile Museum App</h1>
>     <section id="gallery">
>
>     </section>
>   </main>
>  </body>
></html>
>```

Your page should now look something like this: 

![page with blue, grey and black layer](https://cd.sseu.re/Museum_Guide_2018-11-29_15-09-51.png)

### Adding `<a>` and `<img>` elements
The main framework is there, all we need to add is the content of the 'boxes' with orange borders:
![Page in boxes](https://cd.sseu.re/MuseumGuide_2018-11-28_18-50-13.png)

1. Check the `<section>` element in your DevTools. What does it contain? 
![inside section element](https://cd.sseu.re/MuseumGuide_2018-11-29_15-17-25.png)
2. Add an `<h2>` element to your `<section>` element, with the content: 'Gallery'.
3. Add 5 `<a>` elements to your `<section>` element. Assign all their `href`-attributes to "./pages/detail-page.html".
4. Inside each `<a>` element, add a `<img>` element. Give each of them an attribute with the name "class"  and as value the string "artObject". Don't forget to add a 'source' and an 'alt' attribute! Pick the 5 images you like best, or find your own, anywhere on the internet!

> ## 👌 Pro-tip
> _When using picture from the internet, you should use the `image address` of the picutre. You can find it by right-clicking on any image and select `copy image address`_
> ![copy image address](https://cd.sseu.re/een_vrolijke_vioolspeler_-_Google_Search_2018-11-29_16-06-33.png)

> ## 😱  Sanity Check
> Your page/code should now look like this:
> ![final result exercise 2](https://cd.sseu.re/Monosnap_2018-11-29_16-15-23.png)

5. Why are the images under the 'gallery' title ? Why are the images ne


### Create a footer
Inspect the footer and add the code to your `index.html` file!

> ## 😱  Sanity Check
> Your page should now look like this:
> ![End result exercise 2](https://cd.sseu.re/Museum_Guide_2018-11-29_16-22-51.png)
> You can find a link to the code [here]("./finalResults")

### Push your work to GH:
1. Stage your changes, commit them and push them to GitHub:

```shell
$ git add .
$ git commit -m 'Add all elements to index page'
$ ggpush
```


## 🎯 Learning Goal Tracker
In this section, you learned...

* [X] how to navigate and do basic management of the file system from the shell
* [X] how to use git & gitHub for version tracking
* [X] how to use Chrome DevTools to inspect the HTML of a page
* [X] how to create an HTML page in your text editor and open it in the browser
* [X] some important HTML tags, and when/why you should use them
