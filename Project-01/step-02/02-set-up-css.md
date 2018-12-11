# Styling: Set up

## 🎨 What we will build
In this section, you will create a css file and connect it to your `index.html`. By the end, your page will look somewhat like this: ![End result step 02](https://cd.sseu.re/Museum_Guide_2018-12-11_09-06-18.png)


## 🎯 Learning Goals
By the end of this section, you will learn:

* [ ] how to create an CSS page in your text editor and link 


## 📚 Modules that will be discussed

* [CSS 1]()


## ✏️ Assignments
### Creating a new branch
As we are starting on a new part of this project, we will be creating a new branch. 

* In your terminal, navigate to your project.
* Make sure you are on the master branch and you have pulled the latest version of:

```shell
$ git checkout master
$ ggpull
```

>  _❗️ If it did not work, make sure you did **not** copy the dollar sign and that you copied the commands **one line at the time**!_ 

* Create a new branch and check it out using `git checkout -b feat/style-index-and-detail-page`.

You are ready to go!

### Setting Up your CSS
* In your terminal, inside your project directory, open your project in your editor using the command `code .`.
* In VSC, in the main directory of your project, create a new file called `index.css`.
* At the bottom of the the `<head>`-section of `index.html`, add the following line:
```html
<link rel="stylesheet" type="text/css" media="screen" href="index.css">
```
* In `index.css`, add a rule that sets the background color of the body element to #FFBA00.
```
* Open `index.html` in your browser (or refresh the page if you had it opened, still) and check what happened.
* In your editor, change the background color to your favorite color.

> ## 😱  Sanity Check
> Your page should now look somewhat like this:
> ![final result 02.02](https://cd.sseu.re/Museum_Guide_2018-12-05_14-46-48.png)

### Push your changes to GitHub
Check your changes, select the ones you want to commit, commit and push them to your branch.

 ```shell
 $ gst 
 $ git add .
 $ git commit -m 'Set Up CSS, first version background'
 $ ggpush
 ```

## 🎯 Learning Goal Tracker
In this section, you learned...

* [X] how to use Chrome DevTools to inspect the CSS of a page using different views
* [X] how to create an CSS page in your text editor and link it to your HTML file
* [ ] how to style specific elements on a page
* [ ] how to apply some of basic concepts of responsive web development
