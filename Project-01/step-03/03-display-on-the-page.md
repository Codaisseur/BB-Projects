# Building All The Boxes

## 🎨 What we will build
By then end of this section, your page will look like this one: 
![display comments](https://cd.sseu.re/Een_vrolijke_vioolspeler_2018-12-11_15-28-08.png)


## 🎯 Learning Goals
By the end of this section, you will learn:
* [ ] how to display newly created elements

## 📚 Modules that will be discussed
  * [JavaScript 1]()
  * [JavaScript 2]()
  * [JavaScript 3]()
  * [JavaScript 4]()
  * [DOM 1]()

## ✏️ Assignments
#### Display the elements on the page
Time to display our work on our page!

1. Notice that the one comment we displayed, is part of the section with the id `comments`: ![comments section](https://cd.sseu.re/Een_vrolijke_vioolspeler_2018-12-11_15-15-12.png) Select this element using the `getElementById`-method and store it in the variable `commentSection`.
1. Log `commentSection` in the console to see whether you selected the correct element.
1. Use the `appendChild`-method on `commentSection` to add your `comment`-variable to `commentSection`.

> ## 😱  Sanity Check
> You should now be able to add a comment:
> ![display comments](https://cd.sseu.re/Een_vrolijke_vioolspeler_2018-12-11_15-28-08.png)

#### Empty the form
Let's reset the input fields!

1. Reassign the `value`-property of `inputField` to `null`.
1. Reassign the `value`-property of `textArea` to `null`.

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
>
>   // adjust the elements we created
>   h3.innerHTML = `${name} said:`
>   p.innerHTML = msg
>   comment.classList.add('comment')
>   comment.appendChild(h3)
>   comment.appendChild(p)
> 
>   // display the elements on the page
>   const commentSection = document.getElementById('comments')
>   commentSection.appendChild(comment)
>
>   // reset form values
>   inputField.value = null
>   textArea.value = null
> }
> ```

#### Push your work to GH:
1. Stage your changes, commit them and push them to GitHub:

```shell
$ git add .
$ git commit -m 'Display elements and reset form'
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
* [X] how to display newly created elements
* [ ] how to use control flow for form validation
