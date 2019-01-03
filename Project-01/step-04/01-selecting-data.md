# Building All The Boxes

## 🎨 What we will build
By then end of this section, you will have set up your app to use a data set from the Rijksmuseum api.

## 🎯 Learning Goals
By the end of this section, you will learn:
* [ ] to recognize composite data structures.
* [ ] to select specific data from complex data structures.

## 📚 Modules that will be discussed
  * [Internat 1](https://readest.codaisseur.com/courses/beginner-bootcamp/all-bb-modules/internet-1)
  * [JavaScript 3](https://readest.codaisseur.com/courses/beginner-bootcamp/all-bb-modules/javascript-3/objects)

## ✏️ Assignments

#### New Branch
Create a new branch and call it `feat/paintings-from-data`. Check it out!

#### Setup
In the [next section](), you see an example of a `response` you might get from the Rijksmuseum API, which we stored in the variable `data`. First we'll copy this data structure into your project so we can play around with it.

1. In the root directory of your project, create an `index.js` file an link it to your `index.html`.
2. Copy the example data [next section]() into `index.js`.
3. In the console tab of your DevTools, type the name of your variable (`data`) and hit enter. The result should look something like this:
![data in DevTools](https://cd.sseu.re/Museum_Guide_2019-01-03_09-34-49.png)


#### Recognizing composite Data Structures 
Answer the following question about the data variable you just copied into your project:

* Which composite data type is the `data` variable?
* How many elements does the `artObjects` array have?
* Which data type has the value that belongs to the property `countFacets`?
* Which data type has the value that belongs to the property `productionPlaces`?

#### Selecting Data
You can access the value of elapsedMilliseconds with the command `data.elapsedMilliseconds`. How can you access the following values?

* The value of the `count` property?
* The value of the `ondisplay` property of the object that belong to `countFacets`?
* The array that belongs to the property `artObjects`?
* The value of the `title` property of the first element of the `artObjects` array?
* The value of the `width` property of the `webImage` property of the 3rd element of the `artObjects` array?

> ## 👌 Pro-tip
> Use the console tab in your DevTools to try whether your answers are correct!

#### Super Secret Section

> ## 😱  Sanity Check
>
> **⚠️ ! Spoiler Alert ! ⚠️**
>
> These are the answers to the questions above:
>
> * The type of the `data` variable is `object`
> * The `artObjects` array has 10 elements
> * The data type of the value of the `countFacets` property is `object`.
> * The data type of the value of the `productionPlaces` property is `array`.
> 
> * You can select the value of the `count` property through `data.count`
> * You can select the value of the `ondisplay` property through `data.countFacets.ondisplay`.
> * You can select the array that belongs to the property `artObjects` through `data.artObjects`.
> * You can select the value of the `title` property of the first element of the `artObjects` array through `data.artObjects[0].title`.
> * You can select the value of the `width` property of the `webImage` property of the 3rd element of the `artObjects` array through `data.artObjects[2].webImage.width`.

> ## 👌 Pro-tip
> Something like `data.artObjects[5].links.self` becomes pretty tough to understand pretty quickly. We usually like to split code like this into smaller variables, to improve readability. Trying to write code that is not only functional, but also readable (for other developers) and easily maintainable is referred to as the practice of **Clean Coding**.

## 🎯 Learning Goal Tracker
In this section, you learned...
* [X] to recognize composite data structures.
* [X] to select specific data from complex data structures.
