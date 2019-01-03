# Form Validations

## 🎨 What we will build
By then end of this section, your page will look like this one: 
![display comments](https://cd.sseu.re/Een_vrolijke_vioolspeler_2018-12-11_15-28-08.png)


## 🎯 Learning Goals
By the end of this section, you will learn:
* [ ] how to use control flow for form validation

## 📚 Modules that will be discussed
  * [JavaScript 4]()
  * [JavaScript 5]()
  * [JavaScript 6]()
 

## ✏️ Assignments

#### No Empty Comments
Right now, a user can add an empty comment: ![empty comment](https://cd.sseu.re/Een_vrolijke_vioolspeler_2018-12-18_10-02-52.png) That is not very useful, so let's do something about it!

1. Use the `console.log` method to check what the values of your `name` and `msg` variables are if you do not type anything in the the input fields.
2. What happens if you put your `console.log()` statement outside of your `submitComment`-function? Why?
3. Write a boolean expression which returns true if `name` **or** `msg` return a falsy value. Use `console.log` to check whether your logic is correct.

> ## 👌 Pro-tip
> Split up your testing in smaller pieces and later together! This will make it easier to see if and where things go wrong. Also, use strings in your `console.log()` statement to specify which results are displayed. For example:
> ![check boolean expression](https://cd.sseu.re/Een_vrolijke_vioolspeler_2018-12-18_10-14-25.png)

> ## 😱  Sanity Check
> Your boolean expression should look like this:
> ```javascript
>   !name || !msg
>```

3. Add an if statement in your `submitButton` function. If the value of `name` OR `msg` have falsy values, we want to `return null`. Else, we'll continue with the logic we defined in the last section.

## Displaying an error
Now we don't have empty comments, but our user might get somewhat frustrated if they don't know why their comments are nor displaying. So let's communicate what is wrong!

1. Above the return statement in your `if`-code block, add the following line: 
```javascript  
  alert('You forgot to fill in your name or message!')
```
2. What happens if you put this line under your `return` statement? Why?
3. What happens if you remove the line `return null` from your `if`-statement?

#### Short comments
Comments should be short. Let's filter out comments that are too long.
1. Write an if statement that checks whether a comment is longer than 280 characters. If it is, the comment should not be displayed on the page and the user should get a warning that the comment is too long.

> ## 👌 Pro-tip
> Not working as expected? Try to `console.log` the length of your message first!

#### Separate function
To prevent code that is too long and make sure our function does not get too powerful, we'll move our validation logic in a separate function.

1. Declare a function called `doesNotPassAllValidations` which has two parameters: `name` and `msg`.
2. Your function should always return a boolean.
3. If the `name` or `msg` have falsy values, or if the `msg` is too long, your function should give the appropriate alerts and return `true`.
4. Else is should not give any alerts and return `false`.
6. Replace your current `if`-statements with the following logic: If `doesNotPassAllValidations()` returns true, `submitComment` should return `null`. Else it should perform the logic we defined earlier.

> ## 😱  Sanity Check
> `detail-page.js` should contain the following code:
```javascript
function doesNotPassAllValidations(name, msg) {
  if (!name || !msg) {
    alert('You forgot to fill in your name or message!')
    return true;
  }

  if(msg.length > 280) {
    alert('Your comment is too long')
    return true
  }

  return false
}

function submitComment() {
  // ... gather data logic ..

  // check if user input passes validations
  if(doesNotPassAllValidations(name, msg)){
    return null
  }
  // ...
```

#### Extra: More validations:
1. Display a separate message if only the `name` or the `message` input field are not filled in.
2. If a name does not start with a capital letter, change the first letter to `upperCase`.
3. Check whether you message contains inappropriate language. If they do, return the comment with the warning: `Warning: this comment has been flagged as offensive`. Style it in an appropriate way.


#### Push your work to GH:
1. Stage your changes, commit them and push them to GitHub:

```shell
$ git add .
$ git commit -m 'Set Up Form Validation'
$ ggpush
```

> ## 👌 Pro-tip
> Noticed all the `console.log`s we did? We use a method we like to call _check yourself before you wreck yourself_: check whether every bit of code you write does what you think it does, this will help you spotting errors.
> 
> However this is a method that is useful for you, not so much for the final product. It is good practice to remove all unecessary logs and comments from your code before you push to GitHub.

#### Merge your branch
Merge your branch and pull the latest version from master!

## 🎯 Learning Goal Tracker
In this section, you learned...

* [X] how to declare and call functions
* [X] how to check JavaScript in your DevTools
* [X] how to store data in a variable
* [X] how to select elements from a page
* [X] how to create elements using JavaScript
* [X] how to (re)assign values to a property of a DOM-element
* [X] how to display newly created elements
* [X] how to use control flow for form validation
