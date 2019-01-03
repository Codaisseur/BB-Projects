# Building All The Boxes

## 🎨 What we will build
By then end of this section, your index page will display images based on the example data in the previous section.

## 🎯 Learning Goals
By the end of this section, you will learn:
* [ ] how to use an iterator to create elements on a page with content from an array

## 📚 Modules that will be discussed
* All!

## ✏️ Assignments

#### Display data on your page

1. In `index.html`, comment out all links in the gallery section. Your page should look something like this: ![Empty index page](https://cd.sseu.re/Museum_Guide_2019-01-03_10-08-41.png).

> ## 👌 Pro-tip
> You can comment out a large section of code by selecting the code and `cmd` + `/`, or `ctrl` + `/`.

2. Declare a variable called `paintings` and assign it the value of the the `artObjects` array of your `data` variable.
3. Iterate over your `paintings` array and log each element to the console. Check whether it worked out in your DevTools. This is what is should look like:
![paintings in console](https://cd.sseu.re/Museum_Guide_2019-01-03_10-17-11.png)
4. Now, rather than console log each value, use DOM methods to create some HTML code for each element in the array. The resulting HTML code should look something like this:
    ```html
    <a href="./pages/detail-page.html">
      <img alt=_title_of_painting_ class="artObject" src=_url_of_web_image_ />
    </a>
    ```
    The `alt` attribute of the `<img>` element should be the title of the painting and the `src` attribute should be the `url` of the `webImage` of the painting.

> ## 👌 Pro-tip
> Use the steps that you used to create a form on the detail page:
> * Gather Data (in this case `paintings[i]`)
> * Create the elements you need
> * Adjust the elements 
> * Display them on the page
>
> It might be helpful to write down what you need to do in English for each step. _Which data do you need_ ( = the current painting), _which elements should be created_ (see the resulting HTML code above), _how should the elements be adjusted_ (Which attributes do they have? Do they have any child elements?) and _where should they be displayed on your page_ (Which element should be their parent?)?

#### Cleaning Up
1. Move the code from the last assignment to a separate function called `displayPainting`, which should take one argument: `painting`.
1. Inside your `for-loop` declare a variable called `currentPainting` and assign it the current element of the array. Use your console to check whether you created the variable successfully.
1. Call the `displayPainting` inside your `for-loop` and pass it `currentPainting` as an argument. Check whether your index page is working again.
1. Remove the commented out links from `index.html`.

#### Push your work to GH:
1. Stage your changes, commit them and push them to GitHub:

```shell
$ git add .
$ git commit -m 'Set up js files and declare submitComment'
$ ggpush
```

#### Merge your branch
Merge your branch to master.


## 🎯 Learning Goal Tracker
In this section, you learned...

* [X] to recognize composite data structures.
* [X] to select specific data from complex data structures.
* [X] how to use an iterator to create elements on a page with content from an array
