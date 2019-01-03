# Building All The Boxes

## 🎨 What we will build
By then end of this section, you will have set up the connection between `detail-page.html` and `detail-page.js`.

## 🎯 Learning Goals
By the end of this section, you will learn:
* [ ] how to declare and call functions
* [ ] how to check JavaScript in your DevTools

## 📚 Modules that will be discussed
  * [Internet 1 ]()
  * [HTML 2 ]()
  * [Chrome DevTools 3]()
  * [JavaScript 4]()

## ✏️ Assignments

#### Check whether you are all setup
To work through these assignments, we expect that the html elements (and attributes!) of your `detail-page.html` are the same as those of the example app. Your code in `detail-page.html` should include these elements if they are not there, copy them into your `detail-page.html`:

```html
  <!-- ... -->

  <section id='comments'>
    <h2>Comments</h2>

    <section class='comment'>
      <h3>Arien said:</h3>
      <p>"This is definitely one of my favorites!"</p>
    </section>
  </section>

  <form onsubmit="submitComment(); return false">
    <div class="formSection">
      <label for="name">Name:</label>
      <input type="text" id="name">
    </div>
    <div class="formSection">
      <label for="msg">Message:</label>
      <textarea id="msg"></textarea>
    </div>
    <div class="button">
      <button type="default">Post your comment</button>
    </div>
  </form>
  <!-- ... -->
```
> ## 👌 Pro-tip
> If you see comment with three dots (like `<!-- ... -->` in the example), that means we left out some code in our example, that should however be present in your own code!

#### Create a new branch
New feature, so time for a new branch! Create a new branch with the name `feat/comment-form`
#### Set Up

1. In your pages directory, create a `detail-page.js`. 
2. Add the following line of code to the `<head>` section of `detail-page.html`:
```html
 <script src="detail-page.js"></script>
```

You are all set up!

> ## 👌 Pro-tip
> The user story that belongs to this feature is:
> _A user can leave their name and write a comment, when they click `submit`, their name and comment will be displayed on the page._
>
> To accomplish this user story, you have to split it up in smaller steps. If often helps to write these steps out, to keep track of your progress and help formulate questions if you get stuck. In this case, that would look something like:
> * [X] Create an input field for the name, one for the comment and an `submit`-button
> * [ ] Add an event (name and comment) listener/handler to the button
> * [ ] Gather data of the input fields 
> * [ ] Create some elements (to display the data)
> * [ ] Adjust the elements so they display the data
> * [ ] Display the adjusted elements on your page
> * [ ] Empty the input fields so the next user can type some new text.

#### Add an event listener
In this part, we'll add an event listener/handler to the submit button.

1. Click on the `post your comment`-button. What happens?
2. Inspect the following line, which is taken from `detail-page.html`. What is the event listener? Which handler did we assign to it?
```html
<form onsubmit="submitComment(); return false">
```
3. In `detail-page.js` declare a function called `submitComment`. In the function body, log the string 'Hello!' to the console.

4. Check your code in the browser, in the console tab of your DevTools. 

5. Experiment with your code!
    * What happens if you click the button multiple times?
    * What happens if your remove `return false` from the `<form onsubmit="submitComment(); return false">` in `detail-page.html`?

> ## 😱  Sanity Check
> The code in `detail-page.js` should contain this code:
> ```js
> function submitComment() {
>   console.log('Hello!')
> }

>  _❗️ Code not working? Your `submitComment`-function is only called once you click the button, so the string 'Hello!' will only show up once you clicked it!_ 

#### Push your work to GH:
1. Stage your changes, commit them and push them to GitHub:

```shell
$ git add .
$ git commit -m 'Set up js files and declare submitComment'
$ ggpush
```


## 🎯 Learning Goal Tracker
In this section, you learned...

* [X] how to declare and call functions
* [X] how to check JavaScript in your DevTools
* [ ] how to store data in a variable
* [ ] how to select elements from a page
* [ ] how to create elements using JavaScript
* [ ] how to (re)assign values to a property of a DOM-element
* [ ] how to display newly created elements
* [ ] how to use control flow for form validation
