# Set Up Your HTML

## 🎨 What we will build
By then end of this section, your page will look like this one: 
![final result](https://cd.sseu.re/Museum_Guide_2018-11-28_18-03-17.png)

## 🎯 Learning Goals
By the end of this section, you will learn:

* [ ] how to create an HTML page in your text editor and open it in the browser


## 📚 Modules that will be discussed

  * [HTML 1]()
  * [Git 2](orGitHub?)

## ✏️ Assignments
#### Setting Up your HTML Page
It is time to start for real! Let's set up your basic frame work of your HTML page and open it in the browser!

1. In your terminal, navigate into your `museum-app` directory:
![navigate to project](https://cd.sseu.re/1._mimiCodaisseursMBP2_codaisseurweek-1museum-app_zsh_2018-11-28_17-46-22.png)

2. Because we are starting on a new part of our project, we will be creating a new branch. Create a new one and check it out with the command: `git checkout -b feat/structure-index-and-detail-page`:

![create new branch](https://cd.sseu.re/1._mimiCodaisseursMBP2_codaisseurweek-1museum-app_zsh_2018-11-29_17-12-12.png)

3. Open the `museum-app` project in visual studio code using `code .`

4. Click in the side bar and press `a` to create a new file. Call it `index.html`.

5. Add the `DOCTYPE` and `html` elements to your file by copying the following code:
 ```
<!DOCTYPE html>
<html>
  
</html>
```

6. Add a `head`- element and a `body` element between your `html` opening and closing tag.

7. Inside your `head`- element, add a `title` element with the content: 'Museum Guide'.

8. In your browser press `cmd + o` or `ctrl o` to open a new file. Select `index.html` in your project:
![open project in browser](https://cd.sseu.re/Monosnap_2018-11-28_17-58-27.png)

> ## 👌 Pro-tip
> Not sure where to find your file? In your terminal, in your project directory, print the working directory with `pwd`!

9. Your page should look like the image below. Do you know why the page is empty?
![Result](https://cd.sseu.re/Museum_Guide_2018-11-28_18-01-35.png)

> ## 😱  Sanity Check
> Your code should now look like this:
>```html
><!DOCTYPE html>
><html>
>  <head>
>    <title>Museum Guide</title>
>  </head>
>  <body>
>
>  </body>
></html>
>```

10. Stage your changes, commit them and push them to GitHub:

```shell
$ git add .
$ git commit -m 'Set up basic framework HTML'
$ ggpush
```

11. Check on the GitHub repository page whether your changes were pushed. You should see this line:
![new push on branch on GitHub](https://cd.sseu.re/MimiMagmuseum-app_2018-11-28_18-11-10.png)

>  _❗️ If it did not work, make sure you 1) did not copy the dollar sign, 2) added the `.` after `git add` and 3) copied the commands one line at the time!_ 



## 🎯 Learning Goal Tracker
In this section, you learned...

* [X] how to navigate and do basic management of the file system from the shell
* [X] how to use git & gitHub for version tracking
* [X] how to use Chrome DevTools to inspect the HTML of a page
* [X] how to create an HTML page in your text editor and open it in the browser
* [ ] some important HTML tags, and when/why you should use them
