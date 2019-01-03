# Building All The Boxes

## 🎨 What we will build
By then end of this section, you will be able to log your comments to the console: 
![comment element](https://cd.sseu.re/Een_vrolijke_vioolspeler_2018-12-11_15-18-09.png)


## 🎯 Learning Goals
By the end of this section, you will learn:
* [X] how to store data in a variable
* [X] how to select elements from a page
* [X] how to create elements using JavaScript
* [X] how to (re)assign values to a property of a DOM-element

## 📚 Modules that will be discussed
  * [JavaScript 1]()
  * [JavaScript 2]()
  * [JavaScript 3]()
  * [JavaScript 4]()
  * [DOM 1]()

## ✏️ Assignments
#### Gather data
Let's see whether we can get the values of our input fields are store them in some variables.


1. Inside your `submitComment`-function, declare a variable `inputField` and assign it the element with the id 'name'.

2. Log the inputField to the console to check whether you found the right element.

> ## 😱  Sanity Check
> `detail-page.js` should contain this code:
> ```js
> function submitComment() {
>   const inputField = document.getElementById('name')
>   console.log(inputField)
> }

3. Since `inputField` is a DOM-element, it is an object with properties. Inside `submitComment`, declare a new variable called `name` and assign it the value of the `value` property of `inputField`. Log the `name` variable to the console.

4. In the browser, write your name in the `name`-input field and click submit. Do you see your name in the console tab of the DevTools?

> ## 😱  Sanity Check
> `detail-page.js` should contain this code:
> ```js
> function submitComment() {
>   const inputField = document.getElementById('name')
>   const name = inputField.value
>   console.log(name)
> }

5. Follow the same steps to gather the data of your textarea (which has the idea 'msg'), store the data from this input field in a variable called `msg`.

> ## 😱  Sanity Check
> `detail-page.js` should contain this code:
> ```javascript
> function submitComment() {
>   const inputField = document.getElementById('name')
>   const name = inputField.value
>   const textArea = document.getElementById('msg')
>   const msg = textArea.value
>   console.log(msg)
> }
> ```

#### Create the elements you need
1. Inspect the example page to see in which type of elementts are used to display a comment:
![inspect comment](https://cd.sseu.re/Een_vrolijke_vioolspeler_2018-12-11_11-56-51.png)

2. Create a `<section>` element and store it in a variable called `comment`, using the following code:
```javascript
 function submitComment() {
  //  ...
  const msg = textArea.value
  const comment = document.createElement('section')
 }
```

3. Create an `<h3>` element and store it in the variable `h3`. Log the `h3` variable to the console to check whether it worked.
4. Create a `<p>` element and store it in the variable `p`. Check in you console whether it works out as expected.

> ## 😱  Sanity Check
> `detail-page.js` should contain this code:
> ```javascript
> // add event handler
> function submitComment() {
>   // gather data
>   const inputField = document.getElementById('name')
>   const name = inputField.value
>   const textArea = document.getElementById('msg')
>   const msg = textArea.value
>   
>   // create the elements you need
>   const comment = document.createElement('section')
>   const h3 = document.createElement('h3')
>   const p = document.createElement('p')
> }
> ```

#### Adjust the elements you created
Let's combine the data we gathered with the elements we just created!

1. Reassign the `innerHTML` property of your `h3`-variable to the value of \`${name} said:\`.
1. Reassign the `innerHTML` property of your `p`-variable to the value of `msg`.
1. Use the `add`-method of the `classList` property on your `comment`-variable to add the class `'comment'` to it class-attribute.
1. Use the `appendChild`-method on your `comment` to add your `h3` and `p` variables to it.
1. Log your comment variable to the console to check whether your element looks as  it should:
![comment element](https://cd.sseu.re/Een_vrolijke_vioolspeler_2018-12-11_15-18-09.png)

> ## 😱  Sanity Check
> `detail-page.js` should contain this code:
> ```javascript
> // add event handler
> function submitComment() {
>   // ...
>   
>   // create the elements you need
>   const comment = document.createElement('section')
>   const h3 = document.createElement('h3')
>   const p = document.createElement('p')
>
>   // adjust the elements we created
>   h3.innerHTML = `${name} said:`
>   p.innerHTML = msg
>   comment.classList.add('comment')
>   comment.appendChild(h3)
>   comment.appendChild(p)
> 
>   console.log(comment)
> }
> ```

#### Push your work to GH:
1. Stage your changes, commit them and push them to GitHub:

```shell
$ git add .
$ git commit -m 'Create elements with data from form'
$ ggpush
```


## 🎯 Learning Goal Tracker
In this section, you learned...
* [X] how to declare and call functions
* [X] how to check JavaScript in your DevTools
* [X] how to store data in a variable
* [X] how to select elements from a page
* [X] how to create elements using JavaScript
* [X] how to (re)assign values to a property of a DOM-element
* [ ] how to display newly created elements
* [ ] how to use control flow for form validation

**TODO**
