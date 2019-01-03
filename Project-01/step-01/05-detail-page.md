# Building A detail page

## 🎨 What we will build
By then end of this section, your page will look like this one: 
![final result](https://cd.sseu.re/Museum_Guide_2018-11-28_18-03-17.png)

## 🎯 Learning Goals
By the end of this section, you will learn:

* [ ] how to navigate and do basic management of the file system from the shell
* [ ] how to use git & gitHub for version tracking
* [ ] how to use Chrome DevTools to inspect the HTML of a page
* [ ] how to create an HTML page in your text editor and open it in the browser
* [ ] some important HTML tags, and when/why you should use them

## 📚 Modules that will be discussed

  * [HTML 1](or2?)
  * [Git 2](orGitHub?)

## ✏️ Assignments
#### Set up the page
In this exercises, we'll help you to set up the page. We'll cheat a bit, we are only going to create one and link all our anchor elements towards that one page.

1. In your terminal, in your `museum-app`, create a new project directory called `pages` using the `mkdir` command.
2. In Visual Studio Code, inside your `pages` directory, create a file called `detail-page.html`.
3. In your browser, check whether you are redirected to your details-page when you click on an image. Your page should look like this:
![result exercise 1](https://cd.sseu.re/Monosnap_2018-11-29_17-02-54.png)

#### Add all elements
This is your moment to shine! Inspect the detail page of the [example app]() using your Chrome DevTools and add the elements you find to your detail page.

By the end, your page should look something like this:
![result exercise 2](https://cd.sseu.re/Monosnap_2018-11-29_17-01-52.png)
 
#### Push to GitHub
Push your work to GitHub!

```shell
$ git add .
$ git commit -m 'Create index page'
$ ggpush
```

#### Merge into master
We build our feature! Let's merge everything into master.

1. Checkout your GitHub repository page and click the green button:
![Create PR](https://cd.sseu.re/Monosnap_2018-11-29_17-14-47.png)
2. Add a description and press the green button again:
![Add description](https://cd.sseu.re/Comparing_master...featindex-page__MimiMagmuseum-app_2018-11-29_17-37-49.png)
3. If there are no merging conflicts, press the button `merge pull request`:
![Merge PR](https://cd.sseu.re/Featstructure-index-page_by_MimiMag__Pull_Request_1__MimiMagmuseum-app_2018-11-29_17-39-19.png)
4. Click confirm merge:
![Confirm Merge](https://cd.sseu.re/Featstructure-index-page_by_MimiMag__Pull_Request_1__MimiMagmuseum-app_2018-11-29_17-40-28.png)

> ## 😱  Sanity Check
> If it worked the page looks like this:
> ![Succes](https://cd.sseu.re/Featstructure-index-page_by_MimiMag__Pull_Request_1__MimiMagmuseum-app_2018-11-29_17-42-32.png)

5. In your terminal, in `museum-app` checkout the master branch and pull the latest version from origin:
```shell
$ git checkout master
$ ggpull
```

## 🎯 Learning Goal Tracker
In this section, you learned...

* [X] how to navigate and do basic management of the file system from the shell
* [X] how to use git & gitHub for version tracking
* [X] how to use Chrome DevTools to inspect the HTML of a page
* [X] how to create an HTML page in your text editor and open it in the browser
* [X] some important HTML tags, and when/why you should use them
